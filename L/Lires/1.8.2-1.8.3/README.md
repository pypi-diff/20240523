# Comparing `tmp/Lires-1.8.2.tar.gz` & `tmp/Lires-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lires-1.8.2.tar", last modified: Mon May 20 12:44:45 2024, max compression
+gzip compressed data, was "Lires-1.8.3.tar", last modified: Thu May 23 07:04:54 2024, max compression
```

## Comparing `Lires-1.8.2.tar` & `Lires-1.8.3.tar`

### file list

```diff
@@ -1,799 +1,1250 @@
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.325412 Lires-1.8.2/
--rw-r--r--   0 monsoon    (501) staff       (20)    12292 2024-03-31 03:58:34.000000 Lires-1.8.2/.DS_Store
--rw-r--r--   0 monsoon    (501) staff       (20)      201 2024-04-12 02:47:00.000000 Lires-1.8.2/.dockerignore
--rw-r--r--   0 monsoon    (501) staff       (20)      957 2024-04-19 03:46:55.000000 Lires-1.8.2/.gitignore
--rw-r--r--   0 monsoon    (501) staff       (20)    35119 2024-04-12 02:47:00.000000 Lires-1.8.2/LICENSE
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.074220 Lires-1.8.2/Lires.egg-info/
--rw-r--r--   0 monsoon    (501) staff       (20)    42286 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/PKG-INFO
--rw-r--r--   0 monsoon    (501) staff       (20)    33405 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/SOURCES.txt
--rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/dependency_links.txt
--rw-r--r--   0 monsoon    (501) staff       (20)      361 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/entry_points.txt
--rw-r--r--   0 monsoon    (501) staff       (20)      345 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/requires.txt
--rw-r--r--   0 monsoon    (501) staff       (20)       43 2024-05-20 12:44:45.000000 Lires-1.8.2/Lires.egg-info/top_level.txt
--rw-r--r--   0 monsoon    (501) staff       (20)      161 2024-04-16 02:14:56.000000 Lires-1.8.2/MANIFEST.in
--rw-r--r--   0 monsoon    (501) staff       (20)      802 2024-05-16 05:47:03.000000 Lires-1.8.2/Makefile
--rw-r--r--   0 monsoon    (501) staff       (20)    42286 2024-05-20 12:44:45.325243 Lires-1.8.2/PKG-INFO
--rw-r--r--   0 monsoon    (501) staff       (20)     1161 2024-05-12 03:26:10.000000 Lires-1.8.2/README.md
--rw-r--r--   0 monsoon    (501) staff       (20)      781 2024-04-12 02:50:06.000000 Lires-1.8.2/compose.yaml
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.076478 Lires-1.8.2/lires/
--rw-r--r--   0 monsoon    (501) staff       (20)       51 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/__init__.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.078265 Lires-1.8.2/lires/api/
--rw-r--r--   0 monsoon    (501) staff       (20)      318 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/api/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3780 2024-05-20 11:41:32.000000 Lires-1.8.2/lires/api/ai.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4595 2024-05-20 12:33:56.000000 Lires-1.8.2/lires/api/common.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1258 2024-05-20 11:41:32.000000 Lires-1.8.2/lires/api/feed.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1498 2024-05-20 11:41:32.000000 Lires-1.8.2/lires/api/log.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4110 2024-05-20 11:18:33.000000 Lires-1.8.2/lires/api/registry.py
--rw-r--r--   0 monsoon    (501) staff       (20)    10335 2024-05-20 11:16:25.000000 Lires-1.8.2/lires/api/server.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.081305 Lires-1.8.2/lires/cmd/
--rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2799 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/_update_db.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1276 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/clear.py
--rw-r--r--   0 monsoon    (501) staff       (20)     8250 2024-05-20 09:58:11.000000 Lires-1.8.2/lires/cmd/cluster.py
--rw-r--r--   0 monsoon    (501) staff       (20)      329 2024-04-19 03:46:55.000000 Lires-1.8.2/lires/cmd/generateDefaultConf.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3660 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/index.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1890 2024-04-19 03:46:55.000000 Lires-1.8.2/lires/cmd/invite.py
--rw-r--r--   0 monsoon    (501) staff       (20)    10143 2024-05-16 05:05:15.000000 Lires-1.8.2/lires/cmd/log.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1355 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/miscUtils.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1322 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/cmd/status.py
--rw-r--r--   0 monsoon    (501) staff       (20)     7474 2024-05-20 05:01:25.000000 Lires-1.8.2/lires/cmd/userManage.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5735 2024-05-20 09:59:01.000000 Lires-1.8.2/lires/config.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.085299 Lires-1.8.2/lires/core/
--rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)      426 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/base.py
--rw-r--r--   0 monsoon    (501) staff       (20)     6900 2024-05-12 03:26:10.000000 Lires-1.8.2/lires/core/bibReader.py
--rw-r--r--   0 monsoon    (501) staff       (20)    13792 2024-05-15 07:35:26.000000 Lires-1.8.2/lires/core/dataClass.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5983 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/dataSearcher.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5276 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/dataTags.py
--rw-r--r--   0 monsoon    (501) staff       (20)    34238 2024-05-12 03:26:10.000000 Lires-1.8.2/lires/core/dbConn.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2089 2024-05-15 07:35:26.000000 Lires-1.8.2/lires/core/dbConnUpgrade.py
--rw-r--r--   0 monsoon    (501) staff       (20)    11540 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/dbConn_.py
--rw-r--r--   0 monsoon    (501) staff       (20)      796 2024-05-20 04:24:49.000000 Lires-1.8.2/lires/core/error.py
--rw-r--r--   0 monsoon    (501) staff       (20)    14702 2024-05-12 03:26:10.000000 Lires-1.8.2/lires/core/fileTools.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5148 2024-05-05 09:42:09.000000 Lires-1.8.2/lires/core/logger.py
--rw-r--r--   0 monsoon    (501) staff       (20)     8035 2024-05-12 03:26:10.000000 Lires-1.8.2/lires/core/pdfTools.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.085940 Lires-1.8.2/lires/core/refparser/
--rw-r--r--   0 monsoon    (501) staff       (20)       34 2024-04-12 02:47:00.000000 Lires-1.8.2/lires/core/refparser/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2542 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/refparser/endnote.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1978 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/refparser/interface.py
--rw-r--r--   0 monsoon    (501) staff       (20)    12026 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/core/vector.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3366 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/exec.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2952 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/loader.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3339 2024-04-19 03:46:55.000000 Lires-1.8.2/lires/parser.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.086484 Lires-1.8.2/lires/types/
--rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:47:00.000000 Lires-1.8.2/lires/types/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1411 2024-05-20 09:59:59.000000 Lires-1.8.2/lires/types/configT.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1330 2024-05-15 07:35:26.000000 Lires-1.8.2/lires/types/dataT.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.087654 Lires-1.8.2/lires/user/
--rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-04-12 02:47:00.000000 Lires-1.8.2/lires/user/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)    11341 2024-05-20 04:55:04.000000 Lires-1.8.2/lires/user/conn.py
--rw-r--r--   0 monsoon    (501) staff       (20)      340 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/user/encrypt.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2637 2024-04-19 03:46:55.000000 Lires-1.8.2/lires/user/loader.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5014 2024-05-17 03:55:32.000000 Lires-1.8.2/lires/user/object.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.090434 Lires-1.8.2/lires/utils/
--rw-r--r--   0 monsoon    (501) staff       (20)      549 2024-05-17 03:47:55.000000 Lires-1.8.2/lires/utils/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)      837 2024-05-08 01:17:51.000000 Lires-1.8.2/lires/utils/author.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1989 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/utils/compressTools.py
--rw-r--r--   0 monsoon    (501) staff       (20)      955 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/utils/fs.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4352 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/utils/log.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1877 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/utils/network.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1875 2024-05-20 10:06:53.000000 Lires-1.8.2/lires/utils/random.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3779 2024-05-19 01:40:00.000000 Lires-1.8.2/lires/utils/term.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3459 2024-04-12 02:50:06.000000 Lires-1.8.2/lires/utils/time.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2065 2024-05-12 03:26:10.000000 Lires-1.8.2/lires/version.py
--rw-r--r--   0 monsoon    (501) staff       (20)    28005 2024-05-20 12:42:43.000000 Lires-1.8.2/lires/version.yaml
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.091793 Lires-1.8.2/lires_server/
--rw-r--r--   0 monsoon    (501) staff       (20)       40 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_server/__init__.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.092069 Lires-1.8.2/lires_server/assets/
--rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_server/assets/.gitkeep
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.092662 Lires-1.8.2/lires_server/assets/docs/
--rw-r--r--   0 monsoon    (501) staff       (20)     8525 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/404.html
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.109235 Lires-1.8.2/lires_server/assets/docs/assets/
--rw-r--r--   0 monsoon    (501) staff       (20)     1372 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/app.CngJ_OZF.js
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.110965 Lires-1.8.2/lires_server/assets/docs/assets/chunks/
--rw-r--r--   0 monsoon    (501) staff       (20)    87906 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/chunks/framework.CZXUNLJW.js
--rw-r--r--   0 monsoon    (501) staff       (20)    52675 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/chunks/theme.CfuCmiaJ.js
--rw-r--r--   0 monsoon    (501) staff       (20)     9036 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.js
--rw-r--r--   0 monsoon    (501) staff       (20)      438 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3256 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_enviromentVariables.md.C9ixW2VB.js
--rw-r--r--   0 monsoon    (501) staff       (20)      479 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_enviromentVariables.md.C9ixW2VB.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)    11668 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_gettingStarted.md.DpAQEIqk.js
--rw-r--r--   0 monsoon    (501) staff       (20)      460 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_gettingStarted.md.DpAQEIqk.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)      929 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.js
--rw-r--r--   0 monsoon    (501) staff       (20)      929 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)    10132 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.js
--rw-r--r--   0 monsoon    (501) staff       (20)      444 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3030 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.js
--rw-r--r--   0 monsoon    (501) staff       (20)      459 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     4130 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.js
--rw-r--r--   0 monsoon    (501) staff       (20)      414 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     1534 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.js
--rw-r--r--   0 monsoon    (501) staff       (20)      409 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/index.md.DPNZS3UP.js
--rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/index.md.DPNZS3UP.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)    43112 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-cyrillic-ext.r48I6akx.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    31300 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-cyrillic.By2_1cv3.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    17404 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-greek-ext.1u6EdAuj.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    32564 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-greek.DJ8dCoTZ.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)   120840 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-latin-ext.CN1xVJS-.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    74784 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-latin.C2AdPX0b.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    14884 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-vietnamese.BSbpV94h.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    40488 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-cyrillic-ext.BBPuwvHQ.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    29164 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-cyrillic.C5lxZ8CY.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    16272 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-greek-ext.CqjqNYQ-.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    29920 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-greek.BBVDIX6e.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)   110160 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-latin-ext.4ZJIpNVo.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    67792 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-latin.Di8DUHzh.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)    14072 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-vietnamese.BjW4sHH5.woff2
--rw-r--r--   0 monsoon    (501) staff       (20)     2253 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.js
--rw-r--r--   0 monsoon    (501) staff       (20)      434 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3548 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.js
--rw-r--r--   0 monsoon    (501) staff       (20)      454 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)    31211 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.js
--rw-r--r--   0 monsoon    (501) staff       (20)      403 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     4253 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.js
--rw-r--r--   0 monsoon    (501) staff       (20)      439 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.js
--rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3203 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.js
--rw-r--r--   0 monsoon    (501) staff       (20)      448 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3766 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.js
--rw-r--r--   0 monsoon    (501) staff       (20)      415 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3939 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_user-interface.md.pJkOzfoZ.js
--rw-r--r--   0 monsoon    (501) staff       (20)      445 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/manual_user-interface.md.pJkOzfoZ.lean.js
--rw-r--r--   0 monsoon    (501) staff       (20)   118471 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/assets/style.CT5GXN_K.css
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.113672 Lires-1.8.2/lires_server/assets/docs/deployment/
--rw-r--r--   0 monsoon    (501) staff       (20)    25537 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/docker.html
--rw-r--r--   0 monsoon    (501) staff       (20)    19744 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/enviromentVariables.html
--rw-r--r--   0 monsoon    (501) staff       (20)    28144 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/gettingStarted.html
--rw-r--r--   0 monsoon    (501) staff       (20)    17340 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/index.html
--rw-r--r--   0 monsoon    (501) staff       (20)    26650 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/manage.html
--rw-r--r--   0 monsoon    (501) staff       (20)    19517 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/deployment/obsidianPlugin.html
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.114042 Lires-1.8.2/lires_server/assets/docs/dev/
--rw-r--r--   0 monsoon    (501) staff       (20)    20614 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/dev/index.html
--rw-r--r--   0 monsoon    (501) staff       (20)    17795 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/dev/roadmap.html
--rw-r--r--   0 monsoon    (501) staff       (20)      580 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/hashmap.json
--rw-r--r--   0 monsoon    (501) staff       (20)     9290 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/index.html
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.117552 Lires-1.8.2/lires_server/assets/docs/manual/
--rw-r--r--   0 monsoon    (501) staff       (20)    18754 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/add-document.html
--rw-r--r--   0 monsoon    (501) staff       (20)    20042 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/add-edit-entry.html
--rw-r--r--   0 monsoon    (501) staff       (20)    47679 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/api.html
--rw-r--r--   0 monsoon    (501) staff       (20)    20739 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/filter-entry.html
--rw-r--r--   0 monsoon    (501) staff       (20)    16985 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/index.html
--rw-r--r--   0 monsoon    (501) staff       (20)    19669 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/obsidianPlugin.html
--rw-r--r--   0 monsoon    (501) staff       (20)    20272 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/read.html
--rw-r--r--   0 monsoon    (501) staff       (20)    20416 2024-05-20 12:44:15.000000 Lires-1.8.2/lires_server/assets/docs/manual/user-interface.html
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.117986 Lires-1.8.2/lires_server/assets/js-api/
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.118475 Lires-1.8.2/lires_server/assets/js-api/api/
--rw-r--r--   0 monsoon    (501) staff       (20)      715 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/api/fetcher.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     2348 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/api/protocol.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     4759 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/api/serverConn.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     1564 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/api/serverWebsocketConn.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     9355 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/api.js
--rw-r--r--   0 monsoon    (501) staff       (20)       28 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/app.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.118831 Lires-1.8.2/lires_server/assets/js-api/components/
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.118947 Lires-1.8.2/lires_server/assets/js-api/components/common/
--rw-r--r--   0 monsoon    (501) staff       (20)     4279 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/common/fragments.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.119064 Lires-1.8.2/lires_server/assets/js-api/components/editor/
--rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/editor/blockInterface.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.119178 Lires-1.8.2/lires_server/assets/js-api/components/home/
--rw-r--r--   0 monsoon    (501) staff       (20)      554 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/home/bibtexUtils.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      559 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/interface.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     2762 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/store.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      153 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/components/wstate.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      386 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/config.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.120074 Lires-1.8.2/lires_server/assets/js-api/core/
--rw-r--r--   0 monsoon    (501) staff       (20)      421 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/auth.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     2448 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/dataClass.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      302 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/markdownParse.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      783 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/misc.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      973 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/tag.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      471 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/user.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      273 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/core/vueInterface.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.120555 Lires-1.8.2/lires_server/assets/js-api/state/
--rw-r--r--   0 monsoon    (501) staff       (20)      378 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/state/authorState.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      559 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/state/interface.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     2810 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/state/store.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      153 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/state/wstate.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.121320 Lires-1.8.2/lires_server/assets/js-api/utils/
--rw-r--r--   0 monsoon    (501) staff       (20)      479 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/arxiv.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      236 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/cookie.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/file.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)     1024 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/logging.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      623 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/misc.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)       66 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/sha256lib.d.ts
--rw-r--r--   0 monsoon    (501) staff       (20)      350 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_server/assets/js-api/utils/timeUtils.d.ts
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.122285 Lires-1.8.2/lires_server/assets/obsidian-plugin/
--rw-r--r--   0 monsoon    (501) staff       (20)    10130 2024-05-20 12:44:12.000000 Lires-1.8.2/lires_server/assets/obsidian-plugin/main.js
--rw-r--r--   0 monsoon    (501) staff       (20)      247 2024-05-20 12:44:12.000000 Lires-1.8.2/lires_server/assets/obsidian-plugin/manifest.json
--rw-r--r--   0 monsoon    (501) staff       (20)     1344 2024-05-20 12:44:12.000000 Lires-1.8.2/lires_server/assets/obsidian-plugin/styles.css
--rw-r--r--   0 monsoon    (501) staff       (20)       23 2024-05-20 12:44:12.000000 Lires-1.8.2/lires_server/assets/obsidian-plugin/versions.json
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.123245 Lires-1.8.2/lires_server/assets/pdf-viewer/
--rw-r--r--   0 monsoon    (501) staff       (20)    10174 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/LICENSE
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.146035 Lires-1.8.2/lires_server/assets/pdf-viewer/build/
--rw-r--r--   0 monsoon    (501) staff       (20)   800420 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.mjs
--rw-r--r--   0 monsoon    (501) staff       (20)  1774612 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.mjs.map
--rw-r--r--   0 monsoon    (501) staff       (20)   925564 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs
--rw-r--r--   0 monsoon    (501) staff       (20)   780290 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs.map
--rw-r--r--   0 monsoon    (501) staff       (20)  2294368 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.worker.mjs
--rw-r--r--   0 monsoon    (501) staff       (20)  5343574 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.worker.mjs.map
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.171386 Lires-1.8.2/lires_server/assets/pdf-viewer/web/
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.240165 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/
--rw-r--r--   0 monsoon    (501) staff       (20)     2404 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      173 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2379 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2398 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      173 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2651 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      290 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      905 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/83pv-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      721 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      290 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      715 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      291 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      982 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2419 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2413 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      287 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      282 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      317 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-0.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      371 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-1.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      376 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      401 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-3.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      405 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-4.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-5.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-6.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    41193 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-UCS2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      217 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-0.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      250 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-1.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      465 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      470 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-3.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      601 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-4.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      625 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-5.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    33974 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-UCS2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      225 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-0.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      226 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-1.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      233 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      242 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-3.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      337 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-4.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      430 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-5.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      485 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-6.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    40951 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-UCS2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      241 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-0.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      386 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-1.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      391 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    23293 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-UCS2.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1086 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1099 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5pc-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      144 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5pc-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1780 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1920 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      706 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS1-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      143 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS1-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      504 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS2-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     4426 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1125 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      101 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETenms-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      172 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETenms-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2536 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2542 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      218 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      215 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      549 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      179 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      528 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      175 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    14692 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      180 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    19662 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      219 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    14686 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     7290 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      180 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     7269 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      176 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     7298 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      182 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      557 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      553 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2654 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2414 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2292 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1772 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2171 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     4437 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      159 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      132 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Hankaku.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      124 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Hiragana.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1848 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      164 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     1831 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    16791 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      160 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2787 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2789 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2024 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      100 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Katakana.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)     2080 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/LICENSE
--rw-r--r--   0 monsoon    (501) staff       (20)     2765 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/NWP-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      252 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/NWP-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      534 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)       96 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Roman.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    48280 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      156 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    50419 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      156 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    52679 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      160 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    53629 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      157 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    43366 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      193 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    44086 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      178 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    45738 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      182 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    46837 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    25439 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      119 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      680 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      664 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    39443 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      643 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    40539 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      677 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    41695 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      678 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    39534 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      647 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    40630 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    41779 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      682 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      705 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-HW-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      689 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      726 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    40517 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      684 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    40608 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      688 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    25783 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      178 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    26327 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      164 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    26451 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      168 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)    27790 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-H.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/V.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)      179 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/WP-Symbol.bcmap
--rw-r--r--   0 monsoon    (501) staff       (20)  1016315 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/compressed.tracemonkey-pldi-09.pdf
--rw-r--r--   0 monsoon    (501) staff       (20)     2421 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/debugger.css
--rw-r--r--   0 monsoon    (501) staff       (20)    18003 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/debugger.mjs
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.256374 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/
--rw-r--r--   0 monsoon    (501) staff       (20)      920 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/altText_add.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1087 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/altText_done.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      415 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-check.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      883 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-comment.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     2168 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-help.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      408 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-insert.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1452 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-key.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      426 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-newparagraph.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-noicon.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1041 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-note.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      552 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-paperclip.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1143 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-paragraph.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1375 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-pushpin.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     2936 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeHighlight.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1452 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeText.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1323 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorInk.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     5402 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorTextHighlight.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      909 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/editor-toolbar-delete.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/findbarButton-next.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/findbarButton-previous.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      782 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/gv-toolbarButton-download.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     2545 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/loading-icon.gif
--rw-r--r--   0 monsoon    (501) staff       (20)     1559 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/loading.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      417 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-documentProperties.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-firstPage.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1344 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-handTool.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      257 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-lastPage.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      596 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCcw.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      576 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCw.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      971 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollHorizontal.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      731 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollPage.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      969 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollVertical.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1228 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollWrapped.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1085 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-selectTool.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      775 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadEven.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      395 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadNone.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      711 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadOdd.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      861 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-bookmark.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      607 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-currentOutlineItem.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1036 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-download.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      498 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorFreeText.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      910 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorHighlight.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1189 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorInk.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      734 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorStamp.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-menuArrow.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1400 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-openFile.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      701 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageDown.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      682 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageUp.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-presentationMode.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      927 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-print.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1234 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-search.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1080 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-secondaryToolbarToggle.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1560 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-sidebarToggle.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      570 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewAttachments.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      671 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewLayers.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      332 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewOutline.svg
--rw-r--r--   0 monsoon    (501) staff       (20)     1396 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewThumbnail.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      958 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomIn.svg
--rw-r--r--   0 monsoon    (501) staff       (20)      472 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomOut.svg
--rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/treeitem-collapsed.svg
--rw-r--r--   0 monsoon    (501) staff       (20)       94 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/treeitem-expanded.svg
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.256511 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.256671 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ach/
--rw-r--r--   0 monsoon    (501) staff       (20)     7983 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ach/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.256904 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/af/
--rw-r--r--   0 monsoon    (501) staff       (20)     7365 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/af/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.257110 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/an/
--rw-r--r--   0 monsoon    (501) staff       (20)    10101 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/an/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.257480 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ar/
--rw-r--r--   0 monsoon    (501) staff       (20)    17907 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ar/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.257801 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ast/
--rw-r--r--   0 monsoon    (501) staff       (20)     7246 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ast/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.258132 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/az/
--rw-r--r--   0 monsoon    (501) staff       (20)    10136 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/az/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.258365 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/be/
--rw-r--r--   0 monsoon    (501) staff       (20)    19586 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/be/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.258735 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bg/
--rw-r--r--   0 monsoon    (501) staff       (20)    19196 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bg/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.259161 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bn/
--rw-r--r--   0 monsoon    (501) staff       (20)    12486 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bn/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.259734 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bo/
--rw-r--r--   0 monsoon    (501) staff       (20)     9120 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bo/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.260076 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/br/
--rw-r--r--   0 monsoon    (501) staff       (20)    12137 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/br/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.260313 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/brx/
--rw-r--r--   0 monsoon    (501) staff       (20)    10555 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/brx/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.260838 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bs/
--rw-r--r--   0 monsoon    (501) staff       (20)     8299 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bs/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.261119 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ca/
--rw-r--r--   0 monsoon    (501) staff       (20)    11724 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ca/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.262014 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cak/
--rw-r--r--   0 monsoon    (501) staff       (20)    11480 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cak/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.262185 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ckb/
--rw-r--r--   0 monsoon    (501) staff       (20)    10564 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ckb/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.262354 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cs/
--rw-r--r--   0 monsoon    (501) staff       (20)    16308 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cs/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.262621 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cy/
--rw-r--r--   0 monsoon    (501) staff       (20)    16060 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cy/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.262860 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/da/
--rw-r--r--   0 monsoon    (501) staff       (20)    15685 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/da/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.263123 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/de/
--rw-r--r--   0 monsoon    (501) staff       (20)    16228 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/de/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.263385 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/dsb/
--rw-r--r--   0 monsoon    (501) staff       (20)    16483 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/dsb/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.263620 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/el/
--rw-r--r--   0 monsoon    (501) staff       (20)    20103 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/el/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.264004 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-CA/
--rw-r--r--   0 monsoon    (501) staff       (20)    15240 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-CA/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.264341 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-GB/
--rw-r--r--   0 monsoon    (501) staff       (20)    15236 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-GB/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.264595 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-US/
--rw-r--r--   0 monsoon    (501) staff       (20)    14945 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-US/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.264853 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eo/
--rw-r--r--   0 monsoon    (501) staff       (20)    15723 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eo/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.265541 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-AR/
--rw-r--r--   0 monsoon    (501) staff       (20)    16102 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-AR/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.265823 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-CL/
--rw-r--r--   0 monsoon    (501) staff       (20)    16276 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-CL/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.265988 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-ES/
--rw-r--r--   0 monsoon    (501) staff       (20)    16262 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-ES/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.266269 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-MX/
--rw-r--r--   0 monsoon    (501) staff       (20)    11638 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-MX/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.266522 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/et/
--rw-r--r--   0 monsoon    (501) staff       (20)    10270 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/et/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.266717 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eu/
--rw-r--r--   0 monsoon    (501) staff       (20)    16029 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eu/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.266983 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fa/
--rw-r--r--   0 monsoon    (501) staff       (20)    10211 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fa/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.267238 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ff/
--rw-r--r--   0 monsoon    (501) staff       (20)     9192 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ff/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.267487 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fi/
--rw-r--r--   0 monsoon    (501) staff       (20)    15838 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fi/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.267747 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fr/
--rw-r--r--   0 monsoon    (501) staff       (20)    16493 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.267912 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fur/
--rw-r--r--   0 monsoon    (501) staff       (20)    16217 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fur/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.268213 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fy-NL/
--rw-r--r--   0 monsoon    (501) staff       (20)    15786 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fy-NL/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.268870 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ga-IE/
--rw-r--r--   0 monsoon    (501) staff       (20)     7833 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ga-IE/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.269101 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gd/
--rw-r--r--   0 monsoon    (501) staff       (20)    12039 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gd/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.269348 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gl/
--rw-r--r--   0 monsoon    (501) staff       (20)    14760 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.269653 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gn/
--rw-r--r--   0 monsoon    (501) staff       (20)    16393 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gn/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.270004 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gu-IN/
--rw-r--r--   0 monsoon    (501) staff       (20)    12479 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gu-IN/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.270479 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/he/
--rw-r--r--   0 monsoon    (501) staff       (20)    17270 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/he/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.270838 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hi-IN/
--rw-r--r--   0 monsoon    (501) staff       (20)    12614 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hi-IN/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.271343 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hr/
--rw-r--r--   0 monsoon    (501) staff       (20)    10824 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.271594 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hsb/
--rw-r--r--   0 monsoon    (501) staff       (20)    16491 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hsb/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.271756 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hu/
--rw-r--r--   0 monsoon    (501) staff       (20)    16193 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hu/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.271958 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hy-AM/
--rw-r--r--   0 monsoon    (501) staff       (20)    11360 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hy-AM/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.272211 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hye/
--rw-r--r--   0 monsoon    (501) staff       (20)    12628 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hye/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.272453 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ia/
--rw-r--r--   0 monsoon    (501) staff       (20)    16129 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ia/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.272816 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/id/
--rw-r--r--   0 monsoon    (501) staff       (20)    11055 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/id/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.273160 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/is/
--rw-r--r--   0 monsoon    (501) staff       (20)    15797 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/is/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.273381 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/it/
--rw-r--r--   0 monsoon    (501) staff       (20)    16107 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/it/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.273660 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ja/
--rw-r--r--   0 monsoon    (501) staff       (20)    17233 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ja/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.274351 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ka/
--rw-r--r--   0 monsoon    (501) staff       (20)    21596 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ka/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.274915 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kab/
--rw-r--r--   0 monsoon    (501) staff       (20)    13066 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kab/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.275099 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kk/
--rw-r--r--   0 monsoon    (501) staff       (20)    19315 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kk/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.275291 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/km/
--rw-r--r--   0 monsoon    (501) staff       (20)    11385 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/km/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.275679 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kn/
--rw-r--r--   0 monsoon    (501) staff       (20)    10661 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kn/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.275894 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ko/
--rw-r--r--   0 monsoon    (501) staff       (20)    16084 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ko/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.276077 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lij/
--rw-r--r--   0 monsoon    (501) staff       (20)     9467 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lij/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.276354 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lo/
--rw-r--r--   0 monsoon    (501) staff       (20)    15113 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lo/viewer.ftl
--rw-r--r--   0 monsoon    (501) staff       (20)     2498 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/locale.json
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.276529 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lt/
--rw-r--r--   0 monsoon    (501) staff       (20)    10633 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lt/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.276819 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ltg/
--rw-r--r--   0 monsoon    (501) staff       (20)     9311 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ltg/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.277154 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lv/
--rw-r--r--   0 monsoon    (501) staff       (20)     9383 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lv/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.277773 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/meh/
--rw-r--r--   0 monsoon    (501) staff       (20)     2260 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/meh/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.278019 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mk/
--rw-r--r--   0 monsoon    (501) staff       (20)     9659 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mk/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.278194 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mr/
--rw-r--r--   0 monsoon    (501) staff       (20)    11774 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.278498 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ms/
--rw-r--r--   0 monsoon    (501) staff       (20)     9194 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ms/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.278804 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/my/
--rw-r--r--   0 monsoon    (501) staff       (20)    10184 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/my/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.279364 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nb-NO/
--rw-r--r--   0 monsoon    (501) staff       (20)    15318 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nb-NO/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.279643 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ne-NP/
--rw-r--r--   0 monsoon    (501) staff       (20)    12084 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ne-NP/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.279901 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nl/
--rw-r--r--   0 monsoon    (501) staff       (20)    16046 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.280171 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nn-NO/
--rw-r--r--   0 monsoon    (501) staff       (20)    13671 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nn-NO/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.280534 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/oc/
--rw-r--r--   0 monsoon    (501) staff       (20)    13879 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/oc/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.280806 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pa-IN/
--rw-r--r--   0 monsoon    (501) staff       (20)    19797 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pa-IN/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.281167 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pl/
--rw-r--r--   0 monsoon    (501) staff       (20)    16341 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.281580 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-BR/
--rw-r--r--   0 monsoon    (501) staff       (20)    15777 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-BR/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.281864 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-PT/
--rw-r--r--   0 monsoon    (501) staff       (20)    16189 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-PT/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.282207 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/rm/
--rw-r--r--   0 monsoon    (501) staff       (20)    16267 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/rm/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.283252 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ro/
--rw-r--r--   0 monsoon    (501) staff       (20)     9862 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ro/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.283516 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ru/
--rw-r--r--   0 monsoon    (501) staff       (20)    19808 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ru/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.283690 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sat/
--rw-r--r--   0 monsoon    (501) staff       (20)    16483 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sat/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.283958 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sc/
--rw-r--r--   0 monsoon    (501) staff       (20)    11569 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sc/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.284412 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/scn/
--rw-r--r--   0 monsoon    (501) staff       (20)     1593 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/scn/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.284656 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sco/
--rw-r--r--   0 monsoon    (501) staff       (20)     9776 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sco/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.285182 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/si/
--rw-r--r--   0 monsoon    (501) staff       (20)    12008 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/si/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.285621 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sk/
--rw-r--r--   0 monsoon    (501) staff       (20)    16522 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sk/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.285822 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/skr/
--rw-r--r--   0 monsoon    (501) staff       (20)    17922 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/skr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.287476 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sl/
--rw-r--r--   0 monsoon    (501) staff       (20)    15522 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.287862 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/son/
--rw-r--r--   0 monsoon    (501) staff       (20)     7026 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/son/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.288217 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sq/
--rw-r--r--   0 monsoon    (501) staff       (20)    15426 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sq/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.288394 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sr/
--rw-r--r--   0 monsoon    (501) staff       (20)    13848 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.288664 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sv-SE/
--rw-r--r--   0 monsoon    (501) staff       (20)    15598 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sv-SE/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.288961 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/szl/
--rw-r--r--   0 monsoon    (501) staff       (20)     9898 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/szl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.289125 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ta/
--rw-r--r--   0 monsoon    (501) staff       (20)    11748 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ta/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.289533 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/te/
--rw-r--r--   0 monsoon    (501) staff       (20)    11843 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/te/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.289760 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tg/
--rw-r--r--   0 monsoon    (501) staff       (20)    19364 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tg/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.289939 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/th/
--rw-r--r--   0 monsoon    (501) staff       (20)    20722 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/th/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.290599 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tl/
--rw-r--r--   0 monsoon    (501) staff       (20)    10011 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tl/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.290750 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tr/
--rw-r--r--   0 monsoon    (501) staff       (20)    15949 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tr/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.291206 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/trs/
--rw-r--r--   0 monsoon    (501) staff       (20)     7141 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/trs/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.291484 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uk/
--rw-r--r--   0 monsoon    (501) staff       (20)    19271 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uk/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.291808 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ur/
--rw-r--r--   0 monsoon    (501) staff       (20)    10357 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ur/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.292115 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uz/
--rw-r--r--   0 monsoon    (501) staff       (20)     6557 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uz/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.292390 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/vi/
--rw-r--r--   0 monsoon    (501) staff       (20)    16690 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/vi/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.292669 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/wo/
--rw-r--r--   0 monsoon    (501) staff       (20)     3505 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/wo/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.292936 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/xh/
--rw-r--r--   0 monsoon    (501) staff       (20)     7776 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/xh/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.293169 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-CN/
--rw-r--r--   0 monsoon    (501) staff       (20)    14940 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-CN/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.293471 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-TW/
--rw-r--r--   0 monsoon    (501) staff       (20)    15113 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-TW/viewer.ftl
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.304709 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/
--rw-r--r--   0 monsoon    (501) staff       (20)    29513 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitDingbats.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    17597 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixed.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    18055 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBold.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    19151 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBoldItalic.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    18746 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedItalic.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    19469 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerif.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    19395 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBold.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    20733 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBoldItalic.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    21227 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifItalic.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)    16729 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSymbol.pfb
--rw-r--r--   0 monsoon    (501) staff       (20)     1553 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_FOXIT
--rw-r--r--   0 monsoon    (501) staff       (20)     4414 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_LIBERATION
--rw-r--r--   0 monsoon    (501) staff       (20)   137052 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Bold.ttf
--rw-r--r--   0 monsoon    (501) staff       (20)   135124 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-BoldItalic.ttf
--rw-r--r--   0 monsoon    (501) staff       (20)   162036 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Italic.ttf
--rw-r--r--   0 monsoon    (501) staff       (20)   139512 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Regular.ttf
--rw-r--r--   0 monsoon    (501) staff       (20)   120678 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.css
--rw-r--r--   0 monsoon    (501) staff       (20)    33051 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.html
--rw-r--r--   0 monsoon    (501) staff       (20)   645923 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.mjs
--rw-r--r--   0 monsoon    (501) staff       (20)  1369119 2024-05-06 04:24:45.000000 Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.mjs.map
--rw-r--r--   0 monsoon    (501) staff       (20)      240 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_server/config.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.312298 Lires-1.8.2/lires_server/handlers/
--rw-r--r--   0 monsoon    (501) staff       (20)      540 2024-05-12 03:26:10.000000 Lires-1.8.2/lires_server/handlers/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)    11750 2024-05-20 12:36:41.000000 Lires-1.8.2/lires_server/handlers/_base.py
--rw-r--r--   0 monsoon    (501) staff       (20)      770 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_server/handlers/_global_data.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4530 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/apiFiles.py
--rw-r--r--   0 monsoon    (501) staff       (20)      309 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/auth.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2432 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/dataFeature.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1540 2024-05-12 03:26:10.000000 Lires-1.8.2/lires_server/handlers/dataInfo.py
--rw-r--r--   0 monsoon    (501) staff       (20)     7061 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/dataMan.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1086 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/databaseInfo.py
--rw-r--r--   0 monsoon    (501) staff       (20)     6199 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/documents.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2776 2024-05-20 12:37:00.000000 Lires-1.8.2/lires_server/handlers/feed.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2773 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/fileinfo_supp.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1405 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/iServerProxy.py
--rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_server/handlers/info.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5310 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/misc.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5259 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/miscFiles.py
--rw-r--r--   0 monsoon    (501) staff       (20)      621 2024-05-06 04:16:18.000000 Lires-1.8.2/lires_server/handlers/pdfjs.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4078 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/search.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4009 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/summary.py
--rw-r--r--   0 monsoon    (501) staff       (20)     6405 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/user.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5422 2024-05-20 04:55:10.000000 Lires-1.8.2/lires_server/handlers/userMan.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2512 2024-05-18 10:22:08.000000 Lires-1.8.2/lires_server/handlers/websocket.py
--rw-r--r--   0 monsoon    (501) staff       (20)     9155 2024-05-12 03:26:10.000000 Lires-1.8.2/lires_server/main.py
--rw-r--r--   0 monsoon    (501) staff       (20)      903 2024-05-12 03:26:10.000000 Lires-1.8.2/lires_server/types.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.312765 Lires-1.8.2/lires_service/
--rw-r--r--   0 monsoon    (501) staff       (20)      240 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/__init__.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.314221 Lires-1.8.2/lires_service/ai/
--rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/__init__.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.314509 Lires-1.8.2/lires_service/ai/cmd/
--rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/cmd/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1413 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/cmd/summarize.py
--rw-r--r--   0 monsoon    (501) staff       (20)      801 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/globalConfig.py
--rw-r--r--   0 monsoon    (501) staff       (20)    11805 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/lmInterface.py
--rw-r--r--   0 monsoon    (501) staff       (20)     5977 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/lmTools.py
--rw-r--r--   0 monsoon    (501) staff       (20)     4519 2024-05-20 03:40:05.000000 Lires-1.8.2/lires_service/ai/server.py
--rw-r--r--   0 monsoon    (501) staff       (20)      131 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/ai/utils.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2513 2024-05-20 09:58:18.000000 Lires-1.8.2/lires_service/entry.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.314934 Lires-1.8.2/lires_service/log/
--rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/log/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     2249 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/log/logger.py
--rw-r--r--   0 monsoon    (501) staff       (20)     3378 2024-05-15 05:55:43.000000 Lires-1.8.2/lires_service/log/server.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.315552 Lires-1.8.2/lires_service/registry/
--rw-r--r--   0 monsoon    (501) staff       (20)      213 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/registry/__init__.py
--rw-r--r--   0 monsoon    (501) staff       (20)     1967 2024-05-20 11:13:45.000000 Lires-1.8.2/lires_service/registry/server.py
--rw-r--r--   0 monsoon    (501) staff       (20)     7010 2024-04-12 02:50:06.000000 Lires-1.8.2/lires_service/registry/store.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.315798 Lires-1.8.2/lires_web/
--rw-r--r--   0 monsoon    (501) staff       (20)       98 2024-04-19 03:46:55.000000 Lires-1.8.2/lires_web/__init__.py
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.316837 Lires-1.8.2/lires_web/dist/
-drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-20 12:44:45.324963 Lires-1.8.2/lires_web/dist/assets/
--rw-r--r--   0 monsoon    (501) staff       (20)   936012 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/@codemirror-4Zn9bE8B.js
--rw-r--r--   0 monsoon    (501) staff       (20)   606218 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/@lezer-tqr6QOpM.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2285 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/@vavt-DtLj4T47.js
--rw-r--r--   0 monsoon    (501) staff       (20)    72194 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/@vue-D_lT-ze_.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3178 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/async-mutex-CSJywVGb.js
--rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/codemirror-l0sNRNKZ.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2386 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/copy-to-clipboard-B1uT6SkR.js
--rw-r--r--   0 monsoon    (501) staff       (20)      623 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/crelt-C8TCjufn.js
--rw-r--r--   0 monsoon    (501) staff       (20)     9206 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/cssfilter-BjxKUPhv.js
--rw-r--r--   0 monsoon    (501) staff       (20)    32370 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/entities-C20TfXL6.js
--rw-r--r--   0 monsoon    (501) staff       (20)      297 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/extend-shallow-DA8A8LGH.js
--rw-r--r--   0 monsoon    (501) staff       (20)    25090 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/fast-xml-parser-CJG3bOwu.js
--rw-r--r--   0 monsoon    (501) staff       (20)     6319 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/gray-matter-D4hcLa5V.js
--rw-r--r--   0 monsoon    (501) staff       (20)   149729 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/index-DVZewPDh.js
--rw-r--r--   0 monsoon    (501) staff       (20)    47791 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/index-Umoxfe5H.css
--rw-r--r--   0 monsoon    (501) staff       (20)      259 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/is-extendable-CiA4f1iz.js
--rw-r--r--   0 monsoon    (501) staff       (20)    39551 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/js-yaml-B7yGoGZD.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2307 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/kind-of-l3izQsJJ.js
--rw-r--r--   0 monsoon    (501) staff       (20)     9137 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/linkify-it-DmNjr4Kv.js
--rw-r--r--   0 monsoon    (501) staff       (20)    49352 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/markdown-it-DI8MEbma.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2276 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/markdown-it-image-figures-BD49Kf-b.js
--rw-r--r--   0 monsoon    (501) staff       (20)     1864 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/markdown-it-task-lists-BNI9E7ji.js
--rw-r--r--   0 monsoon    (501) staff       (20)      529 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/markdown-it-xss-DEpVfk-m.js
--rw-r--r--   0 monsoon    (501) staff       (20)    89568 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/md-editor-v3-92WZKX8v.css
--rw-r--r--   0 monsoon    (501) staff       (20)   109482 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/md-editor-v3-CPol1xJ_.js
--rw-r--r--   0 monsoon    (501) staff       (20)     4884 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/mdurl-k9Sl0PQj.js
--rw-r--r--   0 monsoon    (501) staff       (20)     9497 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/medium-zoom-bWEtUbjf.js
--rw-r--r--   0 monsoon    (501) staff       (20)      195 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/node-stdlib-browser-d7cmxmpa.js
--rw-r--r--   0 monsoon    (501) staff       (20)     3545 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/pinia-BHWH00Pk.js
--rw-r--r--   0 monsoon    (501) staff       (20)  3766714 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/plotly.js-dist-FakLekxN.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2408 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/punycode.js-Dj65hjkv.js
--rw-r--r--   0 monsoon    (501) staff       (20)     1259 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/section-matter-DWrNKXO4.js
--rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/strip-bom-string-BxrG9K6S.js
--rw-r--r--   0 monsoon    (501) staff       (20)     1071 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/strnum-u8jQhLSb.js
--rw-r--r--   0 monsoon    (501) staff       (20)     2195 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/style-mod-Bc2inJdb.js
--rw-r--r--   0 monsoon    (501) staff       (20)      423 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/toggle-selection-BHUZwh74.js
--rw-r--r--   0 monsoon    (501) staff       (20)     5216 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/uc.micro-kMc2yuuw.js
--rw-r--r--   0 monsoon    (501) staff       (20)    29392 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/vite-plugin-node-polyfills-Cgl3E5jI.js
--rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/vue-l0sNRNKZ.js
--rw-r--r--   0 monsoon    (501) staff       (20)    23092 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/vue-router-DNoSD41y.js
--rw-r--r--   0 monsoon    (501) staff       (20)     1494 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/w3c-keyname-Vcq4gwWv.js
--rw-r--r--   0 monsoon    (501) staff       (20)     8902 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/assets/xss-DnjGkJ2-.js
--rw-r--r--   0 monsoon    (501) staff       (20)    16446 2024-05-20 12:44:33.000000 Lires-1.8.2/lires_web/dist/favicon.ico
--rw-r--r--   0 monsoon    (501) staff       (20)     3763 2024-05-20 12:44:35.000000 Lires-1.8.2/lires_web/dist/index.html
--rw-r--r--   0 monsoon    (501) staff       (20)     1859 2024-05-16 05:23:50.000000 Lires-1.8.2/pyproject.toml
--rw-r--r--   0 monsoon    (501) staff       (20)     1385 2024-05-16 07:46:18.000000 Lires-1.8.2/requirements.py
--rw-r--r--   0 monsoon    (501) staff       (20)       38 2024-05-20 12:44:45.325452 Lires-1.8.2/setup.cfg
--rw-r--r--   0 monsoon    (501) staff       (20)      614 2024-04-12 02:50:06.000000 Lires-1.8.2/setup.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.488357 Lires-1.8.3/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12292 2024-03-31 03:58:34.000000 Lires-1.8.3/.DS_Store
+-rw-r--r--   0 monsoon    (501) staff       (20)      168 2024-05-22 08:36:02.000000 Lires-1.8.3/.dockerignore
+-rw-r--r--   0 monsoon    (501) staff       (20)    35119 2024-04-12 02:47:00.000000 Lires-1.8.3/LICENSE
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.066805 Lires-1.8.3/Lires.egg-info/
+-rw-r--r--   0 monsoon    (501) staff       (20)      152 2024-05-23 07:04:54.000000 Lires-1.8.3/Lires.egg-info/PKG-INFO
+-rw-r--r--   0 monsoon    (501) staff       (20)    53494 2024-05-23 07:04:54.000000 Lires-1.8.3/Lires.egg-info/SOURCES.txt
+-rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-23 07:04:54.000000 Lires-1.8.3/Lires.egg-info/dependency_links.txt
+-rw-r--r--   0 monsoon    (501) staff       (20)       43 2024-05-23 07:04:54.000000 Lires-1.8.3/Lires.egg-info/top_level.txt
+-rw-r--r--   0 monsoon    (501) staff       (20)      319 2024-05-23 04:07:01.000000 Lires-1.8.3/MANIFEST.in
+-rw-r--r--   0 monsoon    (501) staff       (20)      864 2024-05-23 06:12:53.000000 Lires-1.8.3/Makefile
+-rw-r--r--   0 monsoon    (501) staff       (20)      152 2024-05-23 07:04:54.488218 Lires-1.8.3/PKG-INFO
+-rw-r--r--   0 monsoon    (501) staff       (20)     1161 2024-05-12 03:26:10.000000 Lires-1.8.3/README.md
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.050794 Lires-1.8.3/external/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.050845 Lires-1.8.3/external/eigen/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.073052 Lires-1.8.3/external/eigen/Eigen/
+-rw-r--r--   0 monsoon    (501) staff       (20)     2086 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/AccelerateSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     1155 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Cholesky
+-rw-r--r--   0 monsoon    (501) staff       (20)     1922 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/CholmodSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)    13464 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Core
+-rw-r--r--   0 monsoon    (501) staff       (20)      122 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Dense
+-rw-r--r--   0 monsoon    (501) staff       (20)       35 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Eigen
+-rw-r--r--   0 monsoon    (501) staff       (20)     1825 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Eigenvalues
+-rw-r--r--   0 monsoon    (501) staff       (20)     1986 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Geometry
+-rw-r--r--   0 monsoon    (501) staff       (20)      882 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Householder
+-rw-r--r--   0 monsoon    (501) staff       (20)     2164 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 monsoon    (501) staff       (20)      942 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Jacobi
+-rw-r--r--   0 monsoon    (501) staff       (20)     1412 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/KLUSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     1266 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/LU
+-rw-r--r--   0 monsoon    (501) staff       (20)     1039 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/MetisSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     2436 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/OrderingMethods
+-rw-r--r--   0 monsoon    (501) staff       (20)     1789 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/PaStiXSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     1165 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/PardisoSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     1267 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/QR
+-rw-r--r--   0 monsoon    (501) staff       (20)      897 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/QtAlignedMalloc
+-rw-r--r--   0 monsoon    (501) staff       (20)     1244 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SPQRSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     1663 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SVD
+-rw-r--r--   0 monsoon    (501) staff       (20)      888 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/Sparse
+-rw-r--r--   0 monsoon    (501) staff       (20)     1281 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SparseCholesky
+-rw-r--r--   0 monsoon    (501) staff       (20)     2256 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SparseCore
+-rw-r--r--   0 monsoon    (501) staff       (20)     1819 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SparseLU
+-rw-r--r--   0 monsoon    (501) staff       (20)     1232 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SparseQR
+-rw-r--r--   0 monsoon    (501) staff       (20)      864 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/StdDeque
+-rw-r--r--   0 monsoon    (501) staff       (20)      793 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/StdList
+-rw-r--r--   0 monsoon    (501) staff       (20)      870 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/StdVector
+-rw-r--r--   0 monsoon    (501) staff       (20)     2286 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/SuperLUSupport
+-rw-r--r--   0 monsoon    (501) staff       (20)     2178 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/ThreadPool
+-rw-r--r--   0 monsoon    (501) staff       (20)     1425 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/UmfPackSupport
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.053902 Lires-1.8.3/external/eigen/Eigen/src/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.073557 Lires-1.8.3/external/eigen/Eigen/src/AccelerateSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15066 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/AccelerateSupport/AccelerateSupport.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      160 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/AccelerateSupport/InternalHeaderCheck.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.074845 Lires-1.8.3/external/eigen/Eigen/src/Cholesky/
+-rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Cholesky/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    24801 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    18576 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5315 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.075350 Lires-1.8.3/external/eigen/Eigen/src/CholmodSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)    28515 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      154 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/CholmodSupport/InternalHeaderCheck.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.100567 Lires-1.8.3/external/eigen/Eigen/src/Core/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9935 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15914 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Array.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8132 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6554 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2822 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Assign.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    44731 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11783 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13950 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    20841 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Block.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6277 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7050 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    77423 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4815 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7749 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    37923 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7811 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3874 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7817 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    31525 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    23511 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    28815 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7345 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DeviceWrapper.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9348 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17874 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1056 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11469 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Dot.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6141 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4799 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6029 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22191 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    56710 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    14414 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8393 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/IO.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    14565 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      134 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3473 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7041 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Map.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11239 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    66485 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10866 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    23971 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    23874 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3091 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3634 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    14910 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9576 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    20181 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    48537 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13521 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Product.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    58591 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7652 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Random.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10753 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/RandomImpl.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    23226 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Redux.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    19343 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Ref.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5744 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    16729 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4306 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7485 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7682 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Select.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    14885 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1886 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15808 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/SkewSymmetricMatrix3.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7024 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Solve.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10228 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5885 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8863 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21961 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4325 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Stride.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3129 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Swap.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17725 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13272 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    37944 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3383 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    34109 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    35676 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.052143 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.102394 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15629 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4413 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   100918 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11669 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.107538 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16611 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    48063 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/GemmKernel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4659 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   119904 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    26581 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/PacketMathFP16.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    55588 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/TrsmKernel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    56496 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/TrsmUnrolls.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)    10437 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.111859 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 monsoon    (501) staff       (20)    22571 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2289 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   167055 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10104 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    44669 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    30672 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMAbfloat16.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   132173 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/MatrixVectorProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   126859 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5165 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/AltiVec/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.113433 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 monsoon    (501) staff       (20)    35385 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5880 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   113378 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9041 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    41441 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1736 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.117651 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 monsoon    (501) staff       (20)    18014 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2771 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    56429 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10104 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/Tuple.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2323 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.051708 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.117791 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 monsoon    (501) staff       (20)      643 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.117962 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/HVX/
+-rw-r--r--   0 monsoon    (501) staff       (20)    44382 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/HVX/PacketMath.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.118816 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16973 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15894 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    33218 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.121267 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 monsoon    (501) staff       (20)    23134 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10332 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2147 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   196876 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    62006 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1909 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/NEON/UnaryFunctors.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.122438 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 monsoon    (501) staff       (20)    14004 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2884 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    89836 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7308 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.123499 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 monsoon    (501) staff       (20)     1172 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21167 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1416 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.124457 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7466 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13871 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    24402 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2611 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.125528 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 monsoon    (501) staff       (20)    17293 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7894 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    37093 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.127735 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6566 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    32092 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9882 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4117 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1832 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    48942 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.138175 Lires-1.8.3/external/eigen/Eigen/src/Core/products/
+-rw-r--r--   0 monsoon    (501) staff       (20)   144472 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    20951 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17218 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11310 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9176 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    23183 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10068 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10504 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22530 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    25741 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10159 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7626 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6632 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4360 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    20826 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    31817 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    18182 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    25169 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    19701 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13479 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6010 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.144222 Lires-1.8.3/external/eigen/Eigen/src/Core/util/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6737 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Assert.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    27284 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    18480 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21834 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6228 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8798 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/EmulateArray.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    16434 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    24390 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9491 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4175 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    51587 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4138 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/MaxSizeVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    54912 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21013 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22266 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/MoreMeta.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1519 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1521 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7932 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/Serializer.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5981 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17104 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    43559 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.147755 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12063 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17288 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7514 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22514 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17461 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9497 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13786 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5530 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22195 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21010 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6075 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    35357 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6648 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22346 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.151647 Lires-1.8.3/external/eigen/Eigen/src/Geometry/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19095 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8556 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8357 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    20919 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    12182 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11684 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9992 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    35092 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7035 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8310 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7171 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    63924 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7984 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6396 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.152760 Lires-1.8.3/external/eigen/Eigen/src/Geometry/arch/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6260 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.153531 Lires-1.8.3/external/eigen/Eigen/src/Householder/
+-rw-r--r--   0 monsoon    (501) staff       (20)     4938 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5780 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22888 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Householder/HouseholderSequence.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Householder/InternalHeaderCheck.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.155918 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6583 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6828 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8756 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15955 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    14767 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13395 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7432 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4395 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.156761 Lires-1.8.3/external/eigen/Eigen/src/Jacobi/
+-rw-r--r--   0 monsoon    (501) staff       (20)      138 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Jacobi/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    16977 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.157388 Lires-1.8.3/external/eigen/Eigen/src/KLUSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      146 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/KLUSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11418 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.158720 Lires-1.8.3/external/eigen/Eigen/src/LU/
+-rw-r--r--   0 monsoon    (501) staff       (20)     3743 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    32525 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      130 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    16606 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22492 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4291 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.158938 Lires-1.8.3/external/eigen/Eigen/src/LU/arch/
+-rw-r--r--   0 monsoon    (501) staff       (20)    13885 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.159236 Lires-1.8.3/external/eigen/Eigen/src/MetisSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      150 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/MetisSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4510 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.159942 Lires-1.8.3/external/eigen/Eigen/src/OrderingMethods/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15275 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    62472 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      156 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/OrderingMethods/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5125 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.160225 Lires-1.8.3/external/eigen/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      152 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/PaStiXSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    21331 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.160524 Lires-1.8.3/external/eigen/Eigen/src/PardisoSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      154 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/PardisoSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    19446 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.162129 Lires-1.8.3/external/eigen/Eigen/src/QR/
+-rw-r--r--   0 monsoon    (501) staff       (20)    27408 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8080 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    25798 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    29547 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    19701 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3142 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      130 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/QR/InternalHeaderCheck.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.162379 Lires-1.8.3/external/eigen/Eigen/src/SPQRSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SPQRSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11571 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.163876 Lires-1.8.3/external/eigen/Eigen/src/SVD/
+-rw-r--r--   0 monsoon    (501) staff       (20)    62847 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7396 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/BDCSVD_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      132 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    34877 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    10623 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    19672 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15185 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.164514 Lires-1.8.3/external/eigen/Eigen/src/SparseCholesky/
+-rw-r--r--   0 monsoon    (501) staff       (20)      154 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCholesky/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    33776 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5660 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.176069 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10350 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7689 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    12768 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      146 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11966 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    24051 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6474 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    22913 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    36649 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4689 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    13650 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6067 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3463 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1176 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    12401 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    80786 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17020 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11132 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7614 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1786 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    15433 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    26121 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4497 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9113 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3123 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6170 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7138 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17746 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7670 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9629 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.180518 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/
+-rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    36986 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4451 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7749 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5083 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    12534 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2091 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6737 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6654 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3734 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4023 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6074 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8261 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9042 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     5152 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     4613 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2978 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.180805 Lires-1.8.3/external/eigen/Eigen/src/SparseQR/
+-rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseQR/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    28187 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.181674 Lires-1.8.3/external/eigen/Eigen/src/StlSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)     3254 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3135 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3308 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     2672 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.181936 Lires-1.8.3/external/eigen/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      154 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SuperLUSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    32218 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.185048 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/
+-rw-r--r--   0 monsoon    (501) staff       (20)     2140 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/Barrier.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    16356 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/CoreThreadPoolDevice.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     8863 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/EventCount.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    17060 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/NonBlockingThreadPool.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     9277 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/RunQueue.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      746 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/ThreadCancel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1268 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/ThreadEnvironment.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    11231 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/ThreadLocal.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1708 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/ThreadPoolInterface.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      611 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/ThreadPool/ThreadYield.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.185312 Lires-1.8.3/external/eigen/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 monsoon    (501) staff       (20)      154 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/UmfPackSupport/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)    24448 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.190200 Lires-1.8.3/external/eigen/Eigen/src/misc/
+-rw-r--r--   0 monsoon    (501) staff       (20)     3420 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/Image.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      134 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/InternalHeaderCheck.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3201 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     1795 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6667 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/blas.h
+-rw-r--r--   0 monsoon    (501) staff       (20)   881178 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     6983 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/lapacke_helpers.h
+-rw-r--r--   0 monsoon    (501) staff       (20)      473 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.196825 Lires-1.8.3/external/eigen/Eigen/src/plugins/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15645 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)    23546 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)    63345 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/BlockMethods.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)     6277 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)     6500 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)     9904 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/IndexedViewMethods.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)      137 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/InternalHeaderCheck.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)    17396 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)     4995 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.inc
+-rw-r--r--   0 monsoon    (501) staff       (20)     6824 2024-05-22 07:46:48.000000 Lires-1.8.3/external/eigen/Eigen/src/plugins/ReshapedMethods.inc
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.198738 Lires-1.8.3/lires/
+-rw-r--r--   0 monsoon    (501) staff       (20)       51 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.200719 Lires-1.8.3/lires/api/
+-rw-r--r--   0 monsoon    (501) staff       (20)      318 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/api/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3780 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/ai.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4595 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/common.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1258 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/feed.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1498 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/log.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4110 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/registry.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    10335 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/api/server.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.203373 Lires-1.8.3/lires/cmd/
+-rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/cmd/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2799 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/cmd/_update_db.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1276 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/cmd/clear.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     8250 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/cmd/cluster.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1229 2024-05-23 07:02:13.000000 Lires-1.8.3/lires/cmd/config.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3635 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/cmd/index.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1890 2024-04-19 03:46:55.000000 Lires-1.8.3/lires/cmd/invite.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    10143 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/cmd/log.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1351 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/cmd/miscUtils.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1322 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/cmd/status.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     7474 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/cmd/userManage.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5650 2024-05-23 06:51:23.000000 Lires-1.8.3/lires/config.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.206740 Lires-1.8.3/lires/core/
+-rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      426 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/base.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     6900 2024-05-12 03:26:10.000000 Lires-1.8.3/lires/core/bibReader.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    13801 2024-05-23 02:41:51.000000 Lires-1.8.3/lires/core/dataClass.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5276 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/dataTags.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    34224 2024-05-23 02:45:35.000000 Lires-1.8.3/lires/core/dbConn.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2089 2024-05-15 07:35:26.000000 Lires-1.8.3/lires/core/dbConnUpgrade.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    11540 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/dbConn_.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      796 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/core/error.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    14702 2024-05-12 03:26:10.000000 Lires-1.8.3/lires/core/fileTools.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5148 2024-05-05 09:42:09.000000 Lires-1.8.3/lires/core/logger.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     8035 2024-05-12 03:26:10.000000 Lires-1.8.3/lires/core/pdfTools.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.207319 Lires-1.8.3/lires/core/refparser/
+-rw-r--r--   0 monsoon    (501) staff       (20)       34 2024-04-12 02:47:00.000000 Lires-1.8.3/lires/core/refparser/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2542 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/refparser/endnote.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1978 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/core/refparser/interface.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    10610 2024-05-23 06:16:45.000000 Lires-1.8.3/lires/core/vector.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3271 2024-05-23 06:45:10.000000 Lires-1.8.3/lires/exec.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2965 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/loader.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3237 2024-05-23 04:12:23.000000 Lires-1.8.3/lires/parser.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.207712 Lires-1.8.3/lires/types/
+-rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:47:00.000000 Lires-1.8.3/lires/types/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1272 2024-05-23 06:51:31.000000 Lires-1.8.3/lires/types/configT.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1330 2024-05-15 07:35:26.000000 Lires-1.8.3/lires/types/dataT.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.208764 Lires-1.8.3/lires/user/
+-rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-04-12 02:47:00.000000 Lires-1.8.3/lires/user/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    11341 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/user/conn.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      340 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/user/encrypt.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2637 2024-04-19 03:46:55.000000 Lires-1.8.3/lires/user/loader.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5014 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/user/object.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.210485 Lires-1.8.3/lires/utils/
+-rw-r--r--   0 monsoon    (501) staff       (20)      549 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/utils/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      837 2024-05-08 01:17:51.000000 Lires-1.8.3/lires/utils/author.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1989 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/utils/compressTools.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      955 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/utils/fs.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4352 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/utils/log.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1877 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/utils/network.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1875 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/utils/random.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3779 2024-05-21 10:59:48.000000 Lires-1.8.3/lires/utils/term.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3459 2024-04-12 02:50:06.000000 Lires-1.8.3/lires/utils/time.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.211493 Lires-1.8.3/lires/vector/
+-rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.212485 Lires-1.8.3/lires/vector/c/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6644 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/c/alg.cpp
+-rw-r--r--   0 monsoon    (501) staff       (20)      940 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/c/common.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     3017 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/c/enc.cpp
+-rw-r--r--   0 monsoon    (501) staff       (20)      618 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/c/enc.h
+-rw-r--r--   0 monsoon    (501) staff       (20)     7096 2024-05-22 08:43:00.000000 Lires-1.8.3/lires/vector/database.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3668 2024-05-22 08:36:02.000000 Lires-1.8.3/lires/vector/wrap.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2065 2024-05-12 03:26:10.000000 Lires-1.8.3/lires/version.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    28246 2024-05-23 07:04:25.000000 Lires-1.8.3/lires/version.yaml
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.213713 Lires-1.8.3/lires_server/
+-rw-r--r--   0 monsoon    (501) staff       (20)       40 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_server/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.055344 Lires-1.8.3/lires_server/assets/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.214352 Lires-1.8.3/lires_server/assets/docs/
+-rw-r--r--   0 monsoon    (501) staff       (20)     8525 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/404.html
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.229799 Lires-1.8.3/lires_server/assets/docs/assets/
+-rw-r--r--   0 monsoon    (501) staff       (20)     1372 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/app.CngJ_OZF.js
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.234453 Lires-1.8.3/lires_server/assets/docs/assets/chunks/
+-rw-r--r--   0 monsoon    (501) staff       (20)    87906 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/chunks/framework.CZXUNLJW.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    52675 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/chunks/theme.CfuCmiaJ.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     9036 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      438 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3257 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_enviromentVariables.md.Bts03XC7.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      479 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_enviromentVariables.md.Bts03XC7.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    11572 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_gettingStarted.md.CAqJg6m3.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      460 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_gettingStarted.md.CAqJg6m3.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      929 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      929 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    10132 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      444 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3030 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      459 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     4130 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      414 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     1534 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      409 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/index.md.DPNZS3UP.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/index.md.DPNZS3UP.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    43112 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-cyrillic-ext.r48I6akx.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    31300 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-cyrillic.By2_1cv3.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    17404 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-greek-ext.1u6EdAuj.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    32564 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-greek.DJ8dCoTZ.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)   120840 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-latin-ext.CN1xVJS-.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    74784 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-latin.C2AdPX0b.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    14884 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-vietnamese.BSbpV94h.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    40488 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-cyrillic-ext.BBPuwvHQ.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    29164 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-cyrillic.C5lxZ8CY.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    16272 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-greek-ext.CqjqNYQ-.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    29920 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-greek.BBVDIX6e.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)   110160 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-latin-ext.4ZJIpNVo.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    67792 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-latin.Di8DUHzh.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)    14072 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-vietnamese.BjW4sHH5.woff2
+-rw-r--r--   0 monsoon    (501) staff       (20)     2253 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      434 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3548 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      454 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    31211 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      403 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     4253 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      439 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      758 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3203 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      448 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3766 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      415 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3971 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_user-interface.md.CdSRMwMo.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      445 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/manual_user-interface.md.CdSRMwMo.lean.js
+-rw-r--r--   0 monsoon    (501) staff       (20)   118471 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/assets/style.CT5GXN_K.css
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.237166 Lires-1.8.3/lires_server/assets/docs/deployment/
+-rw-r--r--   0 monsoon    (501) staff       (20)    25537 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/docker.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    19745 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/enviromentVariables.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    28048 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/gettingStarted.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    17340 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/index.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    26650 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/manage.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    19517 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/deployment/obsidianPlugin.html
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.238851 Lires-1.8.3/lires_server/assets/docs/dev/
+-rw-r--r--   0 monsoon    (501) staff       (20)    20614 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/dev/index.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    17795 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/dev/roadmap.html
+-rw-r--r--   0 monsoon    (501) staff       (20)      580 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/hashmap.json
+-rw-r--r--   0 monsoon    (501) staff       (20)     9290 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/index.html
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.242099 Lires-1.8.3/lires_server/assets/docs/manual/
+-rw-r--r--   0 monsoon    (501) staff       (20)    18754 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/add-document.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    20042 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/add-edit-entry.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    47679 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/api.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    20739 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/filter-entry.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    16985 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/index.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    19669 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/obsidianPlugin.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    20272 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/read.html
+-rw-r--r--   0 monsoon    (501) staff       (20)    20448 2024-05-21 06:12:24.000000 Lires-1.8.3/lires_server/assets/docs/manual/user-interface.html
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.243103 Lires-1.8.3/lires_server/assets/js-api/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.244372 Lires-1.8.3/lires_server/assets/js-api/api/
+-rw-r--r--   0 monsoon    (501) staff       (20)      715 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/api/fetcher.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     2348 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/api/protocol.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     4759 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/api/serverConn.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     1564 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/api/serverWebsocketConn.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     9355 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/api.js
+-rw-r--r--   0 monsoon    (501) staff       (20)       28 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/app.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.244856 Lires-1.8.3/lires_server/assets/js-api/components/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.244992 Lires-1.8.3/lires_server/assets/js-api/components/common/
+-rw-r--r--   0 monsoon    (501) staff       (20)     4279 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/common/fragments.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.245841 Lires-1.8.3/lires_server/assets/js-api/components/editor/
+-rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/editor/blockInterface.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.245988 Lires-1.8.3/lires_server/assets/js-api/components/home/
+-rw-r--r--   0 monsoon    (501) staff       (20)      554 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/home/bibtexUtils.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      559 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/interface.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     2762 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/store.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      153 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/components/wstate.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      386 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/config.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.247085 Lires-1.8.3/lires_server/assets/js-api/core/
+-rw-r--r--   0 monsoon    (501) staff       (20)      421 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/auth.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     2448 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/dataClass.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      302 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/markdownParse.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      783 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/misc.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      973 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/tag.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      471 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/user.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      273 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/core/vueInterface.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.247633 Lires-1.8.3/lires_server/assets/js-api/state/
+-rw-r--r--   0 monsoon    (501) staff       (20)      378 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/state/authorState.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      559 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/state/interface.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     2810 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/state/store.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      153 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/state/wstate.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.248560 Lires-1.8.3/lires_server/assets/js-api/utils/
+-rw-r--r--   0 monsoon    (501) staff       (20)      479 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/arxiv.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      236 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/cookie.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/file.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)     1024 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/logging.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      623 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/misc.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)       66 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/sha256lib.d.ts
+-rw-r--r--   0 monsoon    (501) staff       (20)      350 2024-05-21 06:12:42.000000 Lires-1.8.3/lires_server/assets/js-api/utils/timeUtils.d.ts
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.249185 Lires-1.8.3/lires_server/assets/obsidian-plugin/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10130 2024-05-21 06:12:21.000000 Lires-1.8.3/lires_server/assets/obsidian-plugin/main.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      247 2024-05-21 06:12:21.000000 Lires-1.8.3/lires_server/assets/obsidian-plugin/manifest.json
+-rw-r--r--   0 monsoon    (501) staff       (20)     1344 2024-05-21 06:12:21.000000 Lires-1.8.3/lires_server/assets/obsidian-plugin/styles.css
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.250095 Lires-1.8.3/lires_server/assets/pdf-viewer/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10174 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/LICENSE
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.271399 Lires-1.8.3/lires_server/assets/pdf-viewer/build/
+-rw-r--r--   0 monsoon    (501) staff       (20)   800420 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.mjs
+-rw-r--r--   0 monsoon    (501) staff       (20)  1774612 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.mjs.map
+-rw-r--r--   0 monsoon    (501) staff       (20)   925564 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs
+-rw-r--r--   0 monsoon    (501) staff       (20)   780290 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs.map
+-rw-r--r--   0 monsoon    (501) staff       (20)  2294368 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.worker.mjs
+-rw-r--r--   0 monsoon    (501) staff       (20)  5343574 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.worker.mjs.map
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.295775 Lires-1.8.3/lires_server/assets/pdf-viewer/web/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.363007 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/
+-rw-r--r--   0 monsoon    (501) staff       (20)     2404 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      173 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2379 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2398 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      173 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2651 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      290 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      905 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/83pv-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      721 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      290 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      715 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      291 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      982 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2419 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2413 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      287 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      282 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      317 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-0.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      371 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-1.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      376 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      401 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-3.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      405 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-4.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-5.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      406 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-6.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    41193 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-UCS2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      217 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-0.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      250 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-1.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      465 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      470 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-3.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      601 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-4.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      625 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-5.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    33974 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-UCS2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      225 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-0.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      226 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-1.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      233 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      242 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-3.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      337 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-4.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      430 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-5.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      485 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-6.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    40951 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-UCS2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      241 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-0.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      386 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-1.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      391 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    23293 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-UCS2.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1086 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      142 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1099 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5pc-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      144 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5pc-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1780 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1920 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      706 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS1-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      143 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS1-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      504 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS2-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     4426 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1125 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      101 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETenms-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      172 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETenms-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2536 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2542 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      218 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      215 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      549 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      179 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      528 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      175 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    14692 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      180 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    19662 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      219 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    14686 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     7290 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      180 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     7269 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      176 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     7298 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      182 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      557 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      553 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2654 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2414 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      148 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2292 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1772 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2171 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      149 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     4437 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      159 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      132 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Hankaku.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      124 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Hiragana.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1848 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      164 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     1831 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    16791 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      160 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2787 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2789 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2024 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      100 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Katakana.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)     2080 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/LICENSE
+-rw-r--r--   0 monsoon    (501) staff       (20)     2765 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/NWP-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      252 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/NWP-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      534 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      170 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)       96 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Roman.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    48280 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      156 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    50419 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      156 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    52679 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      160 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    53629 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      157 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    43366 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      193 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    44086 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      178 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    45738 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      182 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    46837 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      181 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    25439 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      119 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      680 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      664 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    39443 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      643 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    40539 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      677 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    41695 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      678 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    39534 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      647 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    40630 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    41779 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      682 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      705 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-HW-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      689 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      726 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    40517 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      684 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    40608 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      688 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    25783 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      178 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    26327 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      164 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    26451 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      168 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)    27790 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-H.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      169 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      166 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/V.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)      179 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/WP-Symbol.bcmap
+-rw-r--r--   0 monsoon    (501) staff       (20)  1016315 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/compressed.tracemonkey-pldi-09.pdf
+-rw-r--r--   0 monsoon    (501) staff       (20)     2421 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/debugger.css
+-rw-r--r--   0 monsoon    (501) staff       (20)    18003 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/debugger.mjs
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.377176 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/
+-rw-r--r--   0 monsoon    (501) staff       (20)      920 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/altText_add.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1087 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/altText_done.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      415 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-check.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      883 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-comment.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     2168 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-help.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      408 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-insert.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1452 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-key.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      426 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-newparagraph.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      158 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-noicon.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1041 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-note.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      552 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-paperclip.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1143 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-paragraph.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1375 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-pushpin.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     2936 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeHighlight.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1452 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeText.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1323 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorInk.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     5402 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorTextHighlight.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      909 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/editor-toolbar-delete.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/findbarButton-next.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      578 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/findbarButton-previous.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      782 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/gv-toolbarButton-download.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     2545 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/loading-icon.gif
+-rw-r--r--   0 monsoon    (501) staff       (20)     1559 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/loading.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      417 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-documentProperties.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-firstPage.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1344 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-handTool.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      257 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-lastPage.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      596 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCcw.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      576 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCw.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      971 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollHorizontal.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      731 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollPage.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      969 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollVertical.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1228 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollWrapped.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1085 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-selectTool.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      775 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadEven.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      395 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadNone.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      711 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadOdd.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      861 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-bookmark.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      607 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-currentOutlineItem.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1036 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-download.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      498 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorFreeText.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      910 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorHighlight.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1189 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorInk.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      734 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorStamp.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-menuArrow.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1400 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-openFile.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      701 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageDown.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      682 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageUp.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      681 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-presentationMode.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      927 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-print.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1234 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-search.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1080 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-secondaryToolbarToggle.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1560 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-sidebarToggle.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      570 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewAttachments.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      671 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewLayers.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      332 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewOutline.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1396 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewThumbnail.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      958 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomIn.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)      472 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomOut.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/treeitem-collapsed.svg
+-rw-r--r--   0 monsoon    (501) staff       (20)       94 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/treeitem-expanded.svg
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.377324 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.377457 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ach/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7983 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ach/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.377883 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/af/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7365 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/af/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.378313 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/an/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10101 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/an/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.379450 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ar/
+-rw-r--r--   0 monsoon    (501) staff       (20)    17907 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ar/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.379888 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ast/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7246 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ast/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.380344 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/az/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10136 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/az/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.380576 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/be/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19586 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/be/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.380972 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bg/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19196 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bg/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.381550 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bn/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12486 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bn/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.382059 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bo/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9120 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bo/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.382391 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/br/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12137 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/br/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.382627 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/brx/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10555 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/brx/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.383357 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bs/
+-rw-r--r--   0 monsoon    (501) staff       (20)     8299 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bs/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.383614 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ca/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11724 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ca/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.384438 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cak/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11480 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cak/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.384598 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ckb/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10564 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ckb/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.384733 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cs/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16308 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cs/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.384989 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cy/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16060 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cy/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.385242 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/da/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15685 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/da/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.385517 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/de/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16228 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/de/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.385768 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/dsb/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16483 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/dsb/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.385939 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/el/
+-rw-r--r--   0 monsoon    (501) staff       (20)    20103 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/el/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.386266 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-CA/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15240 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-CA/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.386776 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-GB/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15236 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-GB/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.387038 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-US/
+-rw-r--r--   0 monsoon    (501) staff       (20)    14945 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-US/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.387341 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eo/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15723 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eo/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.388108 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-AR/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16102 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-AR/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.388407 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-CL/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16276 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-CL/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.388568 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-ES/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16262 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-ES/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.388849 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-MX/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11638 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-MX/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.389097 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/et/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10270 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/et/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.389279 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eu/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16029 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eu/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.389551 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fa/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10211 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fa/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.389798 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ff/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9192 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ff/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.390049 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fi/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15838 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fi/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.390335 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16493 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.390508 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fur/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16217 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fur/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.390824 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fy-NL/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15786 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fy-NL/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.391500 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ga-IE/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7833 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ga-IE/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.391733 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gd/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12039 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gd/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.391967 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gl/
+-rw-r--r--   0 monsoon    (501) staff       (20)    14760 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.392253 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gn/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16393 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gn/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.392563 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gu-IN/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12479 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gu-IN/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.393115 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/he/
+-rw-r--r--   0 monsoon    (501) staff       (20)    17270 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/he/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.393447 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hi-IN/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12614 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hi-IN/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.394142 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10824 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.394392 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hsb/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16491 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hsb/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.394552 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hu/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16193 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hu/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.394775 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hy-AM/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11360 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hy-AM/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.395017 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hye/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12628 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hye/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.395266 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ia/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16129 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ia/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.395565 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/id/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11055 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/id/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.396047 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/is/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15797 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/is/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.396286 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/it/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16107 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/it/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.396555 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ja/
+-rw-r--r--   0 monsoon    (501) staff       (20)    17233 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ja/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.398174 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ka/
+-rw-r--r--   0 monsoon    (501) staff       (20)    21596 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ka/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.399082 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kab/
+-rw-r--r--   0 monsoon    (501) staff       (20)    13066 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kab/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.399261 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kk/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19315 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kk/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.399421 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/km/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11385 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/km/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.400458 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kn/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10661 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kn/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.400645 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ko/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16084 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ko/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.400813 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lij/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9467 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lij/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.401060 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lo/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15113 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lo/viewer.ftl
+-rw-r--r--   0 monsoon    (501) staff       (20)     2498 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/locale.json
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.401241 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lt/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10633 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lt/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.401495 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ltg/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9311 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ltg/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.401759 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lv/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9383 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lv/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.402295 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/meh/
+-rw-r--r--   0 monsoon    (501) staff       (20)     2260 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/meh/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.402527 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mk/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9659 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mk/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.402660 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11774 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.402897 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ms/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9194 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ms/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.403166 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/my/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10184 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/my/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.403973 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nb-NO/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15318 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nb-NO/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.404390 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ne-NP/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12084 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ne-NP/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.404652 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nl/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16046 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.404928 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nn-NO/
+-rw-r--r--   0 monsoon    (501) staff       (20)    13671 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nn-NO/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.405675 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/oc/
+-rw-r--r--   0 monsoon    (501) staff       (20)    13879 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/oc/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.405981 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pa-IN/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19797 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pa-IN/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.406323 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pl/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16341 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.406867 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-BR/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15777 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-BR/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.407143 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-PT/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16189 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-PT/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.407442 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/rm/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16267 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/rm/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.408165 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ro/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9862 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ro/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.408405 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ru/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19808 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ru/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.408567 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sat/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16483 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sat/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.408867 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sc/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11569 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sc/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.409315 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/scn/
+-rw-r--r--   0 monsoon    (501) staff       (20)     1593 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/scn/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.409561 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sco/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9776 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sco/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.409773 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/si/
+-rw-r--r--   0 monsoon    (501) staff       (20)    12008 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/si/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.410019 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sk/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16522 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sk/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.410190 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/skr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    17922 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/skr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.410458 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sl/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15522 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.411025 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/son/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7026 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/son/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.411270 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sq/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15426 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sq/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.411450 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    13848 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.411790 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sv-SE/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15598 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sv-SE/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.412325 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/szl/
+-rw-r--r--   0 monsoon    (501) staff       (20)     9898 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/szl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.412477 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ta/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11748 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ta/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.413484 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/te/
+-rw-r--r--   0 monsoon    (501) staff       (20)    11843 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/te/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.413887 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tg/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19364 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tg/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.414083 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/th/
+-rw-r--r--   0 monsoon    (501) staff       (20)    20722 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/th/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.414835 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tl/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10011 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tl/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.414985 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tr/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15949 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tr/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.415293 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/trs/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7141 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/trs/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.415706 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uk/
+-rw-r--r--   0 monsoon    (501) staff       (20)    19271 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uk/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.416041 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ur/
+-rw-r--r--   0 monsoon    (501) staff       (20)    10357 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ur/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.416451 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uz/
+-rw-r--r--   0 monsoon    (501) staff       (20)     6557 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uz/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.416689 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/vi/
+-rw-r--r--   0 monsoon    (501) staff       (20)    16690 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/vi/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.416993 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/wo/
+-rw-r--r--   0 monsoon    (501) staff       (20)     3505 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/wo/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.417494 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/xh/
+-rw-r--r--   0 monsoon    (501) staff       (20)     7776 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/xh/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.417678 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-CN/
+-rw-r--r--   0 monsoon    (501) staff       (20)    14940 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-CN/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.417952 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-TW/
+-rw-r--r--   0 monsoon    (501) staff       (20)    15113 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-TW/viewer.ftl
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.429494 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/
+-rw-r--r--   0 monsoon    (501) staff       (20)    29513 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitDingbats.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    17597 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixed.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    18055 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBold.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    19151 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBoldItalic.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    18746 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedItalic.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    19469 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerif.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    19395 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBold.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    20733 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBoldItalic.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    21227 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifItalic.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)    16729 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSymbol.pfb
+-rw-r--r--   0 monsoon    (501) staff       (20)     1553 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_FOXIT
+-rw-r--r--   0 monsoon    (501) staff       (20)     4414 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_LIBERATION
+-rw-r--r--   0 monsoon    (501) staff       (20)   137052 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Bold.ttf
+-rw-r--r--   0 monsoon    (501) staff       (20)   135124 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-BoldItalic.ttf
+-rw-r--r--   0 monsoon    (501) staff       (20)   162036 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Italic.ttf
+-rw-r--r--   0 monsoon    (501) staff       (20)   139512 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Regular.ttf
+-rw-r--r--   0 monsoon    (501) staff       (20)   120678 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.css
+-rw-r--r--   0 monsoon    (501) staff       (20)    33051 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.html
+-rw-r--r--   0 monsoon    (501) staff       (20)   645923 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.mjs
+-rw-r--r--   0 monsoon    (501) staff       (20)  1369119 2024-05-06 04:24:45.000000 Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.mjs.map
+-rw-r--r--   0 monsoon    (501) staff       (20)      240 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_server/config.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.434867 Lires-1.8.3/lires_server/handlers/
+-rw-r--r--   0 monsoon    (501) staff       (20)      540 2024-05-12 03:26:10.000000 Lires-1.8.3/lires_server/handlers/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    12365 2024-05-23 06:42:05.000000 Lires-1.8.3/lires_server/handlers/_base.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      770 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_server/handlers/_global_data.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4530 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/apiFiles.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      309 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/auth.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2474 2024-05-22 08:43:36.000000 Lires-1.8.3/lires_server/handlers/dataFeature.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1540 2024-05-12 03:26:10.000000 Lires-1.8.3/lires_server/handlers/dataInfo.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     7176 2024-05-23 02:42:48.000000 Lires-1.8.3/lires_server/handlers/dataMan.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1086 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/databaseInfo.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     6242 2024-05-23 06:44:57.000000 Lires-1.8.3/lires_server/handlers/documents.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2776 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/feed.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2831 2024-05-23 02:47:54.000000 Lires-1.8.3/lires_server/handlers/fileinfo_supp.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1405 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/iServerProxy.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      190 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_server/handlers/info.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5310 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/misc.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5259 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/miscFiles.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      621 2024-05-06 04:16:18.000000 Lires-1.8.3/lires_server/handlers/pdfjs.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4117 2024-05-22 08:36:02.000000 Lires-1.8.3/lires_server/handlers/search.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4009 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/summary.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     6405 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/user.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5422 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/userMan.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2526 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_server/handlers/websocket.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     9123 2024-05-22 08:36:02.000000 Lires-1.8.3/lires_server/main.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      903 2024-05-12 03:26:10.000000 Lires-1.8.3/lires_server/types.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.435645 Lires-1.8.3/lires_service/
+-rw-r--r--   0 monsoon    (501) staff       (20)      240 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.437339 Lires-1.8.3/lires_service/ai/
+-rw-r--r--   0 monsoon    (501) staff       (20)       93 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.437615 Lires-1.8.3/lires_service/ai/cmd/
+-rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/cmd/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1413 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/cmd/summarize.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      801 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/globalConfig.py
+-rw-r--r--   0 monsoon    (501) staff       (20)    11805 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/lmInterface.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     5977 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/lmTools.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     4519 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_service/ai/server.py
+-rw-r--r--   0 monsoon    (501) staff       (20)      131 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/ai/utils.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2513 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_service/entry.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.438105 Lires-1.8.3/lires_service/log/
+-rw-r--r--   0 monsoon    (501) staff       (20)        0 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/log/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     2249 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/log/logger.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     3378 2024-05-15 05:55:43.000000 Lires-1.8.3/lires_service/log/server.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.438621 Lires-1.8.3/lires_service/registry/
+-rw-r--r--   0 monsoon    (501) staff       (20)      213 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/registry/__init__.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1967 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_service/registry/server.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     7010 2024-04-12 02:50:06.000000 Lires-1.8.3/lires_service/registry/store.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.439102 Lires-1.8.3/lires_web/
+-rw-r--r--   0 monsoon    (501) staff       (20)       98 2024-04-19 03:46:55.000000 Lires-1.8.3/lires_web/__init__.py
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.444818 Lires-1.8.3/lires_web/dist/
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.485826 Lires-1.8.3/lires_web/dist/assets/
+-rw-r--r--   0 monsoon    (501) staff       (20)   936012 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/@codemirror-4Zn9bE8B.js
+-rw-r--r--   0 monsoon    (501) staff       (20)   606218 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/@lezer-tqr6QOpM.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2285 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/@vavt-DtLj4T47.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    72194 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/@vue-D_lT-ze_.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3178 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/async-mutex-CSJywVGb.js
+-rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/codemirror-l0sNRNKZ.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2386 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/copy-to-clipboard-B1uT6SkR.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      623 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/crelt-C8TCjufn.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     9206 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/cssfilter-BjxKUPhv.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    32370 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/entities-C20TfXL6.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      297 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/extend-shallow-DA8A8LGH.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    25090 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/fast-xml-parser-CJG3bOwu.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     6319 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/gray-matter-D4hcLa5V.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    47791 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/index-Bzo7HIUU.css
+-rw-r--r--   0 monsoon    (501) staff       (20)   149749 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/index-Tvuvqxrm.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      259 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/is-extendable-CiA4f1iz.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    39551 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/js-yaml-B7yGoGZD.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2307 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/kind-of-l3izQsJJ.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     9137 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/linkify-it-DmNjr4Kv.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    49352 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/markdown-it-DI8MEbma.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2276 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/markdown-it-image-figures-BD49Kf-b.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     1864 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/markdown-it-task-lists-BNI9E7ji.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      529 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/markdown-it-xss-DEpVfk-m.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    89568 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/md-editor-v3-92WZKX8v.css
+-rw-r--r--   0 monsoon    (501) staff       (20)   109482 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/md-editor-v3-CPol1xJ_.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     4884 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/mdurl-k9Sl0PQj.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     9497 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/medium-zoom-bWEtUbjf.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      195 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/node-stdlib-browser-d7cmxmpa.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     3545 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/pinia-BHWH00Pk.js
+-rw-r--r--   0 monsoon    (501) staff       (20)  3766714 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/plotly.js-dist-FakLekxN.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2408 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/punycode.js-Dj65hjkv.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     1259 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/section-matter-DWrNKXO4.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      260 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/strip-bom-string-BxrG9K6S.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     1071 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/strnum-u8jQhLSb.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     2195 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/style-mod-Bc2inJdb.js
+-rw-r--r--   0 monsoon    (501) staff       (20)      423 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/toggle-selection-BHUZwh74.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     5216 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/uc.micro-kMc2yuuw.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    29392 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/vite-plugin-node-polyfills-Cgl3E5jI.js
+-rw-r--r--   0 monsoon    (501) staff       (20)        1 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/vue-l0sNRNKZ.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    23092 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/vue-router-DNoSD41y.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     1494 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/w3c-keyname-Vcq4gwWv.js
+-rw-r--r--   0 monsoon    (501) staff       (20)     8902 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/assets/xss-DnjGkJ2-.js
+-rw-r--r--   0 monsoon    (501) staff       (20)    16446 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/favicon.ico
+-rw-rw-r--   0 monsoon    (501) staff       (20)   324959 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/icon.png
+-rw-r--r--   0 monsoon    (501) staff       (20)     3930 2024-05-21 06:12:41.000000 Lires-1.8.3/lires_web/dist/index.html
+drwxr-xr-x   0 monsoon    (501) staff       (20)        0 2024-05-23 07:04:54.487048 Lires-1.8.3/lires_web/dist/site-icons/
+-rw-r--r--   0 monsoon    (501) staff       (20)     8085 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/site-icons/android-chrome-192x192.png
+-rw-r--r--   0 monsoon    (501) staff       (20)    21747 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/site-icons/android-chrome-512x512.png
+-rw-r--r--   0 monsoon    (501) staff       (20)     8774 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/site-icons/apple-touch-icon.png
+-rw-r--r--   0 monsoon    (501) staff       (20)      832 2024-05-21 06:12:40.000000 Lires-1.8.3/lires_web/dist/site.manifest.json
+-rw-r--r--   0 monsoon    (501) staff       (20)     3996 2024-05-21 10:59:48.000000 Lires-1.8.3/lires_web/generate_icons.py
+-rw-r--r--   0 monsoon    (501) staff       (20)     1829 2024-05-23 06:47:55.000000 Lires-1.8.3/pyproject.toml
+-rw-r--r--   0 monsoon    (501) staff       (20)     1385 2024-05-21 10:59:48.000000 Lires-1.8.3/requirements.py
+-rw-r--r--   0 monsoon    (501) staff       (20)       38 2024-05-23 07:04:54.488397 Lires-1.8.3/setup.cfg
+-rw-r--r--   0 monsoon    (501) staff       (20)     1720 2024-05-22 12:20:01.000000 Lires-1.8.3/setup.py
```

### Comparing `Lires-1.8.2/.DS_Store` & `Lires-1.8.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/LICENSE` & `Lires-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/Makefile` & `Lires-1.8.3/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 DOCKER_IMAGE_NAME = "lires"
 
 test-build:
 	docker build -f docker/test.Dockerfile -t $(DOCKER_IMAGE_NAME):test .
 test-run:
 	docker run --rm -it \
 		-v ./:/Lires \
+		-v /Lires/lires/vector/lib \
 		-v ./test/_cache:/_cache \
 		-e LRS_HOME=/Lires/test/_sandbox \
 		$(DOCKER_IMAGE_NAME):test /usr/local/bin/python3 ./test/main.py
 test-inspect:
 	docker run --rm -it \
 		-v ./:/Lires \
+		-v /Lires/lires/vector/lib \
 		-v ./test/_cache:/_cache \
 		-e LRS_HOME=/Lires/test/_sandbox \
 		$(DOCKER_IMAGE_NAME):test tmux
 test-clean:
 	docker rmi $(DOCKER_IMAGE_NAME):test
```

### Comparing `Lires-1.8.2/README.md` & `Lires-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/ai.py` & `Lires-1.8.3/lires/api/ai.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/common.py` & `Lires-1.8.3/lires/api/common.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/feed.py` & `Lires-1.8.3/lires/api/feed.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/log.py` & `Lires-1.8.3/lires/api/log.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/registry.py` & `Lires-1.8.3/lires/api/registry.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/api/server.py` & `Lires-1.8.3/lires/api/server.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/_update_db.py` & `Lires-1.8.3/lires/cmd/_update_db.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/clear.py` & `Lires-1.8.3/lires/cmd/clear.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/cluster.py` & `Lires-1.8.3/lires/cmd/cluster.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/index.py` & `Lires-1.8.3/lires/cmd/index.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     parser = argparse.ArgumentParser(description="Build search index for the database")
     parser.add_argument("user", action="store", type=str, help="user name")
     subparsers = parser.add_subparsers(dest="subparser", help="sub-command help")
 
     sp_feat = subparsers.add_parser("build", help="build the index")
     sp_feat.add_argument("--force", action="store_true", help="force-rebuild")
     sp_feat.add_argument("--max-words", action="store", type=int, default=2048, help="max words per document used for summarization, more words will be truncated")
-    sp_feat.add_argument("--no-llm-fallback", action="store_true", help="not use LLM as fallback when abstract is not available")
+    # sp_feat.add_argument("--no-llm-fallback", action="store_true", help="not use LLM as fallback when abstract is not available")
 
     sp_query = subparsers.add_parser("query", help="query the index")
     sp_query.add_argument("aim", action="store", type=str, help="query string")
     sp_query.add_argument("--n-return", action="store", type=int, default=16, help="number of documents to return")
     sp_query.add_argument("-ou", "--output-uid", action="store_true", help="print uid instead of human-readable result")
     sp_query.add_argument("-iu", "--input-uid", action="store_true", help="input is uid instead of query string, essentially ask for reading the document with the given uid")
 
@@ -43,44 +43,44 @@
     
     db_ins = await db_pool.get(user)
     db = db_ins.database
 
     iconn = IServerConn()
 
     if args.subparser == "build":
-        vector_db = initVectorDB(db.path.vector_db_file)
+        vector_db = db_ins.vector_db
         await buildFeatureStorage(
-            iconn, db, vector_db, use_llm=not args.no_llm_fallback, force=args.force, max_words_per_doc=args.max_words, 
+            iconn, db, vector_db, force=args.force, max_words_per_doc=args.max_words, 
             )
 
     elif args.subparser == "query":
-        vector_collection = initVectorDB(db.path.vector_db_file).getCollection("doc_feature")
+        vector_collection = await db_ins.vector_db.getCollection("doc_feature")
         if args.input_uid:
-            res = await queryFeatureIndexByUID(
-                db = db, 
-                iconn = iconn,
-                vector_collection = vector_collection,
-                query_uid = args.aim,
-                n_return = args.n_return
-                )
+            raise NotImplementedError
         else:
             res = await queryFeatureIndex(
                 iconn = iconn,
                 vector_collection = vector_collection,
                 query = args.aim,
                 n_return = args.n_return
                 )
         print("-----------------------------------")
         print(f"Query: {args.aim if not args.input_uid else '[' + (await db.get(args.aim)).title + ']'}")
         print("Top results:")
-        for i, (uid, score) in enumerate(zip(res["uids"], res["scores"])):
+        # for i, (uid, score) in enumerate(zip(res["uids"], res["scores"])):
+        #     if args.output_uid:
+        #         print(f"{uid}")
+        #     else:
+        #         print(f"{i+1}: {(await db.get(uid)).title} [score: {score:.4f}]")
+        for i, item in enumerate(res):
+            uid = item["entry"]["uid"]
             if args.output_uid:
                 print(f"{uid}")
             else:
-                print(f"{i+1}: {(await db.get(uid)).title} [score: {score:.4f}]")
+                print(f"{i+1}: {(await db.get(uid)).title} [score: {item['score']:.4f}]")
 
     else:
         ...
     
     await user_pool.close(); await db_pool.close()
 
 def main():
```

### Comparing `Lires-1.8.2/lires/cmd/invite.py` & `Lires-1.8.3/lires/cmd/invite.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/log.py` & `Lires-1.8.3/lires/cmd/log.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/miscUtils.py` & `Lires-1.8.3/lires/cmd/miscUtils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from lires.core.pdfTools import DEFAULT_PDFJS_DOWNLOADING_URL
 
 def main():
     parser = argparse.ArgumentParser("Miscellaneous utilities for lires.")
     sub_parser = parser.add_subparsers(dest = "subparser", help = "task")
 
-    parser_update_pdfjs = sub_parser.add_parser("update_pdfjs", help="update PDF.js distribution")
+    parser_update_pdfjs = sub_parser.add_parser("init-pdfjs", help="update PDF.js distribution")
     parser_update_pdfjs.add_argument("-u", "--url", help = "downloading url", default=DEFAULT_PDFJS_DOWNLOADING_URL)
 
-    parser_edit_config = sub_parser.add_parser("edit_config", help="edit configuration file")
+    parser_edit_config = sub_parser.add_parser("edit-config", help="edit configuration file")
     parser_edit_config.add_argument("-u", "--use_editor", default="", help="choose editor, e.g. . -u vim will invoke 'vim <config>.json'")
 
     args = parser.parse_args()
 
-    if args.subparser == "update_pdfjs":
+    if args.subparser == "init-pdfjs":
         from lires_server.config import PDF_VIEWER_DIR
         from lires.core.pdfTools import downloadDefaultPDFjsViewer
         import asyncio
         asyncio.run(downloadDefaultPDFjsViewer(download_url=args.url, dst_dir=PDF_VIEWER_DIR, force=True))
-    if args.subparser == "edit_config":
+    if args.subparser == "edit-config":
         from lires.config import CONF_FILE_PATH
         from lires.utils import openFile
         import subprocess
         if args.use_editor:
             subprocess.call([args.use_editor, CONF_FILE_PATH])
         else:
             openFile(CONF_FILE_PATH)
```

### Comparing `Lires-1.8.2/lires/cmd/status.py` & `Lires-1.8.3/lires/cmd/status.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/cmd/userManage.py` & `Lires-1.8.3/lires/cmd/userManage.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/config.py` & `Lires-1.8.3/lires/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,27 +50,25 @@
         os.mkdir(_p)
 
 # Set the default configuration here, 
 # will be used for setting default configuration.
 # Also for backward compatibility, 
 # if the old config file exists, and does not contain some new fields,
 # the new fields will be added on top of the old config file on getConf()
-import tiny_vectordb
 import uuid
 import platform
 def __staticConfigToken(prefix = uuid.NAMESPACE_DNS):
     # Create a static token for the configuration file, 
     # based on the $LRS_HOME directory and node id
     return uuid.uuid5(prefix, platform.node() + LRS_HOME).hex
 __default_config: LiresConfT = {
     'group': __staticConfigToken(uuid.NAMESPACE_DNS)[:8],
     'max_users': 1000,
     'default_user_max_storage': '512m',
     'service_port_range': [21000, 22000],
-    'tiny_vectordb_compile_config': tiny_vectordb.autoCompileConfig(),
 }
 __essential_config_keys = []  # keys that must be in the configuration file
 __g_config: Optional[LiresConfT] = None     # buffer
 def getConf() -> LiresConfT:
     global __g_config, CONF_FILE_PATH
     if __g_config is None:
         with open(CONF_FILE_PATH, "r", encoding="utf-8") as conf_file:
@@ -98,15 +96,15 @@
         # check if the essential keys are in the configuration file
         if not all([k in read_conf for k in __essential_config_keys]):
             raise KeyError(f"Essential keys ({__essential_config_keys}) are missing in the configuration file")
         # warn if the configuration file is outdated
         if not compareObject(read_conf, __default_config):
             __logger.warn("Configuration file outdated, "
             "default configuration will be used as fallback, if errors occur, "
-            "please run `lrs-reset` to update the configuration file")
+            "please run `lrs-config reset` to update the configuration file")
 
         # merge the default configuration and the configuration file
         conf: LiresConfT = {**__default_config, **read_conf}   # type: ignore
 
         # eligibility check
         assert len(conf["service_port_range"]) == 2 and \
             conf["service_port_range"][0] < conf["service_port_range"][1], \
```

### Comparing `Lires-1.8.2/lires/core/bibReader.py` & `Lires-1.8.3/lires/core/bibReader.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/dataClass.py` & `Lires-1.8.3/lires/core/dataClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
                 └── ...
         """
         return self.DatabasePath(
             main_dir = self.conn.db_dir,
             file_dir = os.path.join(self.conn.db_dir, "files"),
             index_dir = os.path.join(self.conn.db_dir, "index"),
             summary_dir = os.path.join(self.conn.db_dir, "index", "summary"),
-            vector_db_file = os.path.join(self.conn.db_dir, "index", "vector.db"),
+            vector_db_file = os.path.join(self.conn.db_dir, "index", "vector_v1.db"),
         )
     
     async def dump(self, include_files = False) -> bytes:
         """
         if include files, dump the database to a zip file. 
         else, dump the database to a sqlite file
         """
@@ -225,15 +225,15 @@
                     for root, _, files in os.walk(self.path.file_dir):
                         for f in files:
                             zf.write(os.path.join(root, f), os.path.relpath(os.path.join(root, f), self.path.main_dir))
                 return zip_buffer.getvalue()
     
     async def delete(self, uuid: str) -> bool:
         """ Delete a DataPoint by uuid"""
-        if not self.has(uuid):
+        if not await self.has(uuid):
             await self.logger.error(f"Data not found: {uuid}")
             return False
         await self.logger.info("Deleting {}".format(uuid))
         dp = await self.get(uuid)
         return await dp.fm.deleteEntry(create_backup=False)
     
     # query statistics
```

### Comparing `Lires-1.8.2/lires/core/dataTags.py` & `Lires-1.8.3/lires/core/dataTags.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/dbConn.py` & `Lires-1.8.3/lires/core/dbConn.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,17 @@
             assert ver is not None
             record_version = versionize(ver[0])
 
         if record_version < versionize("1.8.0"):
             await upgrade_1_8_0(self)
             await setVersionRecord("1.8.0")
 
-        await setVersionRecord(curr_version.string())
-        await self.logger.info("Upgraded database {} from version {} to {}".format(self.db_path, record_version, curr_version))
+        if record_version != curr_version:
+            await setVersionRecord(curr_version.string())
+            await self.logger.info("Upgraded database {} from version {} to {}".format(self.db_path, record_version, curr_version))
         DB_MOD_LOCK.release()
         
     async def close(self):
         await self.conn.close()
         await self.cache.conn.close()
     
     async def __aenter__(self):
@@ -452,23 +453,22 @@
         info.device_modify = __THIS_NODE__
         await self.conn.execute("UPDATE files SET info_str=? WHERE uuid=?", (info.toString(), uuid))
         await self.setModifiedFlag(True)
         return True
     
     async def removeEntry(self, uuid: str) -> bool:
         if not (entry:=await self._ensureExist(uuid)): return False
-        await self.logger.debug("(db_conn) Removing entry {}".format(uuid))
         await self.conn.execute("DELETE FROM files WHERE uuid=?", (uuid,))
 
         # remove related cache
         await self.cache.removeTagCache(uuid, entry["tags"])
         await self.cache.removeAuthorCache(uuid, entry["authors"])
 
         await self.setModifiedFlag(True)
-        await self.logger.debug("Removed entry {}".format(uuid))
+        await self.logger.debug("(db_conn) Removed entry {}".format(uuid))
         return True
     
     async def setDocExt(self, uuid: str, ext: Optional[str]) -> bool:
         if not await self._ensureExist(uuid): return False
         await self.logger.debug("(db_conn) Setting doc_ext for {} to {}".format(uuid, ext))
         await self.conn.execute("UPDATE files SET doc_ext=? WHERE uuid=?", (ext, uuid))
         await self._touchEntry(uuid)
@@ -698,15 +698,15 @@
                     tag TEXT PRIMARY KEY,
                     entries TEXT NOT NULL
                 )
                 """)
         return self
 
     async def buildInitCache(self, all_items: list[DBFileInfo]):
-        await self.logger.info("[DBCache] Building initial cache")
+        await self.logger.debug("[DBCache] Building initial cache")
         # build cache for authors and tags
         authors_cache: dict[str, list[str]] = {}
         tags_cache: dict[str, list[str]] = {}
         for item in all_items:
             for author in item["authors"]:
                 # format author name!
                 author = formatAuthorName(author)
```

### Comparing `Lires-1.8.2/lires/core/dbConnUpgrade.py` & `Lires-1.8.3/lires/core/dbConnUpgrade.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/dbConn_.py` & `Lires-1.8.3/lires/core/dbConn_.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/error.py` & `Lires-1.8.3/lires/core/error.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/fileTools.py` & `Lires-1.8.3/lires/core/fileTools.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/logger.py` & `Lires-1.8.3/lires/core/logger.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/pdfTools.py` & `Lires-1.8.3/lires/core/pdfTools.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/refparser/endnote.py` & `Lires-1.8.3/lires/core/refparser/endnote.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/core/refparser/interface.py` & `Lires-1.8.3/lires/core/refparser/interface.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/exec.py` & `Lires-1.8.3/lires/exec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os, asyncio
 from .parser import prepareParser
-from .cmd.generateDefaultConf import generateDefaultConf
+from .config import generateDefaultConf
 
 def initLoggers():
     # May move to other place...
     import os
     from lires.utils import setupLogger, BCOLORS
     from lires.utils.log import TermLogLevelT
 
@@ -28,18 +28,14 @@
     initLoggers()
 
     NOT_RUN = False     # Indicates whether to run main program
 
     if not os.path.exists(CONF_FILE_PATH):
         generateDefaultConf()
 
-    if args.reset_conf:
-        generateDefaultConf()
-        NOT_RUN = True
-
     if args.version:
         for v,change_list in VERSION_HISTORIES:
             change_strings = []
             for change in change_list:
                 if isinstance(change, str):
                     change_strings.append(change)
                 elif isinstance(change, dict):
```

### Comparing `Lires-1.8.2/lires/loader.py` & `Lires-1.8.3/lires/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import os, dataclasses, shutil
 from .core.base import LiresBase
 from .core.dataClass import DataBase
 from .core.vector import initVectorDB
 from .config import DATABASE_HOME, USER_DIR
 from .user import UserPool, LiresUser
 
-from tiny_vectordb import VectorDatabase
+from lires.vector.database import VectorDatabase
 import asyncio
 
 @dataclasses.dataclass(frozen=True)
 class DatabaseInstance:
     database: DataBase
     vector_db: VectorDatabase
     async def close(self):
         await self.database.close()
-        self.vector_db.disk_io.conn.close()
+        await self.vector_db.close()
     
     async def commit(self):
         await self.database.commit()
-        self.vector_db.commit()
+        await self.vector_db.commit()
 
 async def loadDatabaseInstance(user_id: int, database_home: str):
     database_dir = os.path.join(database_home, str(user_id))
     db = await DataBase().init(database_dir)
-    vec_db = initVectorDB(db.path.vector_db_file)
+    vec_db = await initVectorDB(db.path.vector_db_file)
     return DatabaseInstance(db, vec_db)
 
 class DatabasePool(LiresBase):
     def __init__(self, databse_home: str = DATABASE_HOME) -> None:
         super().__init__()
         self._home = databse_home
```

### Comparing `Lires-1.8.2/lires/parser.py` & `Lires-1.8.3/lires/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 def prepareParser() -> argparse.ArgumentParser:
     _description = f"\
 Lires, a self-hosted research literature manager. \
 For more info and source code, visit: https://github.com/MenxLi/Lires\
     "
     parser = argparse.ArgumentParser(description=_description)
     parser.add_argument("-v", "--version", action = "store_true", help = "Show version histories and current version and exit")
-    parser.add_argument("-H", "--show_home", action= "store_true", help = "Print LRS_HOME and exit")
-    parser.add_argument("--reset_conf", action = "store_true", help = "Reset configuration and exit")
+    parser.add_argument("-H", "--show-home", action= "store_true", help = "Print LRS_HOME and exit")
 
     sp = parser.add_subparsers(dest = "subparser", help = "Sub-commands")
 
     parser_registry = sp.add_parser("registry", help = "Start lires registry server")
     _prepareRegistryServerParser(parser_registry)
 
     parser_server = sp.add_parser("server", help = "Start lires main server")
```

### Comparing `Lires-1.8.2/lires/types/configT.py` & `Lires-1.8.3/lires/types/configT.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 from typing import TypedDict, TYPE_CHECKING
 
-if TYPE_CHECKING:
-    from tiny_vectordb.wrap import CompileConfig as TinyVectordbCompileConfig
-
 class LiresConfT(TypedDict):
     """
-    Refer to lrs-reset
+    Refer to lrs-config
     for the generation of default configuration file,
 
     changes in v1.1.2:
         - Almost all fields are moved as static fields of lires.config, May add some fields in the future.
     
     changes in v1.7.5:
         - Add deploy_token field for server communication
         - Change database_id to group
     
     changes in v1.8.0:
         - Remove deploy_token field
     
     changes in v1.8.2:
         - Add max_users and default_user_max_storage fields
+    
+    changes in v1.8.3:
+        - drop tiny_vectordb dependency
     """
     ## Should contain no optional or ambiguous type fields!!
 
     # An unique id for the LRS_HOME directory,
     # used for identifying different LRS_HOME directories
     group: str
 
@@ -37,11 +37,8 @@
     # set to 0 for unlimited users
     max_users: int
 
     # The maximum storage for each user
     # e.g 512m, 1g, 1t
     default_user_max_storage: str
 
-    # jit compile configuration for tiny_vectordb
-    tiny_vectordb_compile_config: TinyVectordbCompileConfig
-
 __all__ = ["LiresConfT"]
```

### Comparing `Lires-1.8.2/lires/types/dataT.py` & `Lires-1.8.3/lires/types/dataT.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/user/conn.py` & `Lires-1.8.3/lires/user/conn.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/user/loader.py` & `Lires-1.8.3/lires/user/loader.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/user/object.py` & `Lires-1.8.3/lires/user/object.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/__init__.py` & `Lires-1.8.3/lires/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/author.py` & `Lires-1.8.3/lires/utils/author.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/compressTools.py` & `Lires-1.8.3/lires/utils/compressTools.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/fs.py` & `Lires-1.8.3/lires/utils/fs.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/log.py` & `Lires-1.8.3/lires/utils/log.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/network.py` & `Lires-1.8.3/lires/utils/network.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/random.py` & `Lires-1.8.3/lires/utils/random.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/term.py` & `Lires-1.8.3/lires/utils/term.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/utils/time.py` & `Lires-1.8.3/lires/utils/time.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/version.py` & `Lires-1.8.3/lires/version.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires/version.yaml` & `Lires-1.8.3/lires/version.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -891,7 +891,16 @@
       - Set default user storage via configuration
     - Documentations:
       - Update documentation structure
     - Fix: 
       - Internal service cache name collision
     - Other changes:
       - Send feed without ai server connection
+  1.8.3:
+    - Features:
+      - Instant vector index update
+      - Not reload page submit registeration
+      - Web app icon for mobile
+    - Refactor:
+      - Use internal vector database
+    - Management:
+      - New tool - `lrs-config`
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/404.html` & `Lires-1.8.3/lires_server/assets/docs/404.html`

 * *Files 0% similar despite different names*

```diff
@@ -11,11 +11,11 @@
     <script type="module" src="/documentation/assets/app.CngJ_OZF.js"></script>
     <link rel="preload" href="/documentation/assets/inter-roman-latin.Di8DUHzh.woff2" as="font" type="font/woff2" crossorigin="">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink active" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav empty fixed" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><!----><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><!----><div class="VPContent" id="VPContent" data-v-5d98c3a5 data-v-1428d186><!--[--><div class="NotFound" data-v-1428d186 data-v-4f08a194><p class="code" data-v-4f08a194>404</p><h1 class="title" data-v-4f08a194>PAGE NOT FOUND</h1><div class="divider" data-v-4f08a194></div><blockquote class="quote" data-v-4f08a194>But if you don&#39;t change your direction, and if you keep looking, you may end up where you are heading.</blockquote><div class="action" data-v-4f08a194><a class="link" href="/documentation/" aria-label="go to home" data-v-4f08a194>Take me home</a></div></div><!--]--></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/app.CngJ_OZF.js` & `Lires-1.8.3/lires_server/assets/docs/assets/app.CngJ_OZF.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/chunks/framework.CZXUNLJW.js` & `Lires-1.8.3/lires_server/assets/docs/assets/chunks/framework.CZXUNLJW.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/chunks/theme.CfuCmiaJ.js` & `Lires-1.8.3/lires_server/assets/docs/assets/chunks/theme.CfuCmiaJ.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_docker.md.qRcDU1HX.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_enviromentVariables.md.C9ixW2VB.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_enviromentVariables.md.Bts03XC7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 import {
     _ as t,
     c as e,
     o as d,
     a2 as o
 } from "./chunks/framework.CZXUNLJW.js";
-const m = JSON.parse('{"title":"Enviroment variales","description":"","frontmatter":{},"headers":[],"relativePath":"deployment/enviromentVariables.md","filePath":"deployment/enviromentVariables.md","lastUpdated":1716199320000}'),
+const m = JSON.parse('{"title":"Enviroment variales","description":"","frontmatter":{},"headers":[],"relativePath":"deployment/enviromentVariables.md","filePath":"deployment/enviromentVariables.md","lastUpdated":1716270324000}'),
     r = {
         name: "deployment/enviromentVariables.md"
     },
-    a = o('<h1 id="enviroment-variales" tabindex="-1">Enviroment variales <a class="header-anchor" href="#enviroment-variales" aria-label="Permalink to &quot;Enviroment variales&quot;">​</a></h1><p>There are various enviroment variables that can control the behavior of the servers, listed here:</p><p><strong>Common variables</strong> Applies to all servers.</p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_HOME</code></td><td>The path to the directory where <code>Lires</code> stores its data.</td><td><code>~/.Lires</code></td></tr><tr><td><code>LRS_KEY</code></td><td>The secret key for inter-service communication.</td><td></td></tr><tr><td><code>LRS_TERM_LOG_LEVEL</code></td><td>The terminal logging level.</td><td><code>INFO</code></td></tr><tr><td><code>LRS_LOG_LEVEL</code></td><td>The logging level send to the log server.</td><td><code>DEBUG</code></td></tr></tbody></table><p><strong><code>lires server</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_SSL_KEYFILE</code></td><td>The path to the SSL key file. (must be used with <code>LRS_SSL_CERTFILE</code>)</td><td></td></tr><tr><td><code>LRS_SSL_CERTFILE</code></td><td>The path to the SSL certificate file.</td><td></td></tr><tr><td><code>LRS_DEV</code></td><td>Set to <code>1</code> to enable server auto-reload on file change</td><td><code>0</code></td></tr><tr><td><code>TVDB_CACHE_DIR</code></td><td>The path to the <code>tiny_vectordb</code> cache directory.</td><td></td></tr><tr><td><code>TVDB_BACKEND</code></td><td>The <code>tiny_vectordb</code> backend to use, can be set to <code>numpy</code> if error occurs.</td><td><code>cxx</code></td></tr></tbody></table><p><strong><code>lires ai</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>HF_HOME</code></td><td>The path to the Hugging Face home directory.</td><td><code>~/.cache/huggingface</code></td></tr><tr><td><code>HF_ENDPONT</code></td><td>The Hugging Face API endpoint.</td><td><code>&quot;https://huggingface.co&quot;</code></td></tr><tr><td><code>OPENAI_API_BASE</code></td><td>The OpenAI API base URL.</td><td><code>&quot;https://api.openai.com/v1</code></td></tr><tr><td><code>OPENAI_API_KEY</code></td><td>The OpenAI API key.</td><td></td></tr></tbody></table><p><strong>Lires-web build variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>VITE_MAINTAINER_NAME</code></td><td>The name of the maintainer.</td><td></td></tr><tr><td><code>VITE_MAINTAINER_EMAIL</code></td><td>The email of the maintainer.</td><td></td></tr></tbody></table>', 10),
+    a = o('<h1 id="enviroment-variales" tabindex="-1">Enviroment variales <a class="header-anchor" href="#enviroment-variales" aria-label="Permalink to &quot;Enviroment variales&quot;">​</a></h1><p>There are various enviroment variables that can control the behavior of the servers, listed here:</p><p><strong>Common variables</strong> Applies to all servers.</p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_HOME</code></td><td>The path to the directory where <code>Lires</code> stores its data.</td><td><code>~/.Lires</code></td></tr><tr><td><code>LRS_KEY</code></td><td>The secret key for inter-service communication.</td><td></td></tr><tr><td><code>LRS_TERM_LOG_LEVEL</code></td><td>The terminal logging level.</td><td><code>INFO</code></td></tr><tr><td><code>LRS_LOG_LEVEL</code></td><td>The logging level send to the log server.</td><td><code>DEBUG</code></td></tr></tbody></table><p><strong><code>lires server</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_SSL_KEYFILE</code></td><td>The path to the SSL key file. (must be used with <code>LRS_SSL_CERTFILE</code>)</td><td></td></tr><tr><td><code>LRS_SSL_CERTFILE</code></td><td>The path to the SSL certificate file.</td><td></td></tr><tr><td><code>LRS_DEV</code></td><td>Set to <code>1</code> to enable server auto-reload on file change.</td><td><code>0</code></td></tr><tr><td><code>TVDB_CACHE_DIR</code></td><td>The path to the <code>tiny_vectordb</code> cache directory.</td><td></td></tr><tr><td><code>TVDB_BACKEND</code></td><td>The <code>tiny_vectordb</code> backend to use, can be set to <code>numpy</code> if error occurs.</td><td><code>cxx</code></td></tr></tbody></table><p><strong><code>lires ai</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>HF_HOME</code></td><td>The path to the Hugging Face home directory.</td><td><code>~/.cache/huggingface</code></td></tr><tr><td><code>HF_ENDPONT</code></td><td>The Hugging Face API endpoint.</td><td><code>&quot;https://huggingface.co&quot;</code></td></tr><tr><td><code>OPENAI_API_BASE</code></td><td>The OpenAI API base URL.</td><td><code>&quot;https://api.openai.com/v1</code></td></tr><tr><td><code>OPENAI_API_KEY</code></td><td>The OpenAI API key.</td><td></td></tr></tbody></table><p><strong>Lires-web build variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>VITE_MAINTAINER_NAME</code></td><td>The name of the maintainer.</td><td></td></tr><tr><td><code>VITE_MAINTAINER_EMAIL</code></td><td>The email of the maintainer.</td><td></td></tr></tbody></table>', 10),
     c = [a];
 
 function i(n, h, s, l, _, p) {
     return d(), e("div", null, c)
 }
 const v = t(r, [
     ["render", i]
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_gettingStarted.md.DpAQEIqk.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_gettingStarted.md.CAqJg6m3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,29 @@
 import {
     _ as s,
     c as a,
     o as e,
     a2 as i
 } from "./chunks/framework.CZXUNLJW.js";
-const g = JSON.parse('{"title":"Getting Started","description":"","frontmatter":{},"headers":[],"relativePath":"deployment/gettingStarted.md","filePath":"deployment/gettingStarted.md","lastUpdated":1716128692000}'),
+const g = JSON.parse('{"title":"Getting Started","description":"","frontmatter":{},"headers":[],"relativePath":"deployment/gettingStarted.md","filePath":"deployment/gettingStarted.md","lastUpdated":1716270324000}'),
     t = {
         name: "deployment/gettingStarted.md"
     },
     n = i(`<h1 id="getting-started" tabindex="-1">Getting Started <a class="header-anchor" href="#getting-started" aria-label="Permalink to &quot;Getting Started&quot;">​</a></h1><p>This guide will help you to install and start the Lires server.<br> For using it with Docker, please refer to <a href="./docker.html">Docker Deployment</a>.</p><h2 id="table-of-contents" tabindex="-1">Table of Contents <a class="header-anchor" href="#table-of-contents" aria-label="Permalink to &quot;Table of Contents&quot;">​</a></h2><nav class="table-of-contents"><ul><li><a href="#table-of-contents">Table of Contents</a></li><li><a href="#installation">Installation</a><ul><li><a href="#from-pypi">From PyPI</a></li><li><a href="#from-source">From source</a></li></ul></li><li><a href="#server-startup">Server startup</a><ul><li><a href="#manual-startup">Manual startup</a></li><li><a href="#cluster-startup">Cluster startup</a></li><li><a href="#create-the-first-user">Create the first user</a></li></ul></li><li><a href="#management">Management</a></li></ul></nav><h2 id="installation" tabindex="-1">Installation <a class="header-anchor" href="#installation" aria-label="Permalink to &quot;Installation&quot;">​</a></h2><h3 id="from-pypi" tabindex="-1">From PyPI <a class="header-anchor" href="#from-pypi" aria-label="Permalink to &quot;From PyPI&quot;">​</a></h3><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">pip</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> install</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> &#39;Lires[all]&#39;</span></span></code></pre></div><h3 id="from-source" tabindex="-1">From source <a class="header-anchor" href="#from-source" aria-label="Permalink to &quot;From source&quot;">​</a></h3><ol><li>Compile frontend files</li></ol><blockquote><p><strong>Prerequisites:</strong> Node.js, Make</p></blockquote><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">make</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> build</span></span></code></pre></div><ol start="2"><li>Install the servers</li></ol><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">pip</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> install</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> &quot;.[all]&quot;</span></span></code></pre></div><h2 id="server-startup" tabindex="-1">Server startup <a class="header-anchor" href="#server-startup" aria-label="Permalink to &quot;Server startup&quot;">​</a></h2><h3 id="manual-startup" tabindex="-1">Manual startup <a class="header-anchor" href="#manual-startup" aria-label="Permalink to &quot;Manual startup&quot;">​</a></h3><p>Start the microservices with the following commands:</p><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> registry</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">  # the global resource module, for service discovery</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> log</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # the log service</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> ai</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">        # the AI service</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> feed</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">      # the feed service</span></span></code></pre></div><p>Lires services are designed to be scalable, and can be started with multiple instances (except for the registry service).</p><div class="info custom-block"><p class="custom-block-title">INFO</p><p>The <code>registry</code> service is for service discovery, and should be started before other services.</p></div><p>Then, start the gateway server:</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> server</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">    # the gateway server</span></span></code></pre></div><p>Lires server is a tornado server that provides API for the client (WebUI &amp; CLI) to communicate with, and should be exposed to the internet.</p><details class="details custom-block"><summary>Details</summary><h4 id="more-on-starting-the-servers" tabindex="-1">More on starting the servers <a class="header-anchor" href="#more-on-starting-the-servers" aria-label="Permalink to &quot;More on starting the servers&quot;">​</a></h4><p><code>$LRS_HOME</code> directory is used for application data storage, by default it is set to <code>~/.Lires</code>.<br> The data directory contains the configuration file, log files, database, cache files...</p><p>To start the application with arbitrary data directory, you can run:</p><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">LRS_HOME</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">=</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">&quot;your/path/here&quot;</span><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;"> lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> ...</span></span></code></pre></div><p>Additionally, various environment variables can be set to customize the behavior of the application. A detailed list of environment variables can be found at <strong><a href="./enviromentVariables.html">here</a></strong>.</p></details><hr><h3 id="cluster-startup" tabindex="-1">Cluster startup <a class="header-anchor" href="#cluster-startup" aria-label="Permalink to &quot;Cluster startup&quot;">​</a></h3><p>It will be laborious and error-prone to start multiple servers manually.<br> Especially when we want to start multiple servers with different configurations.</p><p>Instead, we provide a simple script to enable server clustering for easy deployment.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># Generate a template configuration file</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-cluster</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">your/configuration.yam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">l</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --generate</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># Edit the configuration file</span></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># ...</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># Start the cluster</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-cluster</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">your/configuration.yam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">l</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span></span></code></pre></div><p>The configuration file designates the environment variables, as well as the command line arguments for each server.</p><hr><h3 id="create-the-first-user" tabindex="-1">Create the first user <a class="header-anchor" href="#create-the-first-user" aria-label="Permalink to &quot;Create the first user&quot;">​</a></h3><p><strong>On the first run</strong> you need to create a user account, which can be done by running the <code>lrs-user</code> command in the container.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># export LRS_HOME=&quot;...&quot;</span></span>
-<span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> add</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --admin</span></span></code></pre></div><p>After the user is created, you can manage other users with this user via the web interface.<br> For more information, see <a href="./manage.html#user-management">User management</a>.</p><h2 id="management" tabindex="-1">Management <a class="header-anchor" href="#management" aria-label="Permalink to &quot;Management&quot;">​</a></h2><p>There are several management tools for the server, they are all accessible by <code>lrs-&lt;tool_name&gt;</code>.<br> A list of all the tools and common tasks can be found in <a href="./manage.html">manage.md</a>.</p>`, 36),
+<span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> add</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --admin</span></span></code></pre></div><p>For more information, see <a href="./manage.html#user-management">User management</a>.</p><h2 id="management" tabindex="-1">Management <a class="header-anchor" href="#management" aria-label="Permalink to &quot;Management&quot;">​</a></h2><p>There are several management tools for the server, they are all accessible by <code>lrs-&lt;tool_name&gt;</code>.<br> A list of all the tools and common tasks can be found in <a href="./manage.html">manage.md</a>.</p>`, 36),
     l = [n];
 
 function r(h, o, p, d, c, k) {
     return e(), a("div", null, l)
 }
 const m = s(t, [
     ["render", r]
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.lean.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_index.md.CoeEU7dC.lean.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_manage.md.BIu_1sX3.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.js` & `Lires-1.8.3/lires_server/assets/docs/assets/deployment_obsidianPlugin.md.nIZEfUDA.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.js` & `Lires-1.8.3/lires_server/assets/docs/assets/dev_index.md.BWyXioCS.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.js` & `Lires-1.8.3/lires_server/assets/docs/assets/dev_roadmap.md.JuQ1QPZz.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/index.md.DPNZS3UP.js` & `Lires-1.8.3/lires_server/assets/docs/assets/index.md.DPNZS3UP.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/index.md.DPNZS3UP.lean.js` & `Lires-1.8.3/lires_server/assets/docs/assets/index.md.DPNZS3UP.lean.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-cyrillic-ext.r48I6akx.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-cyrillic-ext.r48I6akx.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-cyrillic.By2_1cv3.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-cyrillic.By2_1cv3.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-greek-ext.1u6EdAuj.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-greek-ext.1u6EdAuj.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-greek.DJ8dCoTZ.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-greek.DJ8dCoTZ.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-latin-ext.CN1xVJS-.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-latin-ext.CN1xVJS-.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-latin.C2AdPX0b.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-latin.C2AdPX0b.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-italic-vietnamese.BSbpV94h.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-italic-vietnamese.BSbpV94h.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-cyrillic-ext.BBPuwvHQ.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-cyrillic-ext.BBPuwvHQ.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-cyrillic.C5lxZ8CY.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-cyrillic.C5lxZ8CY.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-greek-ext.CqjqNYQ-.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-greek-ext.CqjqNYQ-.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-greek.BBVDIX6e.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-greek.BBVDIX6e.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-latin-ext.4ZJIpNVo.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-latin-ext.4ZJIpNVo.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-latin.Di8DUHzh.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-latin.Di8DUHzh.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/inter-roman-vietnamese.BjW4sHH5.woff2` & `Lires-1.8.3/lires_server/assets/docs/assets/inter-roman-vietnamese.BjW4sHH5.woff2`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_add-document.md.DrcA27xh.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_add-edit-entry.md.DrmD-fBC.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_api.md.D91ytbUt.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_filter-entry.md.BYNwwSc_.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.lean.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_index.md.Bw2M76Cg.lean.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_obsidianPlugin.md.D4E6RQm8.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_read.md.DFrZ1-Iq.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/manual_user-interface.md.pJkOzfoZ.js` & `Lires-1.8.3/lires_server/assets/docs/assets/manual_user-interface.md.CdSRMwMo.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 import {
     _ as a,
     c as e,
     o as i,
     a2 as l
 } from "./chunks/framework.CZXUNLJW.js";
-const _ = JSON.parse('{"title":"界面元素","description":"","frontmatter":{},"headers":[],"relativePath":"manual/user-interface.md","filePath":"manual/user-interface.md","lastUpdated":1711621108000}'),
+const _ = JSON.parse('{"title":"界面元素","description":"","frontmatter":{},"headers":[],"relativePath":"manual/user-interface.md","filePath":"manual/user-interface.md","lastUpdated":1716270324000}'),
     s = {
         name: "manual/user-interface.md"
     },
-    t = l('<h1 id="界面元素" tabindex="-1">界面元素 <a class="header-anchor" href="#界面元素" aria-label="Permalink to &quot;界面元素&quot;">​</a></h1><p>本页面介绍软件的用户界面元素，供读者参考，以便于阅读后续使用说明。</p><p>目前本软件主要实现了以下界面：</p><ul><li>登录页面</li><li>主页面</li><li>阅读器</li><li>推送页面</li><li>关于页面</li></ul><p>可通过点击导航栏中的链接，或界面中的相应按钮，进入相应页面。<br> 以下是各个页面的界面元素介绍。</p><h2 id="工具栏" tabindex="-1">工具栏 <a class="header-anchor" href="#工具栏" aria-label="Permalink to &quot;工具栏&quot;">​</a></h2><p>工具栏是所有页面中的通用元素， 在工具栏左侧包含设置和返回/退出登陆按钮， 右侧是页面导航。 例如，下图是主界面中的工具栏：</p><p><img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-toolbar-dark-v1.7.3.png" alt="lires-toolbar"></p><h2 id="数据卡片" tabindex="-1">数据卡片 <a class="header-anchor" href="#数据卡片" aria-label="Permalink to &quot;数据卡片&quot;">​</a></h2><p>数据卡片（Data Card）是Lires的数据条目展示形式，是主页中的数据内容，也是其他页面中的可编辑数据展示形式。 以下为一张数据卡片： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacard-dark-v1.3.0.png" alt="lires-datacard"></p><p>数据卡片包含了文献标题和作者的基本信息以及操作按钮：</p><ul><li>阅读器（Reader）：点击<code>Reader</code>按钮，可以打开该阅读器对文献信息阅读，同时记录笔记。</li><li>链接（Link）：点击<code>Link</code>按钮，可以在新窗口打开文献链接，当文献没有URL字段时不显示。</li><li>概览（Summary）：点击<code>Summary</code>按钮，可以显示文献的详细信息，尝试使用AI进行总结。</li><li>引用（Cite）：点击<code>Cite</code>按钮，可以显示数种引用格式，点击即可复制。</li><li>操作（Actions）：点击<code>Actions</code>按钮，可以展开操作菜单，包含了编辑条目信息、添加和删除文档、 以及删除条目等操作。</li></ul><p>通过点击<code>Actions</code>和<code>Abstract</code>按钮，可将数据卡片完全展开如下： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardExpand-dark-v1.3.0.png" alt="lires-datacardExpand"></p><p>摘要（Abstract）处用于填入文献的摘要信息，点击摘要正文部分即可进行编辑，当编辑完成后自动保存。</p><p>概览（Summary）界面中展示了包括全部作者、期刊、数据大小等详细信息，尝试使用AI进行自动总结， 并基于语义搜索展示文献库中所有最相关文献。下图是概览界面的展示： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardSummary-dark-v1.3.0.png" alt="lires-datacardSummary"></p><p>若文献库中有同名作者，会在作者名后面标注数字，点击数字即可展开作者的其他条目数据卡片。</p><hr><div class="info custom-block"><p class="custom-block-title">INFO</p><p>待完善</p></div>', 18),
+    t = l('<h1 id="界面元素" tabindex="-1">界面元素 <a class="header-anchor" href="#界面元素" aria-label="Permalink to &quot;界面元素&quot;">​</a></h1><p>本页面简要介绍软件的用户界面元素，供读者参考。<br> 可在此页面查找后续文档所提及界面元素的含义。</p><p>目前本软件主要实现了以下页面：</p><ul><li>登录页面</li><li>主页面</li><li>阅读器</li><li>推送页面</li><li>关于页面</li></ul><p>可通过点击导航栏中的链接，或界面中的相应按钮，进入相应页面。<br> 以下是关键界面元素介绍。</p><h2 id="工具栏" tabindex="-1">工具栏 <a class="header-anchor" href="#工具栏" aria-label="Permalink to &quot;工具栏&quot;">​</a></h2><p>工具栏是所有页面中的通用元素， 在工具栏左侧包含设置和返回/退出登陆按钮， 右侧是页面导航。 例如，下图是主界面中的工具栏：</p><p><img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-toolbar-dark-v1.7.3.png" alt="lires-toolbar"></p><h2 id="数据卡片" tabindex="-1">数据卡片 <a class="header-anchor" href="#数据卡片" aria-label="Permalink to &quot;数据卡片&quot;">​</a></h2><p>数据卡片（Data Card）是Lires的数据条目展示形式，是主页中的数据内容，也是其他页面中的可编辑数据展示形式。 以下为一张数据卡片： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacard-dark-v1.3.0.png" alt="lires-datacard"></p><p>数据卡片包含了文献标题和作者的基本信息以及操作按钮：</p><ul><li>阅读器（Reader）：点击<code>Reader</code>按钮，可以打开该阅读器对文献信息阅读，同时记录笔记。</li><li>链接（Link）：点击<code>Link</code>按钮，可以在新窗口打开文献链接，当文献没有URL字段时不显示。</li><li>概览（Summary）：点击<code>Summary</code>按钮，可以显示文献的详细信息，尝试使用AI进行总结。</li><li>引用（Cite）：点击<code>Cite</code>按钮，可以显示数种引用格式，点击即可复制。</li><li>操作（Actions）：点击<code>Actions</code>按钮，可以展开操作菜单，包含了编辑条目信息、添加和删除文档、 以及删除条目等操作。</li></ul><p>通过点击<code>Actions</code>和<code>Abstract</code>按钮，可将数据卡片完全展开如下： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardExpand-dark-v1.3.0.png" alt="lires-datacardExpand"></p><p>摘要（Abstract）处用于填入文献的摘要信息，点击摘要正文部分即可进行编辑，当编辑完成后自动保存。</p><p>概览（Summary）界面中展示了包括全部作者、期刊、数据大小等详细信息，尝试使用AI进行自动总结， 并基于语义搜索展示文献库中所有最相关文献。下图是概览界面的展示： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardSummary-dark-v1.3.0.png" alt="lires-datacardSummary"></p><p>若文献库中有同名作者，会在作者名后面标注数字，点击数字即可展开作者的其他条目数据卡片。</p><hr><div class="info custom-block"><p class="custom-block-title">INFO</p><p>待完善</p></div>', 18),
     r = [t];
 
 function c(n, o, d, p, m, u) {
     return i(), e("div", null, r)
 }
 const b = a(s, [
     ["render", c]
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/assets/style.CT5GXN_K.css` & `Lires-1.8.3/lires_server/assets/docs/assets/style.CT5GXN_K.css`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/docker.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/docker.html`

 * *Files 1% similar despite different names*

```diff
@@ -29,11 +29,11 @@
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># or check output by docker logs</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">docker</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> logs</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -f</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> lrs</span></span></code></pre></div><h2 id="change-the-configuration" tabindex="-1">Change the configuration <a class="header-anchor" href="#change-the-configuration" aria-label="Permalink to &quot;Change the configuration&quot;">​</a></h2><p>The docker image essentially runs the <a href="./gettingStarted.html#cluster-startup"><code>lrs-cluster</code></a> command with the configuration file <code>/root/.Lires/container-cluster.yaml</code>. Which should be mounted to the host machine for easy access and modification.</p><div class="info custom-block"><p class="custom-block-title">INFO</p><p>Although you may change the <a href="./enviromentVariables.html">environment variables</a> with <code>docker run -e ...</code>, it is recommended to modify them in the cluster configuration file, to make sure it will not be overwritten by the values set with the configuration file.</p></div><h2 id="limit-the-resources" tabindex="-1">Limit the resources <a class="header-anchor" href="#limit-the-resources" aria-label="Permalink to &quot;Limit the resources&quot;">​</a></h2><p>An advantage of running the app with docker is that you can limit the resources of the container.</p><p>To limit the memory and cpu usage, you can use the <code>--memory</code> and <code>--cpus</code> flags.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">docker</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> run</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --memory</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> 4g</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --cpus</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> 2</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> ...</span></span></code></pre></div><p>To limit the disk usage, you can use the docker volume driver, for example, first create a volume with limited size, then mount it to the container.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># create a volume with 10G size</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">docker</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> volume</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> create</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --driver</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> local</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --opt</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> type=btrfs</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --opt</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> o=size=10G</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> lrs-data</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># run the container with the volume</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">docker</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> run</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -v</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> lrs-data:/root/.Lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> ...</span></span></code></pre></div><p>For more information, see <a href="https://docs.docker.com/reference/cli/docker/volume/create/#driver-specific-options" target="_blank" rel="noreferrer">docker - driver specific options</a>.</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-19T14:24:52.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/gettingStarted.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Getting Started</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/manage.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Management</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/enviromentVariables.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/enviromentVariables.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     <meta name="generator" content="VitePress v1.1.4">
     <link rel="preload stylesheet" href="/documentation/assets/style.CT5GXN_K.css" as="style">
     
     <script type="module" src="/documentation/assets/app.CngJ_OZF.js"></script>
     <link rel="preload" href="/documentation/assets/inter-roman-latin.Di8DUHzh.woff2" as="font" type="font/woff2" crossorigin="">
     <link rel="modulepreload" href="/documentation/assets/chunks/theme.CfuCmiaJ.js">
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
-    <link rel="modulepreload" href="/documentation/assets/deployment_enviromentVariables.md.C9ixW2VB.lean.js">
+    <link rel="modulepreload" href="/documentation/assets/deployment_enviromentVariables.md.Bts03XC7.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
-    <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_deployment_enviromentVariables" data-v-39a288b8><div><h1 id="enviroment-variales" tabindex="-1">Enviroment variales <a class="header-anchor" href="#enviroment-variales" aria-label="Permalink to &quot;Enviroment variales&quot;">​</a></h1><p>There are various enviroment variables that can control the behavior of the servers, listed here:</p><p><strong>Common variables</strong> Applies to all servers.</p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_HOME</code></td><td>The path to the directory where <code>Lires</code> stores its data.</td><td><code>~/.Lires</code></td></tr><tr><td><code>LRS_KEY</code></td><td>The secret key for inter-service communication.</td><td></td></tr><tr><td><code>LRS_TERM_LOG_LEVEL</code></td><td>The terminal logging level.</td><td><code>INFO</code></td></tr><tr><td><code>LRS_LOG_LEVEL</code></td><td>The logging level send to the log server.</td><td><code>DEBUG</code></td></tr></tbody></table><p><strong><code>lires server</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_SSL_KEYFILE</code></td><td>The path to the SSL key file. (must be used with <code>LRS_SSL_CERTFILE</code>)</td><td></td></tr><tr><td><code>LRS_SSL_CERTFILE</code></td><td>The path to the SSL certificate file.</td><td></td></tr><tr><td><code>LRS_DEV</code></td><td>Set to <code>1</code> to enable server auto-reload on file change</td><td><code>0</code></td></tr><tr><td><code>TVDB_CACHE_DIR</code></td><td>The path to the <code>tiny_vectordb</code> cache directory.</td><td></td></tr><tr><td><code>TVDB_BACKEND</code></td><td>The <code>tiny_vectordb</code> backend to use, can be set to <code>numpy</code> if error occurs.</td><td><code>cxx</code></td></tr></tbody></table><p><strong><code>lires ai</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>HF_HOME</code></td><td>The path to the Hugging Face home directory.</td><td><code>~/.cache/huggingface</code></td></tr><tr><td><code>HF_ENDPONT</code></td><td>The Hugging Face API endpoint.</td><td><code>&quot;https://huggingface.co&quot;</code></td></tr><tr><td><code>OPENAI_API_BASE</code></td><td>The OpenAI API base URL.</td><td><code>&quot;https://api.openai.com/v1</code></td></tr><tr><td><code>OPENAI_API_KEY</code></td><td>The OpenAI API key.</td><td></td></tr></tbody></table><p><strong>Lires-web build variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>VITE_MAINTAINER_NAME</code></td><td>The name of the maintainer.</td><td></td></tr><tr><td><code>VITE_MAINTAINER_EMAIL</code></td><td>The email of the maintainer.</td><td></td></tr></tbody></table></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-20T10:02:00.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/manage.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Management</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/obsidianPlugin.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Obsidian Plugin</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_deployment_enviromentVariables" data-v-39a288b8><div><h1 id="enviroment-variales" tabindex="-1">Enviroment variales <a class="header-anchor" href="#enviroment-variales" aria-label="Permalink to &quot;Enviroment variales&quot;">​</a></h1><p>There are various enviroment variables that can control the behavior of the servers, listed here:</p><p><strong>Common variables</strong> Applies to all servers.</p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_HOME</code></td><td>The path to the directory where <code>Lires</code> stores its data.</td><td><code>~/.Lires</code></td></tr><tr><td><code>LRS_KEY</code></td><td>The secret key for inter-service communication.</td><td></td></tr><tr><td><code>LRS_TERM_LOG_LEVEL</code></td><td>The terminal logging level.</td><td><code>INFO</code></td></tr><tr><td><code>LRS_LOG_LEVEL</code></td><td>The logging level send to the log server.</td><td><code>DEBUG</code></td></tr></tbody></table><p><strong><code>lires server</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>LRS_SSL_KEYFILE</code></td><td>The path to the SSL key file. (must be used with <code>LRS_SSL_CERTFILE</code>)</td><td></td></tr><tr><td><code>LRS_SSL_CERTFILE</code></td><td>The path to the SSL certificate file.</td><td></td></tr><tr><td><code>LRS_DEV</code></td><td>Set to <code>1</code> to enable server auto-reload on file change.</td><td><code>0</code></td></tr><tr><td><code>TVDB_CACHE_DIR</code></td><td>The path to the <code>tiny_vectordb</code> cache directory.</td><td></td></tr><tr><td><code>TVDB_BACKEND</code></td><td>The <code>tiny_vectordb</code> backend to use, can be set to <code>numpy</code> if error occurs.</td><td><code>cxx</code></td></tr></tbody></table><p><strong><code>lires ai</code> variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>HF_HOME</code></td><td>The path to the Hugging Face home directory.</td><td><code>~/.cache/huggingface</code></td></tr><tr><td><code>HF_ENDPONT</code></td><td>The Hugging Face API endpoint.</td><td><code>&quot;https://huggingface.co&quot;</code></td></tr><tr><td><code>OPENAI_API_BASE</code></td><td>The OpenAI API base URL.</td><td><code>&quot;https://api.openai.com/v1</code></td></tr><tr><td><code>OPENAI_API_KEY</code></td><td>The OpenAI API key.</td><td></td></tr></tbody></table><p><strong>Lires-web build variables</strong></p><table><thead><tr><th>Variable</th><th>Description</th><th>Default</th></tr></thead><tbody><tr><td><code>VITE_MAINTAINER_NAME</code></td><td>The name of the maintainer.</td><td></td></tr><tr><td><code>VITE_MAINTAINER_EMAIL</code></td><td>The email of the maintainer.</td><td></td></tr></tbody></table></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-21T05:45:24.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/manage.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Management</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/obsidianPlugin.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Obsidian Plugin</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -33,15 +33,15 @@
 LRS_TERM_LOG_LEVEL The terminal logging level.                      INFO
 LRS_LOG_LEVEL      The logging level send to the log server.        DEBUG
 lliirreess sseerrvveerr vvaarriiaabblleess
 VVaarriiaabbllee         DDeessccrriippttiioonn                                           DDeeffaauulltt
 LRS_SSL_KEYFILE  The path to the SSL key file. (must be used with
                  LRS_SSL_CERTFILE)
 LRS_SSL_CERTFILE The path to the SSL certificate file.
-LRS_DEV          Set to 1 to enable server auto-reload on file change  0
+LRS_DEV          Set to 1 to enable server auto-reload on file change. 0
 TVDB_CACHE_DIR   The path to the tiny_vectordb cache directory.
 TVDB_BACKEND     The tiny_vectordb backend to use, can be set to numpy cxx
                  if error occurs.
 lliirreess aaii vvaarriiaabblleess
 VVaarriiaabbllee        DDeessccrriippttiioonn                       DDeeffaauulltt
 HF_HOME         The path to the Hugging Face home ~/.cache/huggingface
                 directory.
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/gettingStarted.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/gettingStarted.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <meta name="generator" content="VitePress v1.1.4">
     <link rel="preload stylesheet" href="/documentation/assets/style.CT5GXN_K.css" as="style">
     
     <script type="module" src="/documentation/assets/app.CngJ_OZF.js"></script>
     <link rel="preload" href="/documentation/assets/inter-roman-latin.Di8DUHzh.woff2" as="font" type="font/woff2" crossorigin="">
     <link rel="modulepreload" href="/documentation/assets/chunks/theme.CfuCmiaJ.js">
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
-    <link rel="modulepreload" href="/documentation/assets/deployment_gettingStarted.md.DpAQEIqk.lean.js">
+    <link rel="modulepreload" href="/documentation/assets/deployment_gettingStarted.md.CAqJg6m3.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_deployment_gettingStarted" data-v-39a288b8><div><h1 id="getting-started" tabindex="-1">Getting Started <a class="header-anchor" href="#getting-started" aria-label="Permalink to &quot;Getting Started&quot;">​</a></h1><p>This guide will help you to install and start the Lires server.<br> For using it with Docker, please refer to <a href="./docker.html">Docker Deployment</a>.</p><h2 id="table-of-contents" tabindex="-1">Table of Contents <a class="header-anchor" href="#table-of-contents" aria-label="Permalink to &quot;Table of Contents&quot;">​</a></h2><nav class="table-of-contents"><ul><li><a href="#table-of-contents">Table of Contents</a></li><li><a href="#installation">Installation</a><ul><li><a href="#from-pypi">From PyPI</a></li><li><a href="#from-source">From source</a></li></ul></li><li><a href="#server-startup">Server startup</a><ul><li><a href="#manual-startup">Manual startup</a></li><li><a href="#cluster-startup">Cluster startup</a></li><li><a href="#create-the-first-user">Create the first user</a></li></ul></li><li><a href="#management">Management</a></li></ul></nav><h2 id="installation" tabindex="-1">Installation <a class="header-anchor" href="#installation" aria-label="Permalink to &quot;Installation&quot;">​</a></h2><h3 id="from-pypi" tabindex="-1">From PyPI <a class="header-anchor" href="#from-pypi" aria-label="Permalink to &quot;From PyPI&quot;">​</a></h3><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">pip</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> install</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> &#39;Lires[all]&#39;</span></span></code></pre></div><h3 id="from-source" tabindex="-1">From source <a class="header-anchor" href="#from-source" aria-label="Permalink to &quot;From source&quot;">​</a></h3><ol><li>Compile frontend files</li></ol><blockquote><p><strong>Prerequisites:</strong> Node.js, Make</p></blockquote><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">make</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> build</span></span></code></pre></div><ol start="2"><li>Install the servers</li></ol><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">pip</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> install</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> &quot;.[all]&quot;</span></span></code></pre></div><h2 id="server-startup" tabindex="-1">Server startup <a class="header-anchor" href="#server-startup" aria-label="Permalink to &quot;Server startup&quot;">​</a></h2><h3 id="manual-startup" tabindex="-1">Manual startup <a class="header-anchor" href="#manual-startup" aria-label="Permalink to &quot;Manual startup&quot;">​</a></h3><p>Start the microservices with the following commands:</p><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> registry</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">  # the global resource module, for service discovery</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> log</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # the log service</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lires</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> ai</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">        # the AI service</span></span>
@@ -24,12 +24,12 @@
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-cluster</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">your/configuration.yam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">l</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --generate</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># Edit the configuration file</span></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># ...</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># Start the cluster</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-cluster</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">your/configuration.yam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">l</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span></span></code></pre></div><p>The configuration file designates the environment variables, as well as the command line arguments for each server.</p><hr><h3 id="create-the-first-user" tabindex="-1">Create the first user <a class="header-anchor" href="#create-the-first-user" aria-label="Permalink to &quot;Create the first user&quot;">​</a></h3><p><strong>On the first run</strong> you need to create a user account, which can be done by running the <code>lrs-user</code> command in the container.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># export LRS_HOME=&quot;...&quot;</span></span>
-<span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> add</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --admin</span></span></code></pre></div><p>After the user is created, you can manage other users with this user via the web interface.<br> For more information, see <a href="./manage.html#user-management">User management</a>.</p><h2 id="management" tabindex="-1">Management <a class="header-anchor" href="#management" aria-label="Permalink to &quot;Management&quot;">​</a></h2><p>There are several management tools for the server, they are all accessible by <code>lrs-&lt;tool_name&gt;</code>.<br> A list of all the tools and common tasks can be found in <a href="./manage.html">manage.md</a>.</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-19T14:24:52.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Deployment</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/docker.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Docker Deployment</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+<span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> add</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --admin</span></span></code></pre></div><p>For more information, see <a href="./manage.html#user-management">User management</a>.</p><h2 id="management" tabindex="-1">Management <a class="header-anchor" href="#management" aria-label="Permalink to &quot;Management&quot;">​</a></h2><p>There are several management tools for the server, they are all accessible by <code>lrs-&lt;tool_name&gt;</code>.<br> A list of all the tools and common tasks can be found in <a href="./manage.html">manage.md</a>.</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-21T05:45:24.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Deployment</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/docker.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Docker Deployment</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -98,16 +98,14 @@
 ===============================================================================
 ******** CCrreeaattee tthhee ffiirrsstt uusseerr _?​ ********
 OOnn tthhee ffiirrsstt rruunn you need to create a user account, which can be done by
 running the lrs-user command in the container.
 sh
 # export LRS_HOME="..."
 lrs-user add <username> <password> --admin
-After the user is created, you can manage other users with this user via the
-web interface.
 For more information, see _U_s_e_r_ _m_a_n_a_g_e_m_e_n_t.
 ********** MMaannaaggeemmeenntt _?​ **********
 There are several management tools for the server, they are all accessible by
 lrs-<tool_name>.
 A list of all the tools and common tasks can be found in _m_a_n_a_g_e_._m_d.
 Last updated:
 Pager
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/index.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/deployment_index.md.CoeEU7dC.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink active" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_deployment_" data-v-39a288b8><div><h1 id="deployment" tabindex="-1">Deployment <a class="header-anchor" href="#deployment" aria-label="Permalink to &quot;Deployment&quot;">​</a></h1><p>The documentation is for the deployment of Lires. For user manual, please refer to the <a href="/documentation/manual/">User Manual</a>.</p><p>The source code of the project is available on <a href="https://github.com/menxli/lires" target="_blank" rel="noreferrer">GitHub</a>.</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T14:28:24.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/api.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>API</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/gettingStarted.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Getting Started</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/manage.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/manage.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-invite</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">      # Manage invitation codes</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">        # Manage user accounts</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-log</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">         # Check and view logs</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-clear</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # Clear data files</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-reset</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # To reset default configuration</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-index</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # To build and query feature of the database, for fuzzy search</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-utils</span><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;">       # Miscellaneous utilities (e.g. update pdf.js and edit configuration file)</span></span></code></pre></div><p><strong>The tools are self-explanatory by name, all the tools are written with <code>argparse</code> and have a help message that can be accessed by <code>lrs-&lt;tool_name&gt; -h</code>.</strong></p><p><em>Following are some common management tasks.</em></p><h2 id="user-management" tabindex="-1">User management <a class="header-anchor" href="#user-management" aria-label="Permalink to &quot;User management&quot;">​</a></h2><p>After installation, user should be registered with <code>lrs-user</code> command.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> add</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span></span></code></pre></div><p>Or you want to change the password, or admin status of a user, run:</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> update</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">usernam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -p</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">passwor</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">d</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --admin</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> true</span></span></code></pre></div><p>You can check current user information with:</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-user</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> list</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -t</span></span></code></pre></div><h3 id="invitation-code" tabindex="-1">Invitation code <a class="header-anchor" href="#invitation-code" aria-label="Permalink to &quot;Invitation code&quot;">​</a></h3><p>In addition, the user is allowed to register from the web interface with an invitation code. The invitation code can be managed by <code>lrs-invite</code> command.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-invite</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> create</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">cod</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -m</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">max_us</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span></span></code></pre></div><h2 id="log-management" tabindex="-1">Log management <a class="header-anchor" href="#log-management" aria-label="Permalink to &quot;Log management&quot;">​</a></h2><p>The log service is used to store the logs of the application, the log server can have multiple instances, each one will store the logs in a separate sqlite database.</p><p>The logs can be accessed by <code>lrs-log</code> command, the output is combined from the results of all log servers.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-log</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> check</span></span></code></pre></div><p>This will check the overall logged information, specifically the table names and the number of logs in each table.</p><p>To view the log, run:</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-log</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> view</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -t</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">table_nam</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">e</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> |</span><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;"> less</span></span></code></pre></div><p>Since every startup of the log server will create a new log file, it is recommended to periodically archive the logs.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-log</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> merge</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> --rm</span></span></code></pre></div><p>This will merge all the log files into a single file, and remove the original files.</p><div class="warning custom-block"><p class="custom-block-title">WARNING</p><p>Log archiving should be done when the log server is not running, otherwise, the log server will try to write to the removed files and cause errors.</p></div></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-19T11:45:12.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/docker.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Docker Deployment</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/enviromentVariables.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Enviroment Variables</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/deployment/obsidianPlugin.html` & `Lires-1.8.3/lires_server/assets/docs/deployment/obsidianPlugin.html`

 * *Files 0% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     <link rel="modulepreload" href="/documentation/assets/deployment_obsidianPlugin.md.nIZEfUDA.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_deployment_obsidianPlugin" data-v-39a288b8><div><h1 id="obsidian-plugin" tabindex="-1">Obsidian Plugin <a class="header-anchor" href="#obsidian-plugin" aria-label="Permalink to &quot;Obsidian Plugin&quot;">​</a></h1><p>Build the <a href="https://obsidian.md/" target="_blank" rel="noreferrer">Obsidian</a> plugin.</p><h2 id="installation" tabindex="-1">Installation <a class="header-anchor" href="#installation" aria-label="Permalink to &quot;Installation&quot;">​</a></h2><p>Build the plugin with:</p><div class="language-bash vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">bash</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">make</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> obsidian-build</span></span></code></pre></div><p>Then, copy everything under the <code>plugins/obsidian/dist</code> directory to your Obsidian plugins directory, i.e.</p><div class="language-sh vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">sh</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">mkdir</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> -p</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">YOUR_VAUL</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">T</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">/.obsidian/plugins/lires</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">cp</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> plugins/obsidian/dist/</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;">*</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> &lt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">YOUR_VAUL</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">T</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">&gt;</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">/.obsidian/plugins/lires/</span></span></code></pre></div><h2 id="usage" tabindex="-1">Usage <a class="header-anchor" href="#usage" aria-label="Permalink to &quot;Usage&quot;">​</a></h2><p>Please refer to the <a href="./../manual/obsidianPlugin.html">user manual</a> for the usage of the plugin.</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-19T11:49:08.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/enviromentVariables.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Enviroment Variables</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/dev/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Development</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/dev/index.html` & `Lires-1.8.3/lires_server/assets/docs/dev/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">make</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> build</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># fetch third party libs</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">lrs-utils</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> update_pdfjs</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#6A737D;--shiki-dark:#6A737D;"># build for distribution</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">python</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> setup.py</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> sdist</span></span></code></pre></div></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-14T11:58:58.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/deployment/obsidianPlugin.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Obsidian Plugin</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/dev/roadmap.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Roadmap</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/dev/roadmap.html` & `Lires-1.8.3/lires_server/assets/docs/dev/roadmap.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/dev_roadmap.md.JuQ1QPZz.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_dev_roadmap" data-v-39a288b8><div><h1 id="roadmap" tabindex="-1">Roadmap <a class="header-anchor" href="#roadmap" aria-label="Permalink to &quot;Roadmap&quot;">​</a></h1><p>Future plans for the project.</p><h2 id="planned-changes-for-the-next-minor-release-1-9-x" tabindex="-1">Planned changes for the next minor release (1.9.x) <a class="header-anchor" href="#planned-changes-for-the-next-minor-release-1-9-x" aria-label="Permalink to &quot;Planned changes for the next minor release (1.9.x)&quot;">​</a></h2><div class="info custom-block"><p class="custom-block-title">INFO</p><p>These are not finalized.</p></div><ul><li>Move chat api to frontend</li><li>No CORS</li></ul><h2 id="future-plans-without-specific-timeline" tabindex="-1">Future plans without specific timeline <a class="header-anchor" href="#future-plans-without-specific-timeline" aria-label="Permalink to &quot;Future plans without specific timeline&quot;">​</a></h2><p>(TO BE UPDATED)</p><details class="details custom-block"><summary>ideas</summary><ul><li>add a <code>dispatch</code> class to the gateway, which can be used to dispatch messages to other services</li></ul></details></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-20T12:35:16.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/dev/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Development</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><!----></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/hashmap.json` & `Lires-1.8.3/lires_server/assets/docs/hashmap.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9117647058823529%*

 * *Differences: {"'deployment_enviromentvariables.md'": "'Bts03XC7'",*

 * * "'deployment_gettingstarted.md'": "'CAqJg6m3'",*

 * * "'manual_user-interface.md'": "'CdSRMwMo'"}*

```diff
@@ -1,19 +1,19 @@
 {
     "deployment_docker.md": "qRcDU1HX",
-    "deployment_enviromentvariables.md": "C9ixW2VB",
-    "deployment_gettingstarted.md": "DpAQEIqk",
+    "deployment_enviromentvariables.md": "Bts03XC7",
+    "deployment_gettingstarted.md": "CAqJg6m3",
     "deployment_index.md": "CoeEU7dC",
     "deployment_manage.md": "BIu_1sX3",
     "deployment_obsidianplugin.md": "nIZEfUDA",
     "dev_index.md": "BWyXioCS",
     "dev_roadmap.md": "JuQ1QPZz",
     "index.md": "DPNZS3UP",
     "manual_add-document.md": "DrcA27xh",
     "manual_add-edit-entry.md": "DrmD-fBC",
     "manual_api.md": "D91ytbUt",
     "manual_filter-entry.md": "BYNwwSc_",
     "manual_index.md": "Bw2M76Cg",
     "manual_obsidianplugin.md": "D4E6RQm8",
     "manual_read.md": "DFrZ1-Iq",
-    "manual_user-interface.md": "pJkOzfoZ"
+    "manual_user-interface.md": "CdSRMwMo"
 }
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/index.html` & `Lires-1.8.3/lires_server/assets/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/index.md.DPNZS3UP.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar home top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink active" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><!----><!----><div class="VPContent is-home" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPHome" data-v-1428d186 data-v-686f80a6><!--[--><!--]--><div class="VPHero VPHomeHero" data-v-686f80a6 data-v-303bb580><div class="container" data-v-303bb580><div class="main" data-v-303bb580><!--[--><!--]--><!--[--><h1 class="name" data-v-303bb580><span class="clip" data-v-303bb580>Hello!</span></h1><p class="text" data-v-303bb580>Welcome to Lires documentation.</p><p class="tagline" data-v-303bb580>Lires: A self-hosted research literature manager.</p><!--]--><!--[--><!--]--><div class="actions" data-v-303bb580><!--[--><div class="action" data-v-303bb580><a class="VPButton medium brand" href="/documentation/manual/" data-v-303bb580 data-v-cad61b99>Manual</a></div><div class="action" data-v-303bb580><a class="VPButton medium alt" href="/documentation/deployment/" data-v-303bb580 data-v-cad61b99>Deployment</a></div><!--]--></div><!--[--><!--]--></div><!----></div></div><!--[--><!--]--><!--[--><!--]--><!----><!--[--><!--]--><div class="vp-doc container" style="--vp-offset:calc(50% - Infinitypx);" data-v-686f80a6 data-v-82d4af08><!--[--><div style="position:relative;" data-v-686f80a6><div><p><img src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires_v1.7.3.png" alt=""></p></div></div><!--]--></div></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/add-document.html` & `Lires-1.8.3/lires_server/assets/docs/manual/add-document.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/manual_add-document.md.DrcA27xh.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_add-document" data-v-39a288b8><div><h1 id="添加文档" tabindex="-1">添加文档 <a class="header-anchor" href="#添加文档" aria-label="Permalink to &quot;添加文档&quot;">​</a></h1><p>在添加条目后，可以向条目添加文档。目前支持的文档类型包括PDF, HTML 和 图像文件（图像文件会被转换为HTML）。</p><h2 id="在主界面中添加" tabindex="-1">在主界面中添加 <a class="header-anchor" href="#在主界面中添加" aria-label="Permalink to &quot;在主界面中添加&quot;">​</a></h2><p>欲添加文档，可以在主界面中点击数据卡片的<code>Actions</code>按钮，展开操作菜单， 点击<code>Upload document</code>即可选择并上传文档。</p><p><img class="lires-manual-screenshot" style="width:20rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-actionsUnfold-v1.3.0.png" alt="lires-actionsUnfold"></p><p>在条目包含文档后，数据卡片的<code>Upload document</code>按钮会变为<code>Free document</code>， 点击则会删除文档，以便重新上传。</p><h2 id="在阅读器中添加" tabindex="-1">在阅读器中添加 <a class="header-anchor" href="#在阅读器中添加" aria-label="Permalink to &quot;在阅读器中添加&quot;">​</a></h2><p>当阅读器中没有文档的时候，会显示<code>No file, drag and drop to upload</code>的提示。 此时可以直接拖拽文档到阅读器中，或点击<code>upload</code>按钮上传。</p><p>此外，还可以点击右上角操作区的<code>replace</code>按钮选择并上传文档。 此时若存在原文档，无需提前删除，可以直接替换当前文档。</p><p><img class="lires-manual-screenshot" style="width:20rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-readerOptions-v1.7.3.png" alt="lires-readerOptions"></p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T10:18:28.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/add-edit-entry.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>编辑条目</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/filter-entry.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>查找条目</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/add-edit-entry.html` & `Lires-1.8.3/lires_server/assets/docs/manual/add-edit-entry.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/manual_add-edit-entry.md.DrmD-fBC.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_add-edit-entry" data-v-39a288b8><div><h1 id="添加与编辑条目" tabindex="-1">添加与编辑条目 <a class="header-anchor" href="#添加与编辑条目" aria-label="Permalink to &quot;添加与编辑条目&quot;">​</a></h1><p>将一条新条目添加到文献库中，或编辑已有条目的信息。</p><h2 id="条目编辑窗口" tabindex="-1">条目编辑窗口 <a class="header-anchor" href="#条目编辑窗口" aria-label="Permalink to &quot;条目编辑窗口&quot;">​</a></h2><p>通过点击主页右上角工具栏中的<code>添加条目 (New)</code>按钮，或点击扩展数据卡中的<code>Edit</code>按钮， 可以进入条目编辑页面。条目编辑页面中可编辑包括文献信息、标签和URL在内的条目信息。</p><p>下方展示了条目编辑界面，在界面左侧可以输入文献信息（目前支持bibtex、endnote和nbib格式）和URL，右侧可以添加标签。</p><p>在新建条目时会出现<code>Select document</code>按钮，可以通过点击该按钮或者拖拽上传文件， 文件将作为条目的附件，省去后续添加文档。</p><p><img class="lires-manual-screenshot" style="width:20rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-newEntry-v1.4.3.png" alt="lires-newEntry"></p><div class="tip custom-block"><p class="custom-block-title">TIP</p><p>当数据卡片展开，并且鼠标悬停在数据卡片上时，可以使用空格键进入编辑界面</p></div><h2 id="文献信息录入" tabindex="-1">文献信息录入 <a class="header-anchor" href="#文献信息录入" aria-label="Permalink to &quot;文献信息录入&quot;">​</a></h2><p>当上述窗口打开时，除了手动粘贴录入文献信息，还可使用如下方式：</p><ol><li>向信息输入框（或主页）内拖入文本文档（如bibtex文件），此时将会将文本文档内容读取并输入文献信息栏。</li><li>当有文献索引号（如ArXiv ID、DOI）时，可以点击Bibtex标签旁的<code>from-source</code>按钮，此时将弹出如下界面，可使尝试使用文献索引号从网络获取文献信息。</li><li>当需要完全手动输入时，可以点击Bibtex标签旁的<code>template</code>，此时可以选择插入bibtex模版，以辅助录入</li></ol><h2 id="标签录入" tabindex="-1">标签录入 <a class="header-anchor" href="#标签录入" aria-label="Permalink to &quot;标签录入&quot;">​</a></h2><p>通过右侧的标签栏即可选择现有标签或添加新标签。 标签栏选择框内显示标签为文献库中所有标签的集合，通过点击即可选择现有标签。 标签支持多级嵌套，当需要添加新的多级标签时，需要使用-&gt;符号将层级标签相连，如下图所示：</p><p><img class="lires-manual-screenshot" style="width:15rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-addTag-v1.3.0.png" alt="lires-addTag"></p><h2 id="url录入" tabindex="-1">URL录入 <a class="header-anchor" href="#url录入" aria-label="Permalink to &quot;URL录入&quot;">​</a></h2><p>通过在URL栏内输入即可添加URL。</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T10:18:28.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/user-interface.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>界面元素</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/add-document.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>添加文档</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/api.html` & `Lires-1.8.3/lires_server/assets/docs/manual/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -90,11 +90,11 @@
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">async</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> def</span><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;"> main</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">():</span></span>
 <span class="line"><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">    conn </span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">=</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;"> ServerConn(</span><span style="--shiki-light:#E36209;--shiki-dark:#FFAB70;">endpoint</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">=</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">&quot;https://...&quot;</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">, </span><span style="--shiki-light:#E36209;--shiki-dark:#FFAB70;">token</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">=</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">&quot;...&quot;</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">)</span></span>
 <span class="line"><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;">    print</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">(</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">await</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;"> conn.status())</span></span>
 <span class="line"></span>
 <span class="line"><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;">if</span><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;"> __name__</span><span style="--shiki-light:#D73A49;--shiki-dark:#F97583;"> ==</span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;"> &quot;__main__&quot;</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">:</span></span>
 <span class="line"><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">    asyncio.run(main())</span></span></code></pre></div><h2 id="restful-api" tabindex="-1">RESTful API <a class="header-anchor" href="#restful-api" aria-label="Permalink to &quot;RESTful API&quot;">​</a></h2><p>本质上，后端实现了一套RESTful API，上述API都是基于HTTP请求实现的。<br> 然而本软件目前处于开发阶段，API可能会有变动，因此不建议直接使用HTTP请求进行操作， 建议使用上述封装好的API库。</p><p>若要使用RESTful API，可以参考<a href="https://github.com/MenxLi/Lires/blob/dev/lires_server/main.py" target="_blank" rel="noreferrer">网关服务实现</a></p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-04-17T04:30:05.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/obsidianPlugin.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>Obsidian插件</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/deployment/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Deployment</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/filter-entry.html` & `Lires-1.8.3/lires_server/assets/docs/manual/filter-entry.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/manual_filter-entry.md.BYNwwSc_.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_filter-entry" data-v-39a288b8><div><h1 id="查找条目" tabindex="-1">查找条目 <a class="header-anchor" href="#查找条目" aria-label="Permalink to &quot;查找条目&quot;">​</a></h1><p>通过筛选，在数据库中查找所需条目。</p><h2 id="标签筛选" tabindex="-1">标签筛选 <a class="header-anchor" href="#标签筛选" aria-label="Permalink to &quot;标签筛选&quot;">​</a></h2><p>标签筛选是最简单的筛选方式，只需要在主页面中选择左侧标签栏中相应的标签即可。 目前标签筛选只支持标签的交集，即同时满足所有标签的条目。</p><div class="tip custom-block"><p class="custom-block-title">TIP</p><p>标签筛选需要对标签进行良好的维护， 如果不需要此功能，可以在设置中点击<code>️Tag Display</code>按钮，关闭标签功能。</p></div><h2 id="内容搜索" tabindex="-1">内容搜索 <a class="header-anchor" href="#内容搜索" aria-label="Permalink to &quot;内容搜索&quot;">​</a></h2><p>在主界面工具栏最右侧的搜索框中输入关键词，即可进行内容搜索筛选，输入内容不区分大小写，支持模糊匹配。 搜索结果会结合标签筛选的结果，以交集形式显示出符合条件的条目。</p><p>可以通过搜索栏旁的下拉菜单选择搜索的范围，包括标题、作者、笔记等。 下图显示了搜索栏的可选范围：</p><p><img class="lires-manual-screenshot" style="width:15rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-searchSelect-dark-v1.3.0.png" alt="lires-searchSelect"></p><h2 id="语义搜索" tabindex="-1">语义搜索 <a class="header-anchor" href="#语义搜索" aria-label="Permalink to &quot;语义搜索&quot;">​</a></h2><p>通过选择搜索栏中的<code>feature</code>类型，可以基于条目特征进行向量搜索。 此时，并不会筛除数据，而是将语义上与搜索内容更相似度越高的条目排在前面。</p><div class="info custom-block"><p class="custom-block-title">INFO</p><p>向量提取 向量提取基于文献的摘要信息，因此建议在添加文献时，尽量添加摘要信息。 当文献没有摘要信息时，会依照AI摘要、全文、和标题的优先级顺序进行向量索引构建。</p><p>目前向量索引每12小时会更新一次，因此如果添加了新的文献，需要等待一段时间后才能进行向量搜索。</p></div><div class="tip custom-block"><p class="custom-block-title">TIP</p><p>基于语义搜索，还可以进行相似文献发现。 在数据卡片的概览窗口和推送页面的推送卡片中，点击<code>related works</code>按钮，即可进行相似文献发现， 此时，数据卡片中会出现相似度评分，评分越高，相似度越高。</p></div><p>除此以外，软件还提供数据可视化功能，可以将数据卡片中的向量信息可视化为三维空间中的点云，方便进行数据分析。</p><p>通过开启设置中的<code>Scatter Plot</code>按钮，即可打开可视化页面，由于此时需要在服务器端进行数据处理， 因此开启可视化功能时，需要等待一段时间，直到数据处理完成。 如果在进行可视化时，进行向量搜索，会在可视化页面中以颜色显示出搜索结果与内容相似度的大小，如下图所示：</p><p><img class="lires-manual-screenshot" style="width:30rem;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-vectorSearchVis-dark-v1.7.3.png" alt="lires-vectorSearchVis"></p><div class="info custom-block"><p class="custom-block-title">INFO</p><ul><li>在数据库文献数量小于5时，无法绘制可视化图像。</li><li>开启可视化会增加带宽消耗，并且导致渲染开销增加，当数据量较大时，可能会导致页面卡顿。</li></ul></div></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T10:18:28.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/add-document.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>添加文档</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/read.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>阅读文档</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/index.html` & `Lires-1.8.3/lires_server/assets/docs/manual/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/manual_index.md.Bw2M76Cg.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink active" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_" data-v-39a288b8><div><h1 id="用户手册" tabindex="-1">用户手册 <a class="header-anchor" href="#用户手册" aria-label="Permalink to &quot;用户手册&quot;">​</a></h1><p>一个非常简单的用户手册。</p><p>如果需要自己部署，请参考<a href="/documentation/deployment/">Deployment</a>。</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T14:28:24.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><!----></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/user-interface.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>界面元素</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/obsidianPlugin.html` & `Lires-1.8.3/lires_server/assets/docs/manual/obsidianPlugin.html`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
     <link rel="modulepreload" href="/documentation/assets/manual_obsidianPlugin.md.D4E6RQm8.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_obsidianPlugin" data-v-39a288b8><div><h1 id="obsidian-插件" tabindex="-1">Obsidian 插件 <a class="header-anchor" href="#obsidian-插件" aria-label="Permalink to &quot;Obsidian 插件&quot;">​</a></h1><p>从 <a href="https://obsidian.md/" target="_blank" rel="noreferrer">Obsidian</a> 引用 Lires 条目。</p><h2 id="安装" tabindex="-1">安装 <a class="header-anchor" href="#安装" aria-label="Permalink to &quot;安装&quot;">​</a></h2><p>目前本插件尚未发布到 Obsidian 社区插件库，需要<a href="./../deployment/obsidianPlugin.html">从源码构建插件</a> 或从关于页面下载已构建的插件。</p><p>随后手动安装插件： 将插件文件夹拷贝到 Obsidian 插件文件夹中（<code>&lt;vault&gt;/.obsidian/plugins/</code>）， 重启 Obsidian，并在设置中<a href="#启用插件">启用插件</a>。</p><details class="details custom-block"><summary>详细步骤</summary><ol><li>下载并解压得到<code>lires-obsidian-plugin</code>文件夹</li><li>将<code>lires-obsidian-plugin</code>文件夹拷贝到<code>&lt;vault&gt;/.obsidian/plugins/</code>文件夹中，其中<code>&lt;vault&gt;</code>是你的 Obsidian 笔记本文件夹（如<code>/Users/username/Documents/Obsidian/MyVault/.obsidian/plugins/</code>）。如在<code>.obsidian</code>中没有<code>plugins</code>文件夹，可以手动创建。</li><li>重启 Obsidian</li></ol></details><h2 id="启用插件" tabindex="-1">启用插件 <a class="header-anchor" href="#启用插件" aria-label="Permalink to &quot;启用插件&quot;">​</a></h2><p>参考<a href="https://docs.obsidian.md/Plugins/Getting+started/Build+a+plugin#Step+3+Enable+the+plugin" target="_blank" rel="noreferrer">官方指南</a>，进行如下操作：</p><ol><li>打开 Obsidian</li><li>点击 <code>设置</code> -&gt; <code>社区插件</code></li><li>如果尚未启用社区插件，选择 <code>启用社区插件</code></li><li>启用 <code>Lires</code> 插件</li></ol><h2 id="设置lires账户信息" tabindex="-1">设置Lires账户信息 <a class="header-anchor" href="#设置lires账户信息" aria-label="Permalink to &quot;设置Lires账户信息&quot;">​</a></h2><p>打开 Obsidian，点击设置 -&gt; 社区插件 -&gt; Lires -&gt; 设置，输入你的 Lires 账户信息，重启 Obsidian。</p><h2 id="使用" tabindex="-1">使用 <a class="header-anchor" href="#使用" aria-label="Permalink to &quot;使用&quot;">​</a></h2><p>Lires 插件使用代码块形式引用Lires条目， 目前支持两种引用方式：</p><ol><li><code>lires-cite</code>：使用短名称引用条目</li><li><code>lires-ref</code>：生成引用条目的简介信息</li></ol><p><img src="https://pic4.zhimg.com/v2-1963de23d479e77d4b904bd7d36b7f5f_b.webp" alt="obsidian-plugin-gif"></p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-19T11:49:08.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/read.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>阅读文档</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/api.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>API</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/read.html` & `Lires-1.8.3/lires_server/assets/docs/manual/read.html`

 * *Files 0% similar despite different names*

```diff
@@ -19,11 +19,11 @@
   <body>
     <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_read" data-v-39a288b8><div><h1 id="阅读文档" tabindex="-1">阅读文档 <a class="header-anchor" href="#阅读文档" aria-label="Permalink to &quot;阅读文档&quot;">​</a></h1><p>阅读文献并添加笔记</p><h2 id="阅读器" tabindex="-1">阅读器 <a class="header-anchor" href="#阅读器" aria-label="Permalink to &quot;阅读器&quot;">​</a></h2><p>目前使用<a href="https://mozilla.github.io/pdf.js/getting_started/#download" target="_blank" rel="noreferrer">PDF.js Viewer</a>作为阅读器，暂不支持文档编辑功能。 若想要编辑文档，请下载文档到本地，使用本地编辑器进行编辑后点击右上角<code>replace</code>按钮上传文档。</p><h2 id="笔记" tabindex="-1">笔记 <a class="header-anchor" href="#笔记" aria-label="Permalink to &quot;笔记&quot;">​</a></h2><p>本软件使用<code>markdown</code>格式来记录笔记，你可以在笔记中添加文本、图片、代码等内容。 在进行修改时，你可以使用<code>Ctrl+S</code>快捷键来保存笔记。</p><h3 id="添加附件" tabindex="-1">添加附件 <a class="header-anchor" href="#添加附件" aria-label="Permalink to &quot;添加附件&quot;">​</a></h3><p>你可以通过点击<code>upload</code>按钮来 在笔记中添加图片、代码等附件，附件会被自动上传到服务器并在笔记中显示。</p><p>通过点击页面下方的<code>⬆️</code>上标按钮，可以打开附件管理窗口，你可以在这里查看和删除附件。</p><div class="info custom-block"><p class="custom-block-title">INFO</p><p>当笔记中的附件链接被删除时，附件仍然会保留在服务器上，但不会在笔记中显示，请在附件窗口中手动删除附件。</p></div><h3 id="front-matter" tabindex="-1">Front Matter <a class="header-anchor" href="#front-matter" aria-label="Permalink to &quot;Front Matter&quot;">​</a></h3><p>笔记部分支持使用以下元数据来进行配置</p><div class="language-yaml vp-adaptive-theme"><button title="Copy Code" class="copy"></button><span class="lang">yaml</span><pre class="shiki shiki-themes github-light github-dark vp-code"><code><span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">---</span></span>
 <span class="line"><span style="--shiki-light:#22863A;--shiki-dark:#85E89D;">links</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">:</span></span>
 <span class="line"><span style="--shiki-light:#22863A;--shiki-dark:#85E89D;">    url_name1</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">: </span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">url1</span></span>
 <span class="line"><span style="--shiki-light:#22863A;--shiki-dark:#85E89D;">    url_name2</span><span style="--shiki-light:#24292E;--shiki-dark:#E1E4E8;">: </span><span style="--shiki-light:#032F62;--shiki-dark:#9ECBFF;">url2</span></span>
 <span class="line"><span style="--shiki-light:#005CC5;--shiki-dark:#79B8FF;">    ...</span></span>
 <span class="line"><span style="--shiki-light:#6F42C1;--shiki-dark:#B392F0;">---</span></span></code></pre></div><p>目前仅支持<code>links</code>字段，用于添加链接（未来计划支持更多）。 在阅读文献时，你可以在文档的开头添加这个元数据， 此时，页面下端会显示一个链接列表，点击链接可以跳转到对应的网页。</p></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-04-09T02:50:29.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/filter-entry.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>查找条目</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/obsidianPlugin.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>Obsidian插件</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

### Comparing `Lires-1.8.2/lires_server/assets/docs/manual/user-interface.html` & `Lires-1.8.3/lires_server/assets/docs/manual/user-interface.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     <meta name="generator" content="VitePress v1.1.4">
     <link rel="preload stylesheet" href="/documentation/assets/style.CT5GXN_K.css" as="style">
     
     <script type="module" src="/documentation/assets/app.CngJ_OZF.js"></script>
     <link rel="preload" href="/documentation/assets/inter-roman-latin.Di8DUHzh.woff2" as="font" type="font/woff2" crossorigin="">
     <link rel="modulepreload" href="/documentation/assets/chunks/theme.CfuCmiaJ.js">
     <link rel="modulepreload" href="/documentation/assets/chunks/framework.CZXUNLJW.js">
-    <link rel="modulepreload" href="/documentation/assets/manual_user-interface.md.pJkOzfoZ.lean.js">
+    <link rel="modulepreload" href="/documentation/assets/manual_user-interface.md.CdSRMwMo.lean.js">
     <script id="check-dark-mode">(()=>{const e=localStorage.getItem("vitepress-theme-appearance")||"auto",a=window.matchMedia("(prefers-color-scheme: dark)").matches;(!e||e==="auto"?a:e==="dark")&&document.documentElement.classList.add("dark")})();</script>
     <script id="check-mac-os">document.documentElement.classList.toggle("mac",/Mac|iPhone|iPod|iPad/i.test(navigator.platform));</script>
   </head>
   <body>
-    <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_user-interface" data-v-39a288b8><div><h1 id="界面元素" tabindex="-1">界面元素 <a class="header-anchor" href="#界面元素" aria-label="Permalink to &quot;界面元素&quot;">​</a></h1><p>本页面介绍软件的用户界面元素，供读者参考，以便于阅读后续使用说明。</p><p>目前本软件主要实现了以下界面：</p><ul><li>登录页面</li><li>主页面</li><li>阅读器</li><li>推送页面</li><li>关于页面</li></ul><p>可通过点击导航栏中的链接，或界面中的相应按钮，进入相应页面。<br> 以下是各个页面的界面元素介绍。</p><h2 id="工具栏" tabindex="-1">工具栏 <a class="header-anchor" href="#工具栏" aria-label="Permalink to &quot;工具栏&quot;">​</a></h2><p>工具栏是所有页面中的通用元素， 在工具栏左侧包含设置和返回/退出登陆按钮， 右侧是页面导航。 例如，下图是主界面中的工具栏：</p><p><img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-toolbar-dark-v1.7.3.png" alt="lires-toolbar"></p><h2 id="数据卡片" tabindex="-1">数据卡片 <a class="header-anchor" href="#数据卡片" aria-label="Permalink to &quot;数据卡片&quot;">​</a></h2><p>数据卡片（Data Card）是Lires的数据条目展示形式，是主页中的数据内容，也是其他页面中的可编辑数据展示形式。 以下为一张数据卡片： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacard-dark-v1.3.0.png" alt="lires-datacard"></p><p>数据卡片包含了文献标题和作者的基本信息以及操作按钮：</p><ul><li>阅读器（Reader）：点击<code>Reader</code>按钮，可以打开该阅读器对文献信息阅读，同时记录笔记。</li><li>链接（Link）：点击<code>Link</code>按钮，可以在新窗口打开文献链接，当文献没有URL字段时不显示。</li><li>概览（Summary）：点击<code>Summary</code>按钮，可以显示文献的详细信息，尝试使用AI进行总结。</li><li>引用（Cite）：点击<code>Cite</code>按钮，可以显示数种引用格式，点击即可复制。</li><li>操作（Actions）：点击<code>Actions</code>按钮，可以展开操作菜单，包含了编辑条目信息、添加和删除文档、 以及删除条目等操作。</li></ul><p>通过点击<code>Actions</code>和<code>Abstract</code>按钮，可将数据卡片完全展开如下： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardExpand-dark-v1.3.0.png" alt="lires-datacardExpand"></p><p>摘要（Abstract）处用于填入文献的摘要信息，点击摘要正文部分即可进行编辑，当编辑完成后自动保存。</p><p>概览（Summary）界面中展示了包括全部作者、期刊、数据大小等详细信息，尝试使用AI进行自动总结， 并基于语义搜索展示文献库中所有最相关文献。下图是概览界面的展示： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardSummary-dark-v1.3.0.png" alt="lires-datacardSummary"></p><p>若文献库中有同名作者，会在作者名后面标注数字，点击数字即可展开作者的其他条目数据卡片。</p><hr><div class="info custom-block"><p class="custom-block-title">INFO</p><p>待完善</p></div></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-03-28T10:18:28.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>用户手册</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/add-edit-entry.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>编辑条目</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
-    <script>window.__VP_HASH_MAP__=JSON.parse("{\"dev_roadmap.md\":\"JuQ1QPZz\",\"deployment_gettingstarted.md\":\"DpAQEIqk\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_index.md\":\"BWyXioCS\",\"manual_user-interface.md\":\"pJkOzfoZ\",\"manual_read.md\":\"DFrZ1-Iq\",\"deployment_index.md\":\"CoeEU7dC\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"deployment_enviromentvariables.md\":\"C9ixW2VB\",\"manual_add-document.md\":\"DrcA27xh\",\"deployment_manage.md\":\"BIu_1sX3\",\"manual_index.md\":\"Bw2M76Cg\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"manual_api.md\":\"D91ytbUt\",\"index.md\":\"DPNZS3UP\",\"manual_filter-entry.md\":\"BYNwwSc_\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
+    <div id="app"><div class="Layout" data-v-5d98c3a5><!--[--><!--]--><!--[--><span tabindex="-1" data-v-0f60ec36></span><a href="#VPContent" class="VPSkipLink visually-hidden" data-v-0f60ec36> Skip to content </a><!--]--><!----><header class="VPNav" data-v-5d98c3a5 data-v-ae24b3ad><div class="VPNavBar has-sidebar top" data-v-ae24b3ad data-v-ccf7ddec><div class="wrapper" data-v-ccf7ddec><div class="container" data-v-ccf7ddec><div class="title" data-v-ccf7ddec><div class="VPNavBarTitle has-sidebar" data-v-ccf7ddec data-v-ab179fa1><a class="title" href="/documentation/" data-v-ab179fa1><!--[--><!--]--><!----><span data-v-ab179fa1>Lires document</span><!--[--><!--]--></a></div></div><div class="content" data-v-ccf7ddec><div class="content-body" data-v-ccf7ddec><!--[--><!--]--><div class="VPNavBarSearch search" data-v-ccf7ddec><!----></div><nav aria-labelledby="main-nav-aria-label" class="VPNavBarMenu menu" data-v-ccf7ddec data-v-7f418b0f><span id="main-nav-aria-label" class="visually-hidden" data-v-7f418b0f>Main Navigation</span><!--[--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Home</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/manual/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Manual</span><!--]--></a><!--]--><!--[--><a class="VPLink link VPNavBarMenuLink" href="/documentation/deployment/" tabindex="0" data-v-7f418b0f data-v-9c663999><!--[--><span data-v-9c663999>Deployment</span><!--]--></a><!--]--><!--]--></nav><!----><div class="VPNavBarAppearance appearance" data-v-ccf7ddec data-v-e6aabb21><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-e6aabb21 data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div><div class="VPSocialLinks VPNavBarSocialLinks social-links" data-v-ccf7ddec data-v-0394ad82 data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div><div class="VPFlyout VPNavBarExtra extra" data-v-ccf7ddec data-v-d0bd9dde data-v-b6c34ac9><button type="button" class="button" aria-haspopup="true" aria-expanded="false" aria-label="extra navigation" data-v-b6c34ac9><span class="vpi-more-horizontal icon" data-v-b6c34ac9></span></button><div class="menu" data-v-b6c34ac9><div class="VPMenu" data-v-b6c34ac9 data-v-e7ea1737><!----><!--[--><!--[--><!----><div class="group" data-v-d0bd9dde><div class="item appearance" data-v-d0bd9dde><p class="label" data-v-d0bd9dde>Appearance</p><div class="appearance-action" data-v-d0bd9dde><button class="VPSwitch VPSwitchAppearance" type="button" role="switch" title="Switch to dark theme" aria-checked="false" data-v-d0bd9dde data-v-d1f28634 data-v-1d5665e3><span class="check" data-v-1d5665e3><span class="icon" data-v-1d5665e3><!--[--><span class="vpi-sun sun" data-v-d1f28634></span><span class="vpi-moon moon" data-v-d1f28634></span><!--]--></span></span></button></div></div></div><div class="group" data-v-d0bd9dde><div class="item social-links" data-v-d0bd9dde><div class="VPSocialLinks social-links-list" data-v-d0bd9dde data-v-7bc22406><!--[--><a class="VPSocialLink no-icon" href="https://github.com/menxli/lires" aria-label="github" target="_blank" rel="noopener" data-v-7bc22406 data-v-eee4e7cb><span class="vpi-social-github" /></a><!--]--></div></div></div><!--]--><!--]--></div></div></div><!--[--><!--]--><button type="button" class="VPNavBarHamburger hamburger" aria-label="mobile navigation" aria-expanded="false" aria-controls="VPNavScreen" data-v-ccf7ddec data-v-e5dd9c1c><span class="container" data-v-e5dd9c1c><span class="top" data-v-e5dd9c1c></span><span class="middle" data-v-e5dd9c1c></span><span class="bottom" data-v-e5dd9c1c></span></span></button></div></div></div></div><div class="divider" data-v-ccf7ddec><div class="divider-line" data-v-ccf7ddec></div></div></div><!----></header><div class="VPLocalNav has-sidebar empty" data-v-5d98c3a5 data-v-a6f0e41e><div class="container" data-v-a6f0e41e><button class="menu" aria-expanded="false" aria-controls="VPSidebarNav" data-v-a6f0e41e><span class="vpi-align-left menu-icon" data-v-a6f0e41e></span><span class="menu-text" data-v-a6f0e41e>Menu</span></button><div class="VPLocalNavOutlineDropdown" style="--vp-vh:0px;" data-v-a6f0e41e data-v-17a5e62e><button data-v-17a5e62e>Return to top</button><!----></div></div></div><aside class="VPSidebar" data-v-5d98c3a5 data-v-575e6a36><div class="curtain" data-v-575e6a36></div><nav class="nav" id="VPSidebarNav" aria-labelledby="sidebar-aria-label" tabindex="-1" data-v-575e6a36><span class="visually-hidden" id="sidebar-aria-label" data-v-575e6a36> Sidebar Navigation </span><!--[--><!--]--><!--[--><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link has-active" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>用户手册</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/user-interface.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>界面元素</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-edit-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>编辑条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/add-document.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>添加文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/filter-entry.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>查找条目</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/read.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>阅读文档</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian插件</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/manual/api.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>API</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Deployment</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/gettingStarted.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Getting Started</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/docker.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Docker Deployment</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/manage.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Management</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/enviromentVariables.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Enviroment Variables</p><!--]--></a><!----></div><!----></div><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/deployment/obsidianPlugin.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Obsidian Plugin</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><div class="group" data-v-575e6a36><section class="VPSidebarItem level-0 is-link" data-v-575e6a36 data-v-b8d55f3b><div class="item" tabindex="0" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/" data-v-b8d55f3b><!--[--><h2 class="text" data-v-b8d55f3b>Development</h2><!--]--></a><!----></div><div class="items" data-v-b8d55f3b><!--[--><div class="VPSidebarItem level-1 is-link" data-v-b8d55f3b data-v-b8d55f3b><div class="item" data-v-b8d55f3b><div class="indicator" data-v-b8d55f3b></div><a class="VPLink link link" href="/documentation/dev/roadmap.html" data-v-b8d55f3b><!--[--><p class="text" data-v-b8d55f3b>Roadmap</p><!--]--></a><!----></div><!----></div><!--]--></div></section></div><!--]--><!--[--><!--]--></nav></aside><div class="VPContent has-sidebar" id="VPContent" data-v-5d98c3a5 data-v-1428d186><div class="VPDoc has-sidebar has-aside" data-v-1428d186 data-v-39a288b8><!--[--><!--]--><div class="container" data-v-39a288b8><div class="aside" data-v-39a288b8><div class="aside-curtain" data-v-39a288b8></div><div class="aside-container" data-v-39a288b8><div class="aside-content" data-v-39a288b8><div class="VPDocAside" data-v-39a288b8 data-v-3f215769><!--[--><!--]--><!--[--><!--]--><nav aria-labelledby="doc-outline-aria-label" class="VPDocAsideOutline" role="navigation" data-v-3f215769 data-v-269c27a6><div class="content" data-v-269c27a6><div class="outline-marker" data-v-269c27a6></div><div aria-level="2" class="outline-title" id="doc-outline-aria-label" role="heading" data-v-269c27a6>On this page</div><ul class="VPDocOutlineItem root" data-v-269c27a6 data-v-b933a997><!--[--><!--]--></ul></div></nav><!--[--><!--]--><div class="spacer" data-v-3f215769></div><!--[--><!--]--><!----><!--[--><!--]--><!--[--><!--]--></div></div></div></div><div class="content" data-v-39a288b8><div class="content-container" data-v-39a288b8><!--[--><!--]--><main class="main" data-v-39a288b8><div style="position:relative;" class="vp-doc _documentation_manual_user-interface" data-v-39a288b8><div><h1 id="界面元素" tabindex="-1">界面元素 <a class="header-anchor" href="#界面元素" aria-label="Permalink to &quot;界面元素&quot;">​</a></h1><p>本页面简要介绍软件的用户界面元素，供读者参考。<br> 可在此页面查找后续文档所提及界面元素的含义。</p><p>目前本软件主要实现了以下页面：</p><ul><li>登录页面</li><li>主页面</li><li>阅读器</li><li>推送页面</li><li>关于页面</li></ul><p>可通过点击导航栏中的链接，或界面中的相应按钮，进入相应页面。<br> 以下是关键界面元素介绍。</p><h2 id="工具栏" tabindex="-1">工具栏 <a class="header-anchor" href="#工具栏" aria-label="Permalink to &quot;工具栏&quot;">​</a></h2><p>工具栏是所有页面中的通用元素， 在工具栏左侧包含设置和返回/退出登陆按钮， 右侧是页面导航。 例如，下图是主界面中的工具栏：</p><p><img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-toolbar-dark-v1.7.3.png" alt="lires-toolbar"></p><h2 id="数据卡片" tabindex="-1">数据卡片 <a class="header-anchor" href="#数据卡片" aria-label="Permalink to &quot;数据卡片&quot;">​</a></h2><p>数据卡片（Data Card）是Lires的数据条目展示形式，是主页中的数据内容，也是其他页面中的可编辑数据展示形式。 以下为一张数据卡片： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacard-dark-v1.3.0.png" alt="lires-datacard"></p><p>数据卡片包含了文献标题和作者的基本信息以及操作按钮：</p><ul><li>阅读器（Reader）：点击<code>Reader</code>按钮，可以打开该阅读器对文献信息阅读，同时记录笔记。</li><li>链接（Link）：点击<code>Link</code>按钮，可以在新窗口打开文献链接，当文献没有URL字段时不显示。</li><li>概览（Summary）：点击<code>Summary</code>按钮，可以显示文献的详细信息，尝试使用AI进行总结。</li><li>引用（Cite）：点击<code>Cite</code>按钮，可以显示数种引用格式，点击即可复制。</li><li>操作（Actions）：点击<code>Actions</code>按钮，可以展开操作菜单，包含了编辑条目信息、添加和删除文档、 以及删除条目等操作。</li></ul><p>通过点击<code>Actions</code>和<code>Abstract</code>按钮，可将数据卡片完全展开如下： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardExpand-dark-v1.3.0.png" alt="lires-datacardExpand"></p><p>摘要（Abstract）处用于填入文献的摘要信息，点击摘要正文部分即可进行编辑，当编辑完成后自动保存。</p><p>概览（Summary）界面中展示了包括全部作者、期刊、数据大小等详细信息，尝试使用AI进行自动总结， 并基于语义搜索展示文献库中所有最相关文献。下图是概览界面的展示： <img class="lires-manual-screenshot" style="width:100%;" src="https://limengxun-imagebed.oss-cn-wuhan-lr.aliyuncs.com/pic/lires-datacardSummary-dark-v1.3.0.png" alt="lires-datacardSummary"></p><p>若文献库中有同名作者，会在作者名后面标注数字，点击数字即可展开作者的其他条目数据卡片。</p><hr><div class="info custom-block"><p class="custom-block-title">INFO</p><p>待完善</p></div></div></div></main><footer class="VPDocFooter" data-v-39a288b8 data-v-d4a0bba5><!--[--><!--]--><div class="edit-info" data-v-d4a0bba5><!----><div class="last-updated" data-v-d4a0bba5><p class="VPLastUpdated" data-v-d4a0bba5 data-v-7e05ebdb>Last updated: <time datetime="2024-05-21T05:45:24.000Z" data-v-7e05ebdb></time></p></div></div><nav class="prev-next" aria-labelledby="doc-footer-aria-label" data-v-d4a0bba5><span class="visually-hidden" id="doc-footer-aria-label" data-v-d4a0bba5>Pager</span><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link prev" href="/documentation/manual/" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Previous page</span><span class="title" data-v-d4a0bba5>用户手册</span><!--]--></a></div><div class="pager" data-v-d4a0bba5><a class="VPLink link pager-link next" href="/documentation/manual/add-edit-entry.html" data-v-d4a0bba5><!--[--><span class="desc" data-v-d4a0bba5>Next page</span><span class="title" data-v-d4a0bba5>编辑条目</span><!--]--></a></div></nav></footer><!--[--><!--]--></div></div></div><!--[--><!--]--></div></div><!----><!--[--><!--]--></div></div>
+    <script>window.__VP_HASH_MAP__=JSON.parse("{\"deployment_index.md\":\"CoeEU7dC\",\"index.md\":\"DPNZS3UP\",\"manual_user-interface.md\":\"CdSRMwMo\",\"manual_filter-entry.md\":\"BYNwwSc_\",\"deployment_manage.md\":\"BIu_1sX3\",\"deployment_obsidianplugin.md\":\"nIZEfUDA\",\"dev_index.md\":\"BWyXioCS\",\"manual_add-edit-entry.md\":\"DrmD-fBC\",\"deployment_docker.md\":\"qRcDU1HX\",\"dev_roadmap.md\":\"JuQ1QPZz\",\"manual_obsidianplugin.md\":\"D4E6RQm8\",\"manual_read.md\":\"DFrZ1-Iq\",\"manual_index.md\":\"Bw2M76Cg\",\"deployment_enviromentvariables.md\":\"Bts03XC7\",\"manual_add-document.md\":\"DrcA27xh\",\"manual_api.md\":\"D91ytbUt\",\"deployment_gettingstarted.md\":\"CAqJg6m3\"}");window.__VP_SITE_DATA__=JSON.parse("{\"lang\":\"en-US\",\"dir\":\"ltr\",\"title\":\"Lires document\",\"titleTemplate\":\"Lires\",\"description\":\"Lires documentations\",\"base\":\"/documentation/\",\"head\":[],\"router\":{\"prefetchLinks\":true},\"appearance\":true,\"themeConfig\":{\"nav\":[{\"text\":\"Home\",\"link\":\"/\"},{\"text\":\"Manual\",\"link\":\"/manual/\"},{\"text\":\"Deployment\",\"link\":\"/deployment/\"}],\"sidebar\":[{\"text\":\"用户手册\",\"link\":\"/manual/\",\"items\":[{\"text\":\"界面元素\",\"link\":\"/manual/user-interface\"},{\"text\":\"编辑条目\",\"link\":\"/manual/add-edit-entry\"},{\"text\":\"添加文档\",\"link\":\"/manual/add-document\"},{\"text\":\"查找条目\",\"link\":\"/manual/filter-entry\"},{\"text\":\"阅读文档\",\"link\":\"/manual/read\"},{\"text\":\"Obsidian插件\",\"link\":\"/manual/obsidianPlugin\"},{\"text\":\"API\",\"link\":\"/manual/api\"}]},{\"text\":\"Deployment\",\"link\":\"/deployment/\",\"items\":[{\"text\":\"Getting Started\",\"link\":\"/deployment/gettingStarted\"},{\"text\":\"Docker Deployment\",\"link\":\"/deployment/docker\"},{\"text\":\"Management\",\"link\":\"/deployment/manage\"},{\"text\":\"Enviroment Variables\",\"link\":\"/deployment/enviromentVariables\"},{\"text\":\"Obsidian Plugin\",\"link\":\"/deployment/obsidianPlugin\"}]},{\"text\":\"Development\",\"link\":\"/dev/\",\"items\":[{\"text\":\"Roadmap\",\"link\":\"/dev/roadmap\"}]}],\"socialLinks\":[{\"icon\":\"github\",\"link\":\"https://github.com/menxli/lires\"}]},\"locales\":{},\"scrollOffset\":134,\"cleanUrls\":false}");</script>
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -19,23 +19,24 @@
 _M_a_n_a_g_e_m_e_n_t
 _E_n_v_i_r_o_m_e_n_t_ _V_a_r_i_a_b_l_e_s
 _O_b_s_i_d_i_a_n_ _P_l_u_g_i_n
 _**_**_**_**_**_ _DD_ee_vv_ee_ll_oo_pp_mm_ee_nn_tt_ _**_**_**_**_**
 _R_o_a_d_m_a_p
 On this page
 ************ ?界?面?元?素 _?​ ************
-本页面介绍软件的用户界面元素，供读者参考，以便于阅读后续使用说明。
-目前本软件主要实现了以下界面：
+本页面简要介绍软件的用户界面元素，供读者参考。
+可在此页面查找后续文档所提及界面元素的含义。
+目前本软件主要实现了以下页面：
     * 登录页面
     * 主页面
     * 阅读器
     * 推送页面
     * 关于页面
 可通过点击导航栏中的链接，或界面中的相应按钮，进入相应页面。
-以下是各个页面的界面元素介绍。
+以下是关键界面元素介绍。
 ********** ?工?具?栏 _?​ **********
 工具栏是所有页面中的通用元素， 在工具栏左侧包含设置和返回/退出登陆按钮， 右侧是页面导航。 例如，下图是主界面中的工具栏：
 [lires-toolbar]
 ********** ?数?据?卡?片 _?​ **********
 数据卡片（Data Card）是Lires的数据条目展示形式，是主页中的数据内容，也是其他页面中的可编辑数据展示形式。 以下为一张数据卡片：[lires-
 datacard]
 数据卡片包含了文献标题和作者的基本信息以及操作按钮：
```

### Comparing `Lires-1.8.2/lires_server/assets/js-api/api/fetcher.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/api/fetcher.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/api/protocol.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/api/protocol.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/api/serverConn.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/api/serverConn.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/api/serverWebsocketConn.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/api/serverWebsocketConn.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/api.js` & `Lires-1.8.3/lires_server/assets/js-api/api.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/components/common/fragments.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/components/common/fragments.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/components/home/bibtexUtils.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/components/home/bibtexUtils.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/components/interface.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/components/interface.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/components/store.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/components/store.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/core/dataClass.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/core/dataClass.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/core/misc.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/core/misc.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/core/tag.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/core/tag.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/state/interface.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/state/interface.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/state/store.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/state/store.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/utils/logging.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/utils/logging.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/js-api/utils/misc.d.ts` & `Lires-1.8.3/lires_server/assets/js-api/utils/misc.d.ts`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/obsidian-plugin/main.js` & `Lires-1.8.3/lires_server/assets/obsidian-plugin/main.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/obsidian-plugin/styles.css` & `Lires-1.8.3/lires_server/assets/obsidian-plugin/styles.css`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/LICENSE` & `Lires-1.8.3/lires_server/assets/pdf-viewer/LICENSE`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.mjs` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.mjs`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.mjs.map` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.mjs.map`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs.map` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.sandbox.mjs.map`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.worker.mjs` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.worker.mjs`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/build/pdf.worker.mjs.map` & `Lires-1.8.3/lires_server/assets/pdf-viewer/build/pdf.worker.mjs.map`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/78ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/83pv-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/83pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90msp-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/90pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Add-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-UCS2.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-CNS1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-4.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-4.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-5.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-5.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-UCS2.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-GB1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-UCS2.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Japan1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-UCS2.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Adobe-Korea1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/B5pc-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/B5pc-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS-EUC-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/CNS1-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/CNS1-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETHK-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/ETen-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/Ext-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GB-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GB-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBK2K-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBKp-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBT-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBT-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBTpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/GBpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdla-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKdlb-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKgccs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm314-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKm471-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/HKscs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSC-Johab-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCms-UHC-HW-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/KSCpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/LICENSE` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/LICENSE`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/NWP-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/NWP-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniCNS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniGB-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJIS2004-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-HW-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UTF8-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISPro-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX0213-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-V.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniJISX02132004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-H.bcmap` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/cmaps/UniKS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/compressed.tracemonkey-pldi-09.pdf` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/compressed.tracemonkey-pldi-09.pdf`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/debugger.css` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/debugger.css`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/debugger.mjs` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/debugger.mjs`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/altText_add.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/altText_add.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/altText_done.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/altText_done.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-comment.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-help.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-key.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-note.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-paperclip.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-paperclip.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-paragraph.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/annotation-pushpin.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/annotation-pushpin.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeHighlight.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeHighlight.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeText.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorFreeText.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorInk.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorInk.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/cursor-editorTextHighlight.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/cursor-editorTextHighlight.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/editor-toolbar-delete.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/editor-toolbar-delete.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/findbarButton-next.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/findbarButton-next.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/findbarButton-previous.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/findbarButton-previous.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/gv-toolbarButton-download.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/gv-toolbarButton-download.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/loading-icon.gif` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/loading.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/loading.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-handTool.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-handTool.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCcw.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCcw.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCw.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-rotateCw.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollHorizontal.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollHorizontal.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollPage.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollPage.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollVertical.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollVertical.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollWrapped.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-scrollWrapped.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-selectTool.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-selectTool.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadEven.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadEven.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadOdd.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/secondaryToolbarButton-spreadOdd.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-bookmark.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-bookmark.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-currentOutlineItem.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-currentOutlineItem.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-download.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-download.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorHighlight.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorHighlight.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorInk.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorInk.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorStamp.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-editorStamp.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-menuArrow.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-menuArrow.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-openFile.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-openFile.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageDown.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageDown.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageUp.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-pageUp.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-presentationMode.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-presentationMode.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-print.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-print.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-search.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-search.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-secondaryToolbarToggle.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-secondaryToolbarToggle.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-sidebarToggle.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-sidebarToggle.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewAttachments.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewAttachments.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewLayers.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewLayers.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewThumbnail.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-viewThumbnail.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomIn.svg` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/images/toolbarButton-zoomIn.svg`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ach/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ach/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/af/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/af/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/an/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/an/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ar/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ar/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ast/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ast/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/az/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/az/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/be/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/be/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bg/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bg/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bn/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bn/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bo/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bo/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/br/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/br/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/brx/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/brx/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/bs/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/bs/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ca/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ca/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cak/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cak/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ckb/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ckb/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cs/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cs/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/cy/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/cy/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/da/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/da/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/de/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/de/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/dsb/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/dsb/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/el/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/el/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-CA/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-CA/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-GB/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-GB/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/en-US/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/en-US/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eo/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eo/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-AR/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-AR/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-CL/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-CL/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-ES/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-ES/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/es-MX/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/es-MX/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/et/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/et/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/eu/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/eu/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fa/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fa/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ff/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ff/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fi/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fi/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fur/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fur/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/fy-NL/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/fy-NL/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ga-IE/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ga-IE/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gd/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gd/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gn/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gn/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/gu-IN/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/gu-IN/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/he/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/he/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hi-IN/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hi-IN/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hsb/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hsb/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hu/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hu/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hy-AM/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hy-AM/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/hye/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/hye/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ia/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ia/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/id/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/id/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/is/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/is/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/it/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/it/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ja/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ja/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ka/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ka/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kab/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kab/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kk/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kk/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/km/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/km/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/kn/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/kn/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ko/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ko/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lij/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lij/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lo/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lo/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/locale.json` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/locale.json`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lt/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lt/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ltg/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ltg/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/lv/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/lv/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/meh/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/meh/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mk/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mk/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/mr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/mr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ms/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ms/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/my/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/my/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nb-NO/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nb-NO/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ne-NP/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ne-NP/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/nn-NO/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/nn-NO/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/oc/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/oc/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pa-IN/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pa-IN/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-BR/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-BR/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/pt-PT/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/pt-PT/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/rm/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/rm/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ro/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ro/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ru/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ru/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sat/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sat/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sc/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sc/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/scn/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/scn/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sco/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sco/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/si/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/si/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sk/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sk/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/skr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/skr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/son/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/son/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sq/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sq/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/sv-SE/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/sv-SE/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/szl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/szl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ta/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ta/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/te/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/te/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tg/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tg/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/th/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/th/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tl/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tl/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/tr/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/tr/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/trs/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/trs/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uk/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uk/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/ur/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/ur/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/uz/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/uz/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/vi/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/vi/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/wo/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/wo/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/xh/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/xh/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-CN/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-CN/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/locale/zh-TW/viewer.ftl` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/locale/zh-TW/viewer.ftl`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitDingbats.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitDingbats.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixed.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixed.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBold.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBold.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBoldItalic.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedBoldItalic.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedItalic.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitFixedItalic.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerif.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerif.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBold.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBold.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBoldItalic.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifBoldItalic.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifItalic.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSerifItalic.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSymbol.pfb` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/FoxitSymbol.pfb`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_FOXIT` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_FOXIT`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_LIBERATION` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LICENSE_LIBERATION`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Bold.ttf` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-BoldItalic.ttf` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Italic.ttf` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Regular.ttf` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/standard_fonts/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.css` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.css`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.html` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.html`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.mjs` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.mjs`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/assets/pdf-viewer/web/viewer.mjs.map` & `Lires-1.8.3/lires_server/assets/pdf-viewer/web/viewer.mjs.map`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/__init__.py` & `Lires-1.8.3/lires_server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/_base.py` & `Lires-1.8.3/lires_server/handlers/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 import json
 
 import http.cookies
 from ._global_data import GlobalStorage
 from lires.user import UserInfo
 from lires.core.base import LiresBase
 from lires.core.dataTags import DataTags
+from lires.core.vector import updateFeture, deleteFeature
 from lires.utils import BCOLORS
 
 from abc import abstractmethod
 
 from ..types import Event
 if TYPE_CHECKING:
     from .websocket import WebsocketHandler
-    from lires.core.dataClass import DataBase
-    from tiny_vectordb import VectorDatabase
+    from lires.core.dataClass import DataBase, DataPoint
+    from lires.vector.database import VectorDatabase
 
 T = TypeVar("T")
 FuncT = TypeVar("FuncT", bound=Callable)
 def authenticate(
     admin_required: bool = False,
     ) -> Callable[[FuncT], FuncT]:
     def _authenticate(func: FuncT) -> FuncT:
@@ -188,14 +189,30 @@
         # update the last active time
         await res.refreshActiveTime()
         
         # Set a cached permission, requires it via property
         user_info = await res.info()
         self.__account_info = user_info
         return user_info
+
+    async def ensureFeatureUpdate(self, dp: DataPoint):
+        """
+        Ensure the feature is updated
+        """
+        vec_db = await self.vec_db()
+        asyncio.ensure_future(updateFeture(vec_db, self.iconn, dp))
+        await self.logger.debug(f"Feature update for {dp.uuid}")
+    
+    async def deleteFeature(self, dp: DataPoint):
+        """
+        Delete the feature
+        """
+        vec_db = await self.vec_db()
+        await deleteFeature(vec_db, dp)
+        await self.logger.debug(f"Feature deleted for {dp.uuid}")
     
     @staticmethod
     async def checkTagPermission(_tags: List[str] | DataTags, _mandatory_tags: List[str], raise_error=True) -> bool:
         """
         Check if tags are dominated by mandatory_tags
         """
         tags = DataTags(_tags)
```

### Comparing `Lires-1.8.2/lires_server/handlers/_global_data.py` & `Lires-1.8.3/lires_server/handlers/_global_data.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/apiFiles.py` & `Lires-1.8.3/lires_server/handlers/apiFiles.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/dataFeature.py` & `Lires-1.8.3/lires_server/handlers/dataFeature.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     @authenticate()
     async def get(self, collection_name: str):
         n_components = self.get_argument("n_components", default="3")
         perplexity = self.get_argument("perplexity", default="-1")
         random_state = self.get_argument("random_state", default="100")
 
         try:
-            vector_collection = (await self.vec_db()).getCollection(collection_name)
+            vector_collection = await (await self.vec_db()).getCollection(collection_name)
         except KeyError:
             raise tornado.web.HTTPError(405, f"Collection {collection_name} not found")
         
-        _all_ids = vector_collection.keys()
-        all_feat = vector_collection.getBlock(_all_ids)
+        _all_ids = await vector_collection.keys()
+        all_feat = [(await vector_collection.get(uid))["vector"] for uid in _all_ids]
         if len(all_feat) < 5:
             return self.write(json.dumps({}))
 
         _feature_signature = hash(str(all_feat) + str(n_components) + str(random_state) + str(perplexity))
         for _old_signature, val in self.__class__.feat_3d_all:
             if _old_signature==_feature_signature:
                 await self.logger.debug("Use cached feature.")
```

### Comparing `Lires-1.8.2/lires_server/handlers/dataInfo.py` & `Lires-1.8.3/lires_server/handlers/dataInfo.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/dataMan.py` & `Lires-1.8.3/lires_server/handlers/dataMan.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Data management / manipulation handlers
 This are handlers to (partially) replace the file handlers in lires/server/handlers/file.py
 Provides handers for adding, deleting, and modifying files/tags
 """
 
 from ._base import *
-import json
+import json, asyncio
 from lires.core.bibReader import checkBibtexValidity, BibConverter
 from lires.core.fileTools import addDocument
 from lires.core.dataTags import DataTags
 
 class DataDeleteHandler(RequestHandlerBase):
 
     @authenticate()
@@ -18,15 +18,16 @@
         uuid = self.get_argument("uuid")
         db = await self.db()
         # check tag permission
         if not (await self.userInfo())["is_admin"]:
             await self.checkTagPermission(
                 (await db.get(uuid)).tags, (await self.userInfo())["mandatory_tags"]
                 )
-
+        
+        await self.deleteFeature(await db.get(uuid))
         if await db.delete(uuid):
             await self.logger.info(f"Deleted {uuid}")
         
         await self.broadcastEventMessage({
             'type': 'delete_entry',
             'uuid': uuid, 
             'datapoint_summary': None
@@ -148,15 +149,18 @@
             await self.broadcastEventMessage({
                 'type': 'update_entry',
                 'uuid': uuid,
                 'datapoint_summary': dp.summary.json()
             })
 
         await self.logger.info(", ".join(__info))
+
         self.write(json.dumps(dp.summary.json()))
+        await self.ensureFeatureUpdate(dp)
+
         return 
 
 class TagRenameHandler(RequestHandlerBase):
     @authenticate()
     async def post(self):
         """
         Rename a tag
```

### Comparing `Lires-1.8.2/lires_server/handlers/databaseInfo.py` & `Lires-1.8.3/lires_server/handlers/databaseInfo.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/documents.py` & `Lires-1.8.3/lires_server/handlers/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
                 raise tornado.web.HTTPError(400, reason="File extension not allowed")
         
         # add the file to the document
         if not await dp.fm.addFileBlob(file_data, ext):
             raise tornado.web.HTTPError(409, reason="File already exists")
 
         dp = await db.get(uid)
+        await self.ensureFeatureUpdate(dp)
         d_summary = dp.summary.json()
         await self.logger.info(f"Document {uid} added")
         await self.broadcastEventMessage({
             "type": 'update_entry',
             'uuid': uid,
             'datapoint_summary': d_summary
         })
```

### Comparing `Lires-1.8.2/lires_server/handlers/feed.py` & `Lires-1.8.3/lires_server/handlers/feed.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/fileinfo_supp.py` & `Lires-1.8.3/lires_server/handlers/fileinfo_supp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Get and modify notes of a datapoint
 """
 from ._base import *
+import asyncio
 
 class NoteGetHandler(RequestHandlerBase):
     """
     Get notes of a datapoint
     """
     async def get(self, uid:str):
         """
@@ -90,8 +91,9 @@
 
         await dp.fm.writeAbstract(abstract)
         await self.broadcastEventMessage({
             'type': 'update_entry',
             'uuid': uid,
             'datapoint_summary': dp.summary.json()
         })
+        await self.ensureFeatureUpdate(dp)
         self.write("OK")
```

### Comparing `Lires-1.8.2/lires_server/handlers/iServerProxy.py` & `Lires-1.8.3/lires_server/handlers/iServerProxy.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/misc.py` & `Lires-1.8.3/lires_server/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/miscFiles.py` & `Lires-1.8.3/lires_server/handlers/miscFiles.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/pdfjs.py` & `Lires-1.8.3/lires_server/handlers/pdfjs.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/search.py` & `Lires-1.8.3/lires_server/handlers/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,18 +76,18 @@
                     res.append(uid)
         
         elif search_by == 'feature':
             q_res = await queryFeatureIndex(
                 iconn=self.iconn,
                 query=search_content,
                 n_return=top_k,
-                vector_collection= (await self.vec_db()).getCollection("doc_feature")
+                vector_collection= await (await self.vec_db()).getCollection("doc_feature")
             )
-            res_ = q_res["uids"]
-            scores_ = q_res["scores"]
+            res_ = [x["entry"]["uid"] for x in q_res]
+            scores_ = [x["score"] for x in q_res]
             if cadidate_ids is not None:
                 candidate_set = set(cadidate_ids)    # convert to set may be faster?
                 res = []
                 scores = []
                 for uid, score in zip(res_, scores_):
                     if uid in candidate_set:
                         res.append(uid)
```

### Comparing `Lires-1.8.2/lires_server/handlers/summary.py` & `Lires-1.8.3/lires_server/handlers/summary.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/user.py` & `Lires-1.8.3/lires_server/handlers/user.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/userMan.py` & `Lires-1.8.3/lires_server/handlers/userMan.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_server/handlers/websocket.py` & `Lires-1.8.3/lires_server/handlers/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                 'type': 'logout',
                 'username': (await self.userInfo())['username'],
                 'user_info': await self.userInfoDesensitized(),
             }, to_all=True)
             try:
                 # unregister from global connection pool
                 self.connection_pool.remove(self)
-            except IndexError:
+            except (IndexError, ValueError):
                 await self.logger.error("WebSocket connection not found in connection pool, skipped")
         tornado.ioloop.IOLoop.current().add_callback(_on_close)
 
     async def on_message(self, message):
         # TODO: to deal with user interactions
         await self.logger.debug(f"WebSocket message: {message}")
         pass
```

### Comparing `Lires-1.8.2/lires_server/main.py` & `Lires-1.8.3/lires_server/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 NoCacheStaticFileHandler = cachedStaticFileHandlerFactory(0)
 class Application(tornado.web.Application):
     def __init__(self, debug = False) -> None:
         handlers = [
             # Frontend
             (r'/()', NoCacheStaticFileHandler, {"path": LRSWEB_SRC_ROOT, "default_filename": "index.html"}),
             (r'/(index.html)', NoCacheStaticFileHandler, {"path": LRSWEB_SRC_ROOT}),
-            (r'/(favicon.ico)', NoCacheStaticFileHandler, {"path": LRSWEB_SRC_ROOT}),
-            (r'/(assets/.*)', NoCacheStaticFileHandler, {"path": LRSWEB_SRC_ROOT}),
+            (r'/(favicon.ico)', cachedStaticFileHandlerFactory(600), {"path": LRSWEB_SRC_ROOT}),
+            (r'/(assets/.*)', cachedStaticFileHandlerFactory(600), {"path": LRSWEB_SRC_ROOT}),
+            (r'/(site-icons/.*)', cachedStaticFileHandlerFactory(600), {"path": LRSWEB_SRC_ROOT}),
+            (r'/(site.manifest.json)', cachedStaticFileHandlerFactory(600), {"path": LRSWEB_SRC_ROOT}),
 
             # access server assets, read-only
             (r'/documentation/(.*)', cachedStaticFileHandlerFactory(cache_seconds=600), 
                 {"path": os.path.join(ASSETS_DIR, 'docs'), 'default_filename': 'index.html'}
             ),
             (r"/pdfjs/(.*)", PdfJsHandler, {"path": PdfJsHandler.root_dir}),
             (r"/_resources/api.zip", APIGetHandler_JS),
@@ -103,16 +105,14 @@
 
             # iServer proxy
             (r"/api/iserver/(.*)", IServerProxyHandler),
 
             # data management
             (r"/api/dataman/delete", DataDeleteHandler),
             (r"/api/dataman/update", DataUpdateHandler),
-            (r"/api/dataman/tag-rename", TagRenameHandler),     # keep for compatibility, will remove in v1.8.0
-            (r"/api/dataman/tag-delete", TagDeleteHandler),     # keep for compatibility, will remove in v1.8.0
 
             # user
             (r"/api/user/list", UserListHandler),
             (r"/api/user/info/(.*)", UserInfoHandler),
             (r"/api/user/info-update", UserInfoUpdateHandler),
             (r"/api/userman/create", UserCreateHandler),
             (r"/api/userman/delete", UserDeleteHandler),
@@ -169,19 +169,18 @@
         from lires.core.vector import buildFeatureStorage
 
         for db_ins in g_storage.database_pool:
             await buildFeatureStorage(
                 iconn = g_storage.iconn,
                 db = db_ins.database,
                 vector_db = db_ins.vector_db,
-                use_llm = False,
                 operation_interval=op_interval,
             )
     
-    tornado.ioloop.PeriodicCallback(buildIndex, 12*60*60*1000).start()  # in milliseconds
+    tornado.ioloop.PeriodicCallback(buildIndex, 6*60*60*1000).start()   # in milliseconds
     tornado.ioloop.PeriodicCallback(g_storage.flush, 5*1000).start()    # periodically flush the database
 
     # exit hooks
     import signal
     async def __exitHook():
         await g_storage.finalize()
         await RequestHandlerBase.logger.info("Server shutdown")
```

### Comparing `Lires-1.8.2/lires_server/types.py` & `Lires-1.8.3/lires_server/types.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/ai/cmd/summarize.py` & `Lires-1.8.3/lires_service/ai/cmd/summarize.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/ai/globalConfig.py` & `Lires-1.8.3/lires_service/ai/globalConfig.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/ai/lmInterface.py` & `Lires-1.8.3/lires_service/ai/lmInterface.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/ai/lmTools.py` & `Lires-1.8.3/lires_service/ai/lmTools.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/ai/server.py` & `Lires-1.8.3/lires_service/ai/server.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/entry.py` & `Lires-1.8.3/lires_service/entry.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/log/logger.py` & `Lires-1.8.3/lires_service/log/logger.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/log/server.py` & `Lires-1.8.3/lires_service/log/server.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/registry/server.py` & `Lires-1.8.3/lires_service/registry/server.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_service/registry/store.py` & `Lires-1.8.3/lires_service/registry/store.py`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/@codemirror-4Zn9bE8B.js` & `Lires-1.8.3/lires_web/dist/assets/@codemirror-4Zn9bE8B.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/@lezer-tqr6QOpM.js` & `Lires-1.8.3/lires_web/dist/assets/@lezer-tqr6QOpM.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/@vavt-DtLj4T47.js` & `Lires-1.8.3/lires_web/dist/assets/@vavt-DtLj4T47.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/@vue-D_lT-ze_.js` & `Lires-1.8.3/lires_web/dist/assets/@vue-D_lT-ze_.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/async-mutex-CSJywVGb.js` & `Lires-1.8.3/lires_web/dist/assets/async-mutex-CSJywVGb.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/copy-to-clipboard-B1uT6SkR.js` & `Lires-1.8.3/lires_web/dist/assets/copy-to-clipboard-B1uT6SkR.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/crelt-C8TCjufn.js` & `Lires-1.8.3/lires_web/dist/assets/crelt-C8TCjufn.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/cssfilter-BjxKUPhv.js` & `Lires-1.8.3/lires_web/dist/assets/cssfilter-BjxKUPhv.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/entities-C20TfXL6.js` & `Lires-1.8.3/lires_web/dist/assets/entities-C20TfXL6.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/fast-xml-parser-CJG3bOwu.js` & `Lires-1.8.3/lires_web/dist/assets/fast-xml-parser-CJG3bOwu.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/gray-matter-D4hcLa5V.js` & `Lires-1.8.3/lires_web/dist/assets/gray-matter-D4hcLa5V.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/index-DVZewPDh.js` & `Lires-1.8.3/lires_web/dist/assets/index-Tvuvqxrm.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5964,28 +5964,28 @@
             }
         },
         emits: ["register-success", "register-fail"],
         components: {
             SwitchToggle: Te
         },
         methods: {
-            submitForm() {
+            submitForm(o) {
                 if (this.password !== this.passwordConfirm) {
                     this.$emit("register-fail", "Passwords do not match");
                     return
                 }
                 ee().conn.registerUser(this.invitationCode, this.username, this.password, this.name).then(() => {
                     this.$emit("register-success")
-                }, o => {
-                    o.message.includes("409") ? this.$emit("register-fail", "Username already exists") : o.message.includes("401") ? this.$emit("register-fail", "Invalid invitation code") : o.message.includes("403") ? this.$emit("register-fail", "Invitation code expired") : o.message.includes("507") ? this.$emit("register-fail", "Maximum number of users reached") : this.$emit("register-fail", o)
-                })
+                }, t => {
+                    t.message.includes("409") ? this.$emit("register-fail", "Username already exists") : t.message.includes("401") ? this.$emit("register-fail", "Invalid invitation code") : t.message.includes("403") ? this.$emit("register-fail", "Invitation code expired") : t.message.includes("507") ? this.$emit("register-fail", "Maximum number of users reached") : this.$emit("register-fail", t)
+                }), o.preventDefault()
             }
         }
     },
-    $e = o => (se("data-v-74eb04e9"), o = o(), ie(), o),
+    $e = o => (se("data-v-892e7367"), o = o(), ie(), o),
     yl = {
         id: "form-container"
     },
     wl = {
         class: "form-elem"
     },
     bl = $e(() => n("div", {
@@ -6080,15 +6080,15 @@
     ]), Rl])]), n("div", Al, [k(r, {
         checked: s.showPassword,
         "onUpdate:checked": t[5] || (t[5] = l => s.showPassword = l)
     }, null, 8, ["checked"]), Ml]), Bl], 32)
 }
 const ql = E(_l, [
         ["render", Ll],
-        ["__scopeId", "data-v-74eb04e9"]
+        ["__scopeId", "data-v-892e7367"]
     ]),
     El = {
         id: "login-main"
     },
     Fl = {
         id: "container"
     },
```

### Comparing `Lires-1.8.2/lires_web/dist/assets/index-Umoxfe5H.css` & `Lires-1.8.3/lires_web/dist/assets/index-Bzo7HIUU.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-@keyframes popupGradIn-7a7b12ca{0%{visibility:hidden;opacity:0}to{visibility:visible}}#popup[data-v-7a7b12ca]{position:fixed;z-index:100;display:flex;flex-direction:column;align-items:center;justify-content:center;box-shadow:0 1px 3px 3px var(--color-shadow);border-radius:10px;padding:10px;animation:popupGradIn-7a7b12ca .25s ease-in-out}.loading-widget[data-v-1d6933bb]{display:flex;align-items:center;justify-content:center;height:100%}.loading-widget__spinner[data-v-1d6933bb]{border-radius:50%;animation:spin-1d6933bb 1s ease-in-out infinite}@keyframes spin-1d6933bb{to{transform:rotate(360deg)}}div.loading-popout[data-v-95a13423]{position:absolute;bottom:0;right:0;padding:10px;width:240px;margin:20px;display:flex;flex-direction:row;align-items:center;justify-content:center;gap:10px;border:1px solid var(--color-border);border-radius:5px;box-shadow:0 1px 2px 0 var(--color-shadow);z-index:99;background-color:var(--color-background-theme-thin)}#app[data-v-934929d5]{margin:0;padding:0}:root{--vt-c-white: #f2f2f2;--vt-c-white-soft: #e3e3e3;--vt-c-white-mute: rgb(228, 228, 228);--vt-c-black: #1f1f1f;--vt-c-black-soft: #303030;--vt-c-black-mute: #3f3f3f;--vt-c-indigo: #2c3e50;--vt-c-divider-light-1: rgba(60, 60, 60, .29);--vt-c-divider-light-2: rgba(60, 60, 60, .12);--vt-c-divider-dark-1: rgba(90, 90, 90, .65);--vt-c-divider-dark-2: rgba(90, 90, 90, .48);--vt-c-text-light-1: var(--vt-c-indigo);--vt-c-text-light-2: rgba(60, 60, 60, .66);--vt-c-text-dark-1: var(--vt-c-white);--vt-c-text-dark-2: rgba(235, 235, 235, .64)}:root,:root.light{--section-gap: 160px;--color-background: var(--vt-c-white);--color-background-soft: var(--vt-c-white-soft);--color-background-mute: var(--vt-c-white-mute);--color-background-darker: var(--vt-c-white-mute);--color-background-lighter: var(--vt-c-white);--color-border: var(--vt-c-divider-light-2);--color-border-hover: var(--vt-c-divider-light-1);--color-heading: var(--vt-c-text-light-1);--color-text: var(--vt-c-text-light-1);--color-shadow: rgba(0, 0, 0, .12)}:root.dark{--color-background: var(--vt-c-black);--color-background-soft: var(--vt-c-black-soft);--color-background-mute: var(--vt-c-black-mute);--color-background-darker: var(--vt-c-black);--color-background-lighter: var(--vt-c-black-mute);--color-border: var(--vt-c-divider-dark-2);--color-border-hover: var(--vt-c-divider-dark-1);--color-heading: var(--vt-c-text-dark-1);--color-text: var(--vt-c-text-dark-2);--color-shadow: rgba(0, 0, 0, .3)}:root{--color-red-transparent: rgba(200, 50, 80, .084);--color-red: rgb(200, 50, 80);--color-danger: rgb(200, 50, 80);--color-danger-hover: rgba(200, 50, 80, .2)}:root,:root.light{--color-pure: #fff;--color-theme: rgb(82, 153, 182);--color-text-soft: rgba(80, 80, 80, .5);--color-background-ssoft: #e8e8e8;--color-background-theme-highlight: rgba(137, 189, 213, .2);--color-background-theme-thin: #dbdee5;--color-background-theme: rgba(127, 178, 220, .3);--color-background-tagpanel: #efefef;--color-progressbar: #007bff;--color-background-progressbar: #f4f4f4}:root.dark{--color-pure: #000;--color-theme: rgb(80, 180, 200);--color-text-soft: rgba(180, 180, 180, .5);--color-background-ssoft: #2c2c2c;--color-background-theme-highlight: rgba(108, 186, 185, .2);--color-background-theme-thin: #383b41;--color-background-theme: rgba(52, 84, 93, .3);--color-background-tagpanel: #232323;--color-progressbar: #0e58a8;--color-background-progressbar: #202020}*,*:before,*:after{box-sizing:border-box;margin:0;position:relative;font-weight:400}body{color:var(--color-text);background:var(--color-background);transition:color .5s,background-color .5s;line-height:1.6;font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:15px;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}@keyframes slideInUpAnim{0%{visibility:hidden;transform:translateY(5%);opacity:0}to{visibility:visible;transform:translateY(0)}}@keyframes slideInDownAnim{0%{visibility:hidden;transform:translateY(-5%);opacity:0}to{visibility:visible;transform:translateY(0)}}@keyframes slideInBackAnim{0%{visibility:hidden}1%{transform:translateY(6%) scale(.95);opacity:0;visibility:visible}60%{transform:translateY(-4%) scale(1.01)}to{transform:translateY(0);opacity:1}}@keyframes rotate90in{0%{transform:rotate(-90deg)}to{transform:rotate(0)}}@keyframes gradInAnim{0%{opacity:0}to{opacity:1}}.gradIn{animation-duration:.3s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:gradInAnim}.slideIn{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInUpAnim}.slideInFast,.slidInFast{animation-duration:.15s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInUpAnim}.slideInDown{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInDownAnim}.slideIn2{animation-duration:.375s;animation-fill-mode:backwards;animation-timing-function:ease-out;animation-name:slideInBackAnim}.rotate90in{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:rotate90in}.hoverMaxout11:hover{transform:scale(1.1)}.hoverMaxout105:hover{transform:scale(1.05)}.hoverMaxout103:hover{transform:scale(1.03)}.hoverMaxout101:hover{transform:scale(1.01)}body{display:flex;place-items:center}#app{margin:0 auto;font-weight:400;text-align:center;align-self:center;display:flex;align-items:center;justify-content:center}a,.green{text-decoration:none;color:#089d86;transition:.4s}b{font-weight:700}@media (hover: hover){a:hover{background-color:#00bd7e33}}.shadow{box-shadow:0 1px 3px 2px var(--color-shadow)}.scrollable{overflow-y:auto;overflow-x:auto}.hover-scrollable{overflow-x:hidden;overflow-y:hidden}.hover-scrollable:hover{overflow-x:auto;overflow-y:auto}.non-selectable{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}html{--scrollbarBG: var(--color-background-soft);--thumbBG: var(--color-border)}body,.panel,.scrollable,.hover-scrollable{scrollbar-width:thin;scrollbar-color:var(--thumbBG) var(--scrollbarBG)}body::-webkit-scrollbar,.panel::-webkit-scrollbar,.scrollable::-webkit-scrollbar,.hover-scrollable::-webkit-scrollbar{width:11px}body::-webkit-scrollbar-track,.panel::-webkit-scrollbar-track,.scrollable::-webkit-scrollbar-track,.hover-scrollable::-webkit-scrollbar-track{background:var(--scrollbarBG)}body::-webkit-scrollbar-thumb,.panel::-webkit-scrollbar-thumb,.scrollable::-webkit-scrollbar-thumb,.hover-scrollable::-webkit-scrollbar-thumb{background-color:var(--thumbBG);border-radius:6px;border:3px solid var(--scrollbarBG)}input[type=text],input[type=password]{border:transparent;color:var(--color-text);height:24px;border-radius:8px;padding-left:4px;font-size:small;background-color:var(--color-background-soft);background-color:transparent}textarea{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text)}input[type=button],button{border-radius:5px;height:24px;border:1px solid var(--color-border);background-color:var(--color-background-soft);font-size:small;color:var(--color-text)}input[type=button]:hover,button:hover{background-color:var(--color-background-theme-highlight);transition:all .15s}select{border-radius:8px;border:1px solid var(--color-border);padding:2px 5px;background-color:var(--color-background-soft);background-color:transparent;color:var(--color-text);-webkit-appearance:none}div[data-v-582ee950]{--radius: 16px;--radius-inner: 6px;display:flex;align-items:center;gap:5px}div.toggle[data-v-582ee950]{justify-content:left;flex-direction:row-reverse;flex-wrap:nowrap}#checkCircle[data-v-582ee950]{border:3px solid var(--color-border);height:var(--radius);width:var(--radius);border-radius:50%;justify-content:center}#checkStatus[data-v-582ee950]{height:var(--radius-inner);width:var(--radius-inner);border-radius:50%;background-color:var(--color-theme)}#checkCircle[data-v-582ee950]:hover{background-color:var(--color-background-theme-highlight);transition:all .2s}label:hover+#checkCircle[data-v-582ee950]{background-color:var(--color-background-theme-highlight);transition:all .2s}label[data-v-582ee950]{text-align:left;text-overflow:ellipsis;overflow:clip}div[data-v-3c7d3255]{--button-dim: 16px;--triangle-dim: 8px}div.row[data-v-3c7d3255]{display:flex;align-items:center;gap:2px}div.collapseButton[data-v-3c7d3255]{width:var(--button-dim);height:var(--button-dim);min-width:var(--button-dim);min-height:var(--button-dim);border-radius:50%;display:flex;align-items:center;justify-content:center}.toggleText[data-v-3c7d3255]{flex-grow:1;margin-top:2px;margin-bottom:2px;border-radius:5px;transition:all .1s ease}.toggleText[data-v-3c7d3255]:hover{background-color:var(--color-background-theme-highlight)}.triangle-right[data-v-3c7d3255]{width:var(--triangle-dim);height:var(--triangle-dim);background-color:var(--color-theme);clip-path:polygon(0 0,0% 100%,100% 50%)}.triangle-down[data-v-3c7d3255]{width:var(--triangle-dim);height:var(--triangle-dim);background-color:var(--color-theme);clip-path:polygon(0 0,100% 0%,50% 100%)}div.children[data-v-3c7d3255]{margin-left:20px}#tagSelector-main[data-v-f90dfe41]{flex-grow:1}div.bubble[data-v-f454bc70]{padding:3px 5px;text-align:left;border-radius:7px;background-color:var(--color-background-soft);transition:all .2s;font-size:small;display:flex;justify-content:center;align-items:center;cursor:default}div.highlight[data-v-f454bc70]{background-color:#f836ff3f;box-shadow:0 0 5px var(--color-shadow)}div.muted[data-v-f454bc70]{opacity:.35}div.prefix[data-v-f454bc70]{padding:3px;background-color:var(--color-background-theme-thin);font-size:x-small;color:var(--color-text-theme);border-radius:3px;margin-right:5px}div#bubbleContainer[data-v-62e107cd]{display:flex;flex-wrap:wrap;align-items:center;gap:5px;padding:5px;border-radius:5px;overflow:visible}div#title-title[data-v-9523b989]{margin-left:5px;display:flex;justify-content:space-between;align-items:center}div#title-title h3[data-v-9523b989]{text-align:left;font-weight:700;color:var(--color-theme)}div#title-buttons[data-v-9523b989]{display:flex;gap:5px;opacity:.15;transition:opacity .5s;transition-delay:opacity .2s}div#title-buttons div.button[data-v-9523b989]:hover{text-decoration:underline;text-underline-offset:2px}div#title-buttons div.button[data-v-9523b989]{transition:all .2s;padding-left:5px;padding-right:5px;font-size:smaller;border-radius:5px;cursor:pointer}div#title-title:hover div#title-buttons[data-v-9523b989]{opacity:1}hr[data-v-9523b989]{margin-top:5px;border:1px solid var(--color-border);border-top:none}div#file-tags-main[data-v-9523b989]{padding:15px 10px;min-width:260px;width:fit-content;height:100%;display:flex;flex-direction:column;justify-content:space-between;border-radius:10px 0 0 10px;border:1px solid var(--color-border);border-top:none;border-left:none;border-bottom:none;background-color:var(--color-background-tagpanel);gap:10px}div.buttons[data-v-9523b989]{padding-left:5px;padding-right:5px}#btnClear[data-v-9523b989]{padding:5px;width:100%;border:0px solid var(--color-border);font-weight:700}@keyframes floatingWindowGradIn-c6dbcdc2{0%{visibility:hidden;transform:scale(.9);opacity:0}to{visibility:visible}}div#blocker[data-v-c6dbcdc2]{position:fixed;top:0;left:0;width:100vw;height:100%;background-color:#00000080;display:flex;justify-content:center;align-items:center}div.header[data-v-c6dbcdc2]{display:flex;flex-direction:row;justify-content:space-between;align-items:center;width:100%;padding:10px}.header label[data-v-c6dbcdc2],.header span[data-v-c6dbcdc2]{font-size:x-small;color:var(--color-text);opacity:.5}.header label[data-v-c6dbcdc2]{text-align:left}.floating-window[data-v-c6dbcdc2]{background-color:var(--color-background-soft);border:1px solid var(--color-border);border-radius:5px;display:flex;flex-direction:column;align-items:flex-start;box-shadow:0 1px 3px 2px var(--color-shadow);animation-duration:.1s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:floatingWindowGradIn-c6dbcdc2}.window-content[data-v-c6dbcdc2]{max-width:calc(100vw - 50px);max-height:calc(100vh - 80px);overflow:auto}.close-button[data-v-c6dbcdc2]{min-width:2.6em;width:2.6em;height:1.8em;align-self:flex-start;background:none;border:1px solid var(--color-border);border-radius:.75em;cursor:pointer;padding:0;display:flex;align-items:center;justify-content:center}.close-button[data-v-c6dbcdc2]:hover{background-color:#c832504d;transition:all .2s}.close-icon[data-v-c6dbcdc2]{margin:0;font-size:medium;font-weight:700}div#query-dialog-main[data-v-81948a9f]{display:flex;flex-direction:column;height:100%}div#buttons[data-v-81948a9f]{display:flex;flex-direction:row;justify-content:space-around;margin-top:10px;border-top:1px solid var(--color-border)}div.button[data-v-81948a9f]{display:flex;justify-content:center;align-items:center;width:100%;padding:5px;cursor:pointer;background-color:var(--color-background-soft)}div.button[data-v-81948a9f]:hover{box-shadow:inset 0 0 5px 1px var(--color-shadow)}div.ok-button[data-v-81948a9f]:hover{background-color:var(--color-background-theme-highlight)}div.cancel-button[data-v-81948a9f]:hover{background-color:var(--color-danger-hover)}div.last-button[data-v-81948a9f]{border-left:1px solid var(--color-border)}div#tag-selector-with-entry-main[data-v-990ad4c4]{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;width:100%;height:100%;gap:10px}textarea[data-v-990ad4c4],input[type=text][data-v-990ad4c4],div#tagSelector[data-v-990ad4c4]{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text);width:100%}div#tagSelector[data-v-990ad4c4]{min-width:300px;height:420px;padding:5px}label[data-v-990ad4c4]{font-weight:700}input[type=text][data-v-990ad4c4]{border:1px solid var(--color-border);border-radius:5px}div.entry[data-v-990ad4c4]{display:flex;flex-direction:row;align-items:center;width:100%;gap:5px}button[data-v-990ad4c4]{width:80px;cursor:pointer}button.to-be-confirmed[data-v-990ad4c4]{color:#ff0096;background-color:#00ffa6bf}div#blocker[data-v-c6b659c7]{position:fixed;top:0;left:0;width:100vw;height:100%;background-color:#00000080}#arrow[data-v-c6b659c7]{position:absolute;top:-10px;left:50%;margin-left:-10px;width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-bottom:10px solid var(--color-background-soft)}#floatingMenu[data-v-c6b659c7]{position:fixed;z-index:101;background-color:var(--color-background-soft);border:1px solid var(--color-border);border-radius:5px;box-shadow:0 1px 3px 2px var(--color-shadow)}.floatingMenuItem[data-v-c6b659c7]{cursor:pointer;padding:5px 15px;border-bottom:1px solid var(--color-border)}.floatingMenuItemLast[data-v-c6b659c7]{border-bottom:none}.floatingMenuItem[data-v-c6b659c7]:hover{background-color:var(--color-background-theme-highlight)}#inputDiv[data-v-e295a40e]{display:flex;flex-direction:row;width:100%;gap:10px;padding-left:15px;padding-right:15px}div.hr[data-v-e295a40e]{width:100%;height:1px;background-color:var(--color-border)}label[data-v-e295a40e]{font-weight:700}div.horizontal[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:10px;width:100%}div#bibtexSource[data-v-e295a40e]{font-size:small;margin-left:10px}div#bibtexSource div.button[data-v-e295a40e]{cursor:pointer;opacity:.2;transition:all .2s ease-in-out}div#bibtexSource div.button[data-v-e295a40e]:hover{cursor:pointer;opacity:1;color:var(--color-theme);text-decoration:underline}#inputLeft[data-v-e295a40e],#inputRight[data-v-e295a40e]{display:flex;flex-direction:column;width:100%;gap:10px}textarea[data-v-e295a40e],input[type=text][data-v-e295a40e]{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text);width:100%}div#bibtexArea[data-v-e295a40e]{display:flex;flex-direction:column;align-items:flex-start}div#bibtexArea textarea[data-v-e295a40e]{min-width:300px;width:100%;height:420px;padding:5px;font-size:medium;font-family:monospace}.wrapword[data-v-e295a40e]{white-space:-moz-pre-wrap!important;white-space:-webkit-pre-wrap;white-space:-pre-wrap;white-space:-o-pre-wrap;white-space:pre-wrap;word-wrap:break-word;word-break:break-all}div#urlArea[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:5px}div#urlArea>input[type=text][data-v-e295a40e]{width:100%}div#tagSelector[data-v-e295a40e]{width:100%;min-width:300px;height:420px;overflow:scroll;padding:5px}button#addNewTag[data-v-e295a40e]{width:80px}div.bibsource-container[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:5px}.layout[data-v-9b2c5a9d]{display:flex;flex-direction:column;justify-content:center;align-items:center;gap:20px}#info[data-v-9b2c5a9d]{width:100%;display:flex;flex-direction:column;justify-content:center;align-items:flex-start;text-align:left}b[data-v-9b2c5a9d]{font-weight:700}#shortSummary[data-v-9b2c5a9d]{display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:left}#shortSummaryTitle[data-v-9b2c5a9d]{display:flex;flex-direction:row;justify-content:flex-start;align-items:center;gap:10px}.button[data-v-9b2c5a9d]{cursor:pointer;border-radius:3px}.button[data-v-9b2c5a9d]:hover{background-color:var(--color-background-theme-highlight)}details[data-v-9b2c5a9d]{width:100%}table[data-v-9b2c5a9d]{width:100%}td[data-v-9b2c5a9d]{vertical-align:top;padding-left:5px;padding-right:5px}td#authorTD[data-v-9b2c5a9d]{display:flex;flex-direction:row;justify-content:flex-start;align-items:flex-start;flex-wrap:wrap;gap:10px}td#authorTD div[data-v-9b2c5a9d]{display:block}tr#otherPubTR td[data-v-9b2c5a9d]{width:100%;padding:10px;border-radius:10px;border:1px solid var(--color-border);background-color:var(--color-background-mute)}.slideDown-enter-active[data-v-9b2c5a9d],.slideDown-leave-active[data-v-9b2c5a9d]{transition:all .15s ease}.slideDown-enter-from[data-v-9b2c5a9d],.slideDown-leave-to[data-v-9b2c5a9d]{transform:translateY(-10%);opacity:0}hr[data-v-564cf261]{margin:10px;border:1px solid var(--color-border)}div.row[data-v-564cf261]{display:flex;align-items:center;justify-content:center}div#moreMain[data-v-564cf261]{display:flex;flex-direction:column;align-items:center;justify-content:center;margin-top:8px;margin-bottom:10px;overflow-y:hidden}div#buttons[data-v-564cf261]{gap:10px}label.hint[data-v-564cf261]{font-size:xx-small;color:var(--color-border)}#abstract[data-v-564cf261]{max-width:1200px;text-align:justify;padding-left:10px;padding-right:10px}#abstract summary[data-v-564cf261]{font-weight:700;cursor:pointer;text-align:center}div#actions[data-v-564cf261]{gap:10px;background-color:var(--color-background-mute);margin:3px;padding-block:5px;padding-inline:50px;border-radius:20px;box-shadow:inset 0 1px 2px 0 var(--color-shadow)}[data-v-564cf261] a{cursor:pointer;border-radius:7px;padding-inline:5px;-webkit-user-select:none;user-select:none}[data-v-564cf261] a.btn{text-decoration:underline;text-underline-offset:2px;cursor:pointer}a.danger[data-v-564cf261]{color:var(--color-danger)}a.danger[data-v-564cf261]:hover{background-color:var(--color-danger-hover)}.actions-enter-active[data-v-564cf261],.actions-leave-active[data-v-564cf261]{transition:all .2s}.actions-enter-from[data-v-564cf261],.actions-leave-to[data-v-564cf261]{opacity:0;transform:translateY(-10px)}@keyframes expand-564cf261{0%{max-height:0px;opacity:0;margin:0}50%{max-height:48px;opacity:0}to{max-height:auto;opacity:1}}@keyframes contract-564cf261{0%{max-height:48px;opacity:1}50%{max-height:0px;opacity:0}to{margin:0;max-height:0px;opacity:0}}.expand-transition-enter-active[data-v-564cf261]{animation:expand-564cf261 .2s ease-in-out}.expand-transition-leave-active[data-v-564cf261]{animation:contract-564cf261 .2s ease-in-out}div.row[data-v-f2b3f69e]{display:flex;align-items:center;justify-content:flex-start;cursor:default}div#init[data-v-f2b3f69e]{display:flex;flex-wrap:nowrap;justify-content:space-between}div#init>div.left[data-v-f2b3f69e]{flex-wrap:nowrap;column-gap:5px;overflow:hidden}div#marks[data-v-f2b3f69e]:hover{cursor:pointer}div#fileRow[data-v-f2b3f69e]{border-radius:0;padding:3px;padding-inline:10px;width:100%}div.text[data-v-f2b3f69e]{padding:0;margin:0;text-align:left;text-overflow:ellipsis;overflow:hidden}div#status-container[data-v-f2b3f69e]{display:flex;flex-direction:row;align-items:center;gap:2px}div.status[data-v-f2b3f69e]{display:flex;align-items:center;justify-content:center;width:15px}img.icon[data-v-f2b3f69e]{height:15px;filter:invert(.5) opacity(.25) drop-shadow(0 0 0 var(--color-border))}img.redIcon[data-v-f2b3f69e]{filter:invert(33%) sepia(92%) saturate(3443%) hue-rotate(0deg) brightness(97%) contrast(101%)}img.placeholder[data-v-f2b3f69e]{height:8px}.more-enter-active[data-v-f2b3f69e],.more-leave-active[data-v-f2b3f69e]{transition:all .15s}.more-enter-from[data-v-f2b3f69e],.more-leave-to[data-v-f2b3f69e]{opacity:0}#title[data-v-f2b3f69e]{display:inline-block;white-space:wrap;word-break:break-word;overflow:hidden;text-overflow:ellipsis}@media (max-width: 768px){div#init>div.left[data-v-f2b3f69e]{width:100%;flex-wrap:wrap}div#init[data-v-f2b3f69e]{align-items:flex-start}div#status-container[data-v-f2b3f69e]{flex-direction:column;margin-block:5px;margin-left:5px;gap:1px}img.icon[data-v-f2b3f69e]{height:12px}img.placeholder[data-v-f2b3f69e]{height:12px;width:8px}}#datacard-container-main[data-v-006a79ab]{display:flex;flex-direction:column;align-items:center;justify-content:space-between;width:100%;height:100%;overflow-y:auto;overflow-x:hidden}#datacard-container[data-v-006a79ab]{display:flex;flex-direction:column;overflow-x:hidden;width:100%}label.relatedArticleScore[data-v-006a79ab]{border-radius:5px;padding-left:5px;padding-right:5px;display:flex;align-items:center;justify-content:center;background-color:var(--color-background-theme-highlight)}#datacard-container-footer[data-v-006a79ab]{display:flex;flex-direction:row;align-items:center;justify-content:center;width:100%;padding-block:5px;z-index:1;box-shadow:0 -0px 5px 0 var(--color-shadow)}#datacard-container-footer button[data-v-006a79ab]{border-radius:5px;padding-inline:30px;height:30px;padding-block:5px;font-weight:700;color:var(--color-text);border:none;display:flex;align-items:center;justify-content:center;transition:all .15s ease-in-out}#datacard-container-footer button[data-v-006a79ab]:hover{background-color:var(--color-background-theme-highlight);transform:scale(1.05)}#datacard-container-footer button[data-v-006a79ab]:active{transform:scale(.95)}#datacard-container-footer button[data-v-006a79ab]:disabled{color:var(--color-text-soft)}#datacard-container-footer button[data-v-006a79ab]:disabled:hover{background-color:transparent}.fade-enter-active[data-v-006a79ab],.fade-leave-active[data-v-006a79ab]{transition:all .5s ease-in-out}.fade-enter-from[data-v-006a79ab],.fade-leave-to[data-v-006a79ab]{opacity:0}span.button[data-v-f0fccbdf]{padding:3px 5px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:smaller;gap:2px}span.button[data-v-f0fccbdf]:hover{background-color:var(--color-background-theme-highlight);box-shadow:0 1px 3px 2px var(--color-shadow);transition:all .2s}img.icon[data-v-f0fccbdf]{height:20px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}@media (max-width: 600px){.iconLabel[data-v-f0fccbdf]{display:none}}#disk-usage-main[data-v-35d9044c]{display:flex;flex-direction:column;justify-content:center;align-items:flex-start;gap:0rem;width:100%;height:100%;overflow-y:auto}.disk-usage-bar[data-v-35d9044c]{width:100%;height:1rem;background-color:var(--color-background-progressbar);border-radius:5px;overflow:hidden}.disk-usage-fill[data-v-35d9044c]{height:100%;background-color:var(--color-progressbar);transition:width .3s ease-in-out}.disk-usage-text[data-v-35d9044c]{font-size:.75rem;text-align:center;height:100%;color:var(--color-text-soft);white-space:nowrap}div#usercard-main[data-v-02517de9]{margin-top:10px;display:flex;align-items:center;flex-direction:column;gap:.5rem;width:100%}div#info[data-v-02517de9]{display:flex;justify-content:center;align-items:center;flex-direction:row;gap:20px}label.admin_hint[data-v-02517de9]{font-size:x-small;padding-left:5px;padding-right:5px;height:12px;border-radius:5px;background-color:var(--color-background-theme);color:var(--color-theme)}div#info div#name-edit[data-v-02517de9]{display:flex;flex-direction:row;align-items:center;gap:10px}div#info div#user-desc[data-v-02517de9]{display:flex;flex-direction:column;align-items:flex-start;justify-self:flex-start}p#credential[data-v-02517de9]{font-family:monospace;color:var(--color-text-soft);cursor:pointer;font-size:.75rem}h1[data-v-02517de9]{font-weight:700}img.icon[data-v-02517de9]{height:25px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}img#edit-settings-icon[data-v-02517de9]{padding-top:8px;opacity:0;transition:all .2s ease-in-out}img#edit-settings-icon[data-v-02517de9]:hover{cursor:pointer}div#name-edit:hover img#edit-settings-icon[data-v-02517de9]{opacity:1}div#user-settings[data-v-02517de9]{margin:0 10px 10px;display:flex;flex-direction:column;text-align:left}div#user-settings hr[data-v-02517de9]{margin:0;padding:0}div#user-settings b[data-v-02517de9]{font-weight:700}div#user-settings input[type=text][data-v-02517de9]{width:300px;background-color:var(--color-background);height:36px}div#user-settings details summary[data-v-02517de9]{margin-top:5px;text-align:left;font-size:smaller}div#password-container[data-v-02517de9]{display:flex;flex-direction:column;gap:5px}div#password-container input[type=password][data-v-02517de9]{width:300px;background-color:var(--color-background)}.settings-container[data-v-f00f1fc8]{display:flex;flex-direction:row;align-items:center;justify-content:space-between;gap:2rem;min-width:300px;width:100%;padding-block:.2rem;padding-inline:1rem;border-radius:.5rem;transition:background-color .15s}.settings-container[data-v-f00f1fc8]:hover{background-color:var(--color-background-lighter)}div.widget[data-v-f00f1fc8]{display:flex;flex-grow:0;align-self:"flex-end";justify-self:"flex-end"}.settings-header[data-v-f00f1fc8]{text-align:left}.settings-header p[data-v-f00f1fc8]{font-size:.6rem;color:var(--color-text-soft);margin:0;margin-top:.1rem}.switch-toggle[data-v-58ea3d44]{position:relative;display:inline-block;width:2rem;height:1.2rem}.switch-toggle input[type=checkbox][data-v-58ea3d44]{display:none}.switch-toggle .switch[data-v-58ea3d44]{position:absolute;top:0;left:0;right:0;bottom:0;background-color:#ccc;border-radius:1rem;cursor:pointer;transition:background-color .3s}.switch-toggle .switch[data-v-58ea3d44]:before{position:absolute;content:"";height:.84rem;width:.84rem;left:.18rem;bottom:.18rem;background-color:#fff;border-radius:50%;transition:transform .3s}.switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]{background-color:#2196f3}.switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]:before{transform:translate(.8rem)}.dark .switch-toggle .switch[data-v-58ea3d44]{background-color:#666}.dark .switch-toggle .switch[data-v-58ea3d44]:before{background-color:#aaa}.dark .switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]{background-color:#2a7795}div.main-toolbar.normal-layout[data-v-0d6cb588]{top:10px;left:10px;right:5px;border-radius:13px;padding-inline:10px;padding-right:10px}div.main-toolbar.compact-layout[data-v-0d6cb588]{top:0;left:0;right:0;border-radius:0;padding-inline:20px}div.main-toolbar[data-v-0d6cb588]{position:fixed;display:flex;align-items:center;justify-content:space-between;background-color:var(--color-background-soft);font-size:small;height:30px;z-index:1;transition:top .25s ease-in-out}div.main-toolbar.hidden[data-v-0d6cb588]{top:-30px}div.button[data-v-0d6cb588]{display:flex;align-items:center}div.nav-toggle[data-v-0d6cb588]{display:flex;align-items:center;justify-content:space-between;gap:1.5rem;background-color:var(--color-background-soft);font-size:small;height:30px;z-index:1;transition:top .25s ease-in-out}div.nav-toggle div.button[data-v-0d6cb588]{cursor:pointer;-webkit-user-select:none;user-select:none;font-weight:700;color:var(--color-text-soft)}div.nav-toggle div.button.active-nav[data-v-0d6cb588]{border-bottom:1px solid var(--color-theme);color:var(--color-theme)}@media only screen and (max-width: 767px){div.main-toolbar[data-v-0d6cb588]{left:0;right:0;border-radius:0}}#sp-container[data-v-d141d9f5]{display:flex;height:100%;width:100%;padding:0;margin:0}.splitter-pane[data-v-d141d9f5]{position:relative;flex-grow:1;padding:0;margin:0}.splitter[data-v-d141d9f5]{display:block;background-color:var(--color-border);transition-delay:0s}.splitter[data-v-d141d9f5]:hover,.splitter[data-v-d141d9f5]:active{background-color:var(--color-theme);transition-delay:.5s}div#ploty-chart[data-v-db3ba83e]{width:100%;height:100%;overflow:hidden;touch-action:none;-ms-touch-action:none}div#main-filtervis[data-v-97428746]{display:flex;width:100%;height:100%}.full[data-v-97428746]{width:100%;height:100%}div#plot3dDiv[data-v-97428746]{height:430px;width:100%;overflow:hidden;border-radius:10px;z-index:1;box-shadow:0 0 5px var(--color-shadow)}div#loadingDiv[data-v-97428746]{position:absolute;z-index:2;top:0;left:0;display:flex;flex-direction:row;align-items:center;justify-content:center}div#loadingDiv p.status[data-v-97428746]{font-size:large;font-weight:700}@media screen and (max-height: 900px){div#plot3dDiv[data-v-97428746]{height:260px}}div#searchbar[data-v-ab0dfe65]{display:flex;justify-content:center;align-items:center;margin:5px 0}div#searchbar-container[data-v-ab0dfe65]{display:flex;align-items:center;gap:10px;border:1px solid var(--color-border);border-radius:20px;padding:3px;margin-inline:10px;width:100%;height:2rem}select#searchType[data-v-ab0dfe65]{border:none;outline:none;width:100px;height:100%;border-radius:20px;font-weight:700;background-color:var(--color-background-ssoft);color:var(--color-theme);text-align-last:center}input#searchbar-input[data-v-ab0dfe65]{border:none;outline:none;width:100%;font-size:medium}input#searchbar-input[data-v-ab0dfe65]::placeholder{color:#78787880}div#noteEditor[data-v-d773806f]{display:flex;flex-direction:column;height:100%;width:100%}div.editor[data-v-d773806f]{text-align:left;align-items:center;justify-content:center;position:relative;overflow:hidden;height:100%}div.editor[data-v-d773806f]>*{flex:1;width:100%;height:100%}div#save-hint[data-v-d773806f]{width:100%;height:auto;position:absolute;bottom:24px;right:0;padding:.2rem;color:var(--color-text);padding-inline:.5rem;font-size:.8rem;font-weight:700;background-color:#c8325080;border-top-left-radius:.5rem;border-top-right-radius:.5rem}div#btn-container[data-v-d773806f]{display:flex;flex-direction:row;gap:0px;width:100%;background-color:var(--color-background);border-top:1px solid var(--color-border)}div#misc-toggle[data-v-d773806f]{display:flex;justify-content:center;align-items:center;height:1.2rem;width:100%;background-color:var(--color-background-soft);border-top:1px solid var(--color-border)}div#misc-toggle[data-v-d773806f]:hover{background-color:var(--color-background-theme)}div#triangle[data-v-d773806f]{width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-bottom:10px solid var(--color-theme)}div#triangle-down[data-v-d773806f]{width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-top:10px solid var(--color-theme)}div#misc-container[data-v-d773806f]{display:flex;flex-direction:column;justify-content:flex-start;min-height:5rem;height:fit-content;background-color:var(--color-background);border-top:1px solid var(--color-border)}div.misc-file[data-v-d773806f]{padding-inline:.5rem;justify-content:space-between;border-bottom:1px solid var(--color-border);background-color:var(--color-background);color:var(--color-text);font-size:.8rem;gap:.5rem;display:flex}.misc-file-op-container[data-v-d773806f]{display:none;gap:.5rem}div.misc-file[data-v-d773806f]:hover{background-color:var(--color-background-theme-highlight)}div.misc-file:hover .misc-file-op-container[data-v-d773806f]{display:flex}button[data-v-d773806f],[data-v-d773806f] button{background-color:var(--color-background);border-radius:0%;width:100%;margin:0;border:.1px solid var(--color-border);height:2rem;color:var(--color-text);cursor:pointer}button[data-v-d773806f]:hover,[data-v-d773806f] button:hover{background-color:var(--color-background-theme-highlight)}label.frontmatter-label[data-v-d773806f]{display:none}a.frontmatter-link[data-v-d773806f]{background-color:var(--color-pure);box-shadow:0 2px 3px 0 var(--color-shadow);border-radius:15px;padding-inline:8px}a.frontmatter-link[data-v-d773806f]:hover{background-color:var(--color-background-theme-highlight)}div#summary-panel-main[data-v-165f5216]{width:100%;height:100%;display:flex;flex-direction:column;text-align:left;padding:10px;background-color:var(--color-background)}h2.title[data-v-165f5216]{font-size:1.2em;font-weight:700;margin:0;padding:0}div.authors-div[data-v-165f5216]{display:flex;flex-wrap:wrap;gap:5px}div.author-container[data-v-165f5216]{display:flex;align-items:center}span.author[data-v-165f5216]{text-decoration:underline;text-underline-offset:3px;white-space:nowrap;font-size:small}span.author-paper-count[data-v-165f5216]{font-size:small;color:var(--color-text-soft);padding-inline:3px;border-radius:5px}span.author-paper-count[data-v-165f5216]:hover{cursor:pointer;background-color:var(--color-background-soft)}div.publication[data-v-165f5216]{font-style:italic;font-size:small}div.docsize span[data-v-165f5216]{font-size:.8em;color:var(--color-text-soft);padding-inline:5px;padding-block:2px;border-radius:5px;border:1px solid var(--color-border)}body[data-v-3d4d3304]{height:100vh}#main-home[data-v-3d4d3304]{margin-top:40px;height:calc(100vh - 50px);width:calc(100vw - 20px);display:flex;flex-direction:column;border:1px solid var(--color-border);border-radius:15px;overflow:hidden;box-shadow:0 0 5px var(--color-shadow)}#main-home.compact[data-v-3d4d3304]{margin-top:30px;height:calc(100vh - 30px);width:100vw;border-radius:0}.panel1[data-v-3d4d3304]{width:100%;height:100%;align-self:center;margin:0}#doc-panel[data-v-3d4d3304]{display:flex;flex-direction:column;width:100%;gap:5px;overflow-x:hidden}div#doc-container[data-v-3d4d3304]{display:flex;flex-direction:column;height:100%}div#doc-top-bar[data-v-3d4d3304]{z-index:1;margin-top:0;padding-top:0;display:flex;justify-content:space-between;box-shadow:0 0 5px 0 var(--color-shadow);border-bottom:1px solid var(--color-border)}#blankPlaceholder[data-v-3d4d3304]{display:flex;flex-direction:column;align-items:center;justify-content:center;height:100%}#blankPlaceholder p[data-v-3d4d3304]{color:var(--color-text-soft);text-align:center;margin:10px}.fullHeight[data-v-3d4d3304]{height:100%}.fullWidth[data-v-3d4d3304]{width:100%}div.horizontal[data-v-3d4d3304]{display:flex}.left-in-enter-active[data-v-3d4d3304],.left-in-leave-active[data-v-3d4d3304]{transition:all 75ms ease-in-out}.left-in-enter-from[data-v-3d4d3304]{opacity:0;transform:translate(-10%)}@media screen and (max-width: 767px){#main-home[data-v-3d4d3304]{width:100vw;margin-top:30px;height:calc(100vh - 40px);border-radius:0;border-left:none;border-right:none}}#authorPapers[data-v-8a4a3cb8]{width:100%;max-height:80vh;min-width:360px}a[data-v-8a4a3cb8]{border-radius:1rem;padding-inline:.5rem;padding-block:.2rem}a[data-v-8a4a3cb8]:hover{cursor:pointer}a.link[data-v-8a4a3cb8]{padding:0}a.link[data-v-8a4a3cb8]:hover{text-decoration:underline;text-underline-offset:.1em;background-color:#0000}div#tag-selector[data-v-8a4a3cb8]{padding:5px 10px}div#feed-main[data-v-8a4a3cb8]{display:flex;align-items:center;padding:1rem;background-color:var(--color-background);border-left:5px solid var(--color-background);border-bottom:1px solid var(--color-border);border-radius:5px}div#feed-main[data-v-8a4a3cb8]:hover{transition:all .3s ease;border-left:5px solid var(--color-theme)}.articleBlock[data-v-8a4a3cb8]{width:90vw;max-width:1200px;display:flex;flex-direction:column;justify-content:flex-start;text-align:justify;gap:.3em}div.titleBlock[data-v-8a4a3cb8]{display:flex;flex-direction:column;align-items:flex-start;text-align:start;flex-wrap:wrap;gap:.25em}label.titleId[data-v-8a4a3cb8],.pubCount[data-v-8a4a3cb8]{color:#1ac4d0c9}span.authorSpan[data-v-8a4a3cb8]{display:inline-block;padding-left:.25em;padding-right:.25em}div.actions[data-v-8a4a3cb8]{display:flex;flex-direction:row;justify-content:flex-start;gap:1em}#relatedArticles[data-v-8a4a3cb8]{display:flex;flex-direction:row;justify-content:space-between;align-items:center;width:100%}label.relatedArticleScore[data-v-8a4a3cb8]{border-radius:5px;padding-left:5px;padding-right:5px;display:flex;align-items:center;justify-content:center;background-color:var(--color-background-theme-highlight)}#main[data-v-ed7e2b2f]{margin-top:40px;width:min(1200px,100vw - 20px);min-height:calc(100vh - 40px);display:flex;flex-direction:column;justify-content:flex-start}div#loadingPlaceholder[data-v-ed7e2b2f]{display:flex;flex-direction:column;justify-content:center;align-items:center;flex-grow:1}div#settings[data-v-ed7e2b2f]{display:flex;flex-direction:column;justify-content:center;align-items:center;gap:.5rem}div#settings input[data-v-ed7e2b2f],div#settings select[data-v-ed7e2b2f]{height:1.5rem;border-radius:.5rem;padding-inline:1rem;background-color:var(--color-background-soft);border:none;color:var(--color-text)}div#settings select[data-v-ed7e2b2f]{min-width:2rem;max-width:8rem;font-weight:700}div#settings input[type=text][data-v-ed7e2b2f]{height:2rem;border-radius:1rem;width:100%;margin-block:.5rem}h1[data-v-ed7e2b2f]{font-weight:700}img.icon[data-v-ed7e2b2f]{height:20px;filter:invert(.5) opacity(.35) drop-shadow(0 0 0 var(--color-border));transition:all .2s;cursor:pointer}img.icon.spin[data-v-ed7e2b2f]{animation:spin 1s linear infinite}img.icon[data-v-ed7e2b2f]:hover{filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-theme))}.error[data-v-34f6e322]{color:red}div.main[data-v-34f6e322]{text-align:center}div#login[data-v-34f6e322]{border:1px solid var(--color-border);box-shadow:0 3px 5px var(--color-shadow);border-radius:15px;padding:15px;text-align:center;background-color:var(--color-background-ssoft);margin-bottom:.5rem}input[type=text][data-v-34f6e322],input[type=password][data-v-34f6e322]{font-family:Gill Sans,sans-serif;font-size:medium;border-radius:1rem;min-width:8rem;border:1px solid var(--color-border);background-color:var(--color-background);transition:all .3s;padding-inline:.8rem;height:2rem}input[data-v-34f6e322]:focus{outline:none;border:1px solid var(--color-theme)}div.loginLine[data-v-34f6e322]{margin-top:.5rem}div.loginLine label[data-v-34f6e322]{font-weight:700}div.options[data-v-34f6e322]{margin:5px;display:flex;gap:10px}button[data-v-34f6e322]{width:100%;margin-top:.5rem;border-radius:1rem;height:2rem}input.key-input[data-v-34f6e322]{width:275px}details[data-v-34f6e322]{padding:5px}div#settings[data-v-34f6e322]{border-radius:5px;background-color:var(--color-background-mute);padding:5px}details summary[data-v-34f6e322]{text-align:left}details input[data-v-34f6e322]{width:160px}#port[data-v-34f6e322]{display:inline-block;width:50px}#registration-form[data-v-74eb04e9]{margin:0 auto;text-align:left;padding:1rem;padding-inline:1.5rem}#registration-form button[data-v-74eb04e9]{width:100%;height:2.5rem;margin-top:1rem;border-radius:1.25rem;border:1px solid var(--color-border);background-color:var(--color-background-ssoft);transition:all .3s;font-size:medium;cursor:pointer;box-shadow:0 2px 3px var(--color-shadow)}#registration-form button[data-v-74eb04e9]:hover{background-color:var(--color-background-theme)}td.horizontal[data-v-74eb04e9]{display:flex;flex-direction:row;gap:.5rem;align-items:center}#form-container[data-v-74eb04e9]{display:flex;flex-direction:column;gap:.25rem}.form-elem[data-v-74eb04e9]{display:flex;flex-direction:column-reverse}.form-elem span[data-v-74eb04e9]{margin-left:.5rem;font-size:small;color:var(--color-text)}.form-elem input[data-v-74eb04e9]{font-family:Gill Sans,sans-serif;font-size:medium;border-radius:1rem;min-width:8rem;border:1px solid var(--color-border);background-color:var(--color-background);transition:all .3s;padding-inline:.5rem;height:2rem}.form-elem input[data-v-74eb04e9]:focus{outline:none;border:1px solid var(--color-theme)}.form-elem input:focus+span[data-v-74eb04e9]{color:var(--color-theme)}div#show-password-container[data-v-74eb04e9]{margin-top:.5rem;display:flex;flex-direction:row;gap:.2rem;align-items:center}#login-main[data-v-def42eb3]{display:flex;height:100vh;width:100vw;justify-content:center;align-items:center}#info[data-v-def42eb3]{bottom:0;right:0;margin:.5em;font-size:smaller}div#login-main a[data-v-def42eb3]{cursor:pointer;padding-inline:.5rem;border-radius:.5rem}div#body[data-v-c3f015a3]{width:100%;height:100%}iframe[data-v-c3f015a3]{width:100%;height:100%;padding:0;margin:0}@media only screen and (max-width: 767px){iframe[data-v-c3f015a3]{border-radius:0}}div#main-reader[data-v-39571ec0]{bottom:0;padding-top:0;position:fixed;top:30px;left:0;right:0;background-color:var(--color-background)}@media only screen and (max-width: 767px){div#main-reader[data-v-39571ec0]{padding:0}}div#toolbarOps[data-v-39571ec0]{display:flex;align-items:center;justify-content:center}div#recently-read[data-v-39571ec0]{display:flex;align-items:center;justify-content:center;padding:0 10px;border-radius:5px;background-color:var(--color-background);color:var(--color-text);font-size:.8em;font-weight:700;cursor:pointer;text-wrap:nowrap;white-space:nowrap;overflow-x:hidden}div.horizontal[data-v-ab4897ef]{display:flex;flex-direction:row;align-items:center;gap:10px}h2[data-v-ab4897ef]{white-space:nowrap}div.center[data-v-ab4897ef]{display:flex;justify-content:center;align-items:center}div.full-width[data-v-ab4897ef]{width:100%}div.full-height[data-v-ab4897ef]{height:100%}div.left-align[data-v-ab4897ef]{text-align:left}img.avatar[data-v-ab4897ef]{width:32px;height:32px;border-radius:50%}label.admin_hint[data-v-ab4897ef]{font-size:small;font-weight:700;padding:3px 5px;border-radius:7px;background-color:var(--color-background-theme);color:var(--color-theme)}div#user-widget-header[data-v-ab4897ef]{display:flex;flex-direction:row;justify-content:center;align-items:center;gap:10px}div#user-widget-header b[data-v-ab4897ef]{font-weight:bolder;font-size:x-large}div#add-user-div[data-v-ab4897ef]{margin-top:5px;width:25px;height:25px;display:flex;justify-content:center;align-items:center;border-radius:5px;border:2px solid var(--color-border);background-color:var(--color-background-ssoft);font-weight:bolder;opacity:30%;transition:opacity .25s;transition-delay:.1s;cursor:pointer}div#add-user-div[data-v-ab4897ef]:hover{opacity:90%}table[data-v-ab4897ef]{border-collapse:collapse}tr.user-line[data-v-ab4897ef]:hover{border-radius:5px}tr.user-line[data-v-ab4897ef]:hover{background-color:var(--color-background-theme)}th[data-v-ab4897ef]{font-weight:700;text-align:center;vertical-align:middle;justify-self:center;padding:2px 5px}td[data-v-ab4897ef]{text-align:center;vertical-align:middle;justify-self:center;padding:2px 5px}td.username[data-v-ab4897ef]{font-weight:700;font-size:smaller;color:var(--color-text-soft)}b[data-v-ab4897ef]{font-weight:700}img.icon[data-v-ab4897ef]{height:20px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}div.edit-button[data-v-ab4897ef]{border-radius:30%;width:20px;height:20px;cursor:pointer;opacity:30%}div.edit-button[data-v-ab4897ef]:hover{opacity:100%}div#user-editor-main[data-v-ab4897ef]{padding-inline:2rem;padding-block:1rem;display:flex;flex-direction:column;align-items:flex-start;gap:10px}img.avatar-big[data-v-ab4897ef]{width:128px;height:128px;border-radius:5%}div#user-editor[data-v-ab4897ef]{display:flex;flex-direction:column;align-items:flex-start;gap:10px}div#mandatory-tag-edit[data-v-ab4897ef]{padding-left:5px;padding-right:5px;width:100%;border-radius:8px;background-color:var(--color-background)}div#delete-user-dialog-main[data-v-ab4897ef]{padding:10px;padding-inline:2rem}input[type=button]#delete-user-button[data-v-ab4897ef]{padding:5px;border-radius:5px;border:1px solid var(--color-border);background-color:var(--color-red-transparent);color:var(--color-danger);font-weight:700;width:100%}input[type=button]#delete-user-button[data-v-ab4897ef]:hover{background-color:var(--color-danger-hover)}input[type=text]#delete-user-input[data-v-ab4897ef]{padding:5px;border-radius:5px;border:1px solid var(--color-border)}div#create-user-main[data-v-ab4897ef]{padding-inline:1rem;padding-block:.7rem}table#create-user-table[data-v-ab4897ef]{width:100%;border-collapse:collapse}table#create-user-table tr td[data-v-ab4897ef]{text-align:left}input[type=text].create-user-input[data-v-ab4897ef]{padding:5px;width:100%;background-color:var(--color-background);min-width:200px}input[type=number][data-v-ab4897ef]{padding:5px;width:100%;background-color:var(--color-background);min-width:200px;border:none;color:var(--color-text);border-radius:5px}h1[data-v-2f65f22c]{font-size:2rem;font-weight:700;margin-top:1rem;padding-block:.8rem}h2[data-v-2f65f22c]{font-weight:700;margin-top:1rem;padding-block:.8rem;border-top:1px solid var(--color-border)}a[data-v-2f65f22c]{text-underline-offset:2px}a[data-v-2f65f22c]:hover{text-decoration:underline;background-color:unset}div#about-main[data-v-2f65f22c]{display:flex;flex-direction:column;justify-content:center;align-items:center;max-width:900px;margin-top:40px}b[data-v-2f65f22c]{font-weight:700}div.content[data-v-2f65f22c]{padding-inline:1rem;width:100%;text-align:left}div#versionHistory[data-v-2f65f22c]{padding:20px;display:flex;flex-direction:column}div#block[data-v-2f65f22c]{display:flex;flex-direction:column;justify-content:flex-start;align-items:flex-start}hr[data-v-2f65f22c]{width:100%;margin-top:10px;margin-bottom:10px;border:1px solid var(--color-border);border-top:none}summary[data-v-2f65f22c]{cursor:pointer;-webkit-user-select:none;user-select:none}div.link-container[data-v-2f65f22c]{display:flex;flex-direction:row;justify-content:center;align-items:center;margin-top:1rem;border:1px solid var(--color-border);border-radius:3rem;padding:.3rem;gap:.5rem;white-space:nowrap;width:100%}div#widget-container-main[data-v-257ac3c4]{box-shadow:0 2px 3px 0 var(--color-shadow);background-color:var(--color-background);border:1px solid var(--color-border);border-radius:20px;padding:20px;display:flex;align-items:center;justify-content:center;flex-wrap:wrap;flex-direction:row;max-width:1200px}@media only screen and (max-width: 767px){div#widget-container-main[data-v-257ac3c4]{border-radius:0;border:none;box-shadow:none;padding:0}}div#main-dashboard[data-v-6b501763]{margin-top:65px;display:flex;align-items:flex-start;flex-wrap:wrap;justify-content:center;flex-direction:row;width:calc(100vw - 20px);gap:20px}div.test[data-v-3b8741a7]{margin-top:1rem;font-size:medium}table[data-v-3b8741a7]{width:100%;border:1px solid var(--color-border);border-collapse:collapse}td[data-v-3b8741a7]{padding:.5rem;text-align:left;border:1px solid var(--color-border)}div.test form[data-v-3b8741a7]{display:flex;flex-direction:column;gap:.5rem}div.test form label[data-v-3b8741a7]{margin-top:.5rem}button[data-v-3b8741a7]{width:100%;height:2rem}input[data-v-3b8741a7],select[data-v-3b8741a7]{width:100%;height:1.8rem;border:1px solid var(--color-border)}
+@keyframes popupGradIn-7a7b12ca{0%{visibility:hidden;opacity:0}to{visibility:visible}}#popup[data-v-7a7b12ca]{position:fixed;z-index:100;display:flex;flex-direction:column;align-items:center;justify-content:center;box-shadow:0 1px 3px 3px var(--color-shadow);border-radius:10px;padding:10px;animation:popupGradIn-7a7b12ca .25s ease-in-out}.loading-widget[data-v-1d6933bb]{display:flex;align-items:center;justify-content:center;height:100%}.loading-widget__spinner[data-v-1d6933bb]{border-radius:50%;animation:spin-1d6933bb 1s ease-in-out infinite}@keyframes spin-1d6933bb{to{transform:rotate(360deg)}}div.loading-popout[data-v-95a13423]{position:absolute;bottom:0;right:0;padding:10px;width:240px;margin:20px;display:flex;flex-direction:row;align-items:center;justify-content:center;gap:10px;border:1px solid var(--color-border);border-radius:5px;box-shadow:0 1px 2px 0 var(--color-shadow);z-index:99;background-color:var(--color-background-theme-thin)}#app[data-v-934929d5]{margin:0;padding:0}:root{--vt-c-white: #f2f2f2;--vt-c-white-soft: #e3e3e3;--vt-c-white-mute: rgb(228, 228, 228);--vt-c-black: #1f1f1f;--vt-c-black-soft: #303030;--vt-c-black-mute: #3f3f3f;--vt-c-indigo: #2c3e50;--vt-c-divider-light-1: rgba(60, 60, 60, .29);--vt-c-divider-light-2: rgba(60, 60, 60, .12);--vt-c-divider-dark-1: rgba(90, 90, 90, .65);--vt-c-divider-dark-2: rgba(90, 90, 90, .48);--vt-c-text-light-1: var(--vt-c-indigo);--vt-c-text-light-2: rgba(60, 60, 60, .66);--vt-c-text-dark-1: var(--vt-c-white);--vt-c-text-dark-2: rgba(235, 235, 235, .64)}:root,:root.light{--section-gap: 160px;--color-background: var(--vt-c-white);--color-background-soft: var(--vt-c-white-soft);--color-background-mute: var(--vt-c-white-mute);--color-background-darker: var(--vt-c-white-mute);--color-background-lighter: var(--vt-c-white);--color-border: var(--vt-c-divider-light-2);--color-border-hover: var(--vt-c-divider-light-1);--color-heading: var(--vt-c-text-light-1);--color-text: var(--vt-c-text-light-1);--color-shadow: rgba(0, 0, 0, .12)}:root.dark{--color-background: var(--vt-c-black);--color-background-soft: var(--vt-c-black-soft);--color-background-mute: var(--vt-c-black-mute);--color-background-darker: var(--vt-c-black);--color-background-lighter: var(--vt-c-black-mute);--color-border: var(--vt-c-divider-dark-2);--color-border-hover: var(--vt-c-divider-dark-1);--color-heading: var(--vt-c-text-dark-1);--color-text: var(--vt-c-text-dark-2);--color-shadow: rgba(0, 0, 0, .3)}:root{--color-red-transparent: rgba(200, 50, 80, .084);--color-red: rgb(200, 50, 80);--color-danger: rgb(200, 50, 80);--color-danger-hover: rgba(200, 50, 80, .2)}:root,:root.light{--color-pure: #fff;--color-theme: rgb(82, 153, 182);--color-text-soft: rgba(80, 80, 80, .5);--color-background-ssoft: #e8e8e8;--color-background-theme-highlight: rgba(137, 189, 213, .2);--color-background-theme-thin: #dbdee5;--color-background-theme: rgba(127, 178, 220, .3);--color-background-tagpanel: #efefef;--color-progressbar: #007bff;--color-background-progressbar: #f4f4f4}:root.dark{--color-pure: #000;--color-theme: rgb(80, 180, 200);--color-text-soft: rgba(180, 180, 180, .5);--color-background-ssoft: #2c2c2c;--color-background-theme-highlight: rgba(108, 186, 185, .2);--color-background-theme-thin: #383b41;--color-background-theme: rgba(52, 84, 93, .3);--color-background-tagpanel: #232323;--color-progressbar: #0e58a8;--color-background-progressbar: #202020}*,*:before,*:after{box-sizing:border-box;margin:0;position:relative;font-weight:400}body{color:var(--color-text);background:var(--color-background);transition:color .5s,background-color .5s;line-height:1.6;font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:15px;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}@keyframes slideInUpAnim{0%{visibility:hidden;transform:translateY(5%);opacity:0}to{visibility:visible;transform:translateY(0)}}@keyframes slideInDownAnim{0%{visibility:hidden;transform:translateY(-5%);opacity:0}to{visibility:visible;transform:translateY(0)}}@keyframes slideInBackAnim{0%{visibility:hidden}1%{transform:translateY(6%) scale(.95);opacity:0;visibility:visible}60%{transform:translateY(-4%) scale(1.01)}to{transform:translateY(0);opacity:1}}@keyframes rotate90in{0%{transform:rotate(-90deg)}to{transform:rotate(0)}}@keyframes gradInAnim{0%{opacity:0}to{opacity:1}}.gradIn{animation-duration:.3s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:gradInAnim}.slideIn{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInUpAnim}.slideInFast,.slidInFast{animation-duration:.15s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInUpAnim}.slideInDown{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:slideInDownAnim}.slideIn2{animation-duration:.375s;animation-fill-mode:backwards;animation-timing-function:ease-out;animation-name:slideInBackAnim}.rotate90in{animation-duration:.375s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:rotate90in}.hoverMaxout11:hover{transform:scale(1.1)}.hoverMaxout105:hover{transform:scale(1.05)}.hoverMaxout103:hover{transform:scale(1.03)}.hoverMaxout101:hover{transform:scale(1.01)}body{display:flex;place-items:center}#app{margin:0 auto;font-weight:400;text-align:center;align-self:center;display:flex;align-items:center;justify-content:center}a,.green{text-decoration:none;color:#089d86;transition:.4s}b{font-weight:700}@media (hover: hover){a:hover{background-color:#00bd7e33}}.shadow{box-shadow:0 1px 3px 2px var(--color-shadow)}.scrollable{overflow-y:auto;overflow-x:auto}.hover-scrollable{overflow-x:hidden;overflow-y:hidden}.hover-scrollable:hover{overflow-x:auto;overflow-y:auto}.non-selectable{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}html{--scrollbarBG: var(--color-background-soft);--thumbBG: var(--color-border)}body,.panel,.scrollable,.hover-scrollable{scrollbar-width:thin;scrollbar-color:var(--thumbBG) var(--scrollbarBG)}body::-webkit-scrollbar,.panel::-webkit-scrollbar,.scrollable::-webkit-scrollbar,.hover-scrollable::-webkit-scrollbar{width:11px}body::-webkit-scrollbar-track,.panel::-webkit-scrollbar-track,.scrollable::-webkit-scrollbar-track,.hover-scrollable::-webkit-scrollbar-track{background:var(--scrollbarBG)}body::-webkit-scrollbar-thumb,.panel::-webkit-scrollbar-thumb,.scrollable::-webkit-scrollbar-thumb,.hover-scrollable::-webkit-scrollbar-thumb{background-color:var(--thumbBG);border-radius:6px;border:3px solid var(--scrollbarBG)}input[type=text],input[type=password]{border:transparent;color:var(--color-text);height:24px;border-radius:8px;padding-left:4px;font-size:small;background-color:var(--color-background-soft);background-color:transparent}textarea{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text)}input[type=button],button{border-radius:5px;height:24px;border:1px solid var(--color-border);background-color:var(--color-background-soft);font-size:small;color:var(--color-text)}input[type=button]:hover,button:hover{background-color:var(--color-background-theme-highlight);transition:all .15s}select{border-radius:8px;border:1px solid var(--color-border);padding:2px 5px;background-color:var(--color-background-soft);background-color:transparent;color:var(--color-text);-webkit-appearance:none}div[data-v-582ee950]{--radius: 16px;--radius-inner: 6px;display:flex;align-items:center;gap:5px}div.toggle[data-v-582ee950]{justify-content:left;flex-direction:row-reverse;flex-wrap:nowrap}#checkCircle[data-v-582ee950]{border:3px solid var(--color-border);height:var(--radius);width:var(--radius);border-radius:50%;justify-content:center}#checkStatus[data-v-582ee950]{height:var(--radius-inner);width:var(--radius-inner);border-radius:50%;background-color:var(--color-theme)}#checkCircle[data-v-582ee950]:hover{background-color:var(--color-background-theme-highlight);transition:all .2s}label:hover+#checkCircle[data-v-582ee950]{background-color:var(--color-background-theme-highlight);transition:all .2s}label[data-v-582ee950]{text-align:left;text-overflow:ellipsis;overflow:clip}div[data-v-3c7d3255]{--button-dim: 16px;--triangle-dim: 8px}div.row[data-v-3c7d3255]{display:flex;align-items:center;gap:2px}div.collapseButton[data-v-3c7d3255]{width:var(--button-dim);height:var(--button-dim);min-width:var(--button-dim);min-height:var(--button-dim);border-radius:50%;display:flex;align-items:center;justify-content:center}.toggleText[data-v-3c7d3255]{flex-grow:1;margin-top:2px;margin-bottom:2px;border-radius:5px;transition:all .1s ease}.toggleText[data-v-3c7d3255]:hover{background-color:var(--color-background-theme-highlight)}.triangle-right[data-v-3c7d3255]{width:var(--triangle-dim);height:var(--triangle-dim);background-color:var(--color-theme);clip-path:polygon(0 0,0% 100%,100% 50%)}.triangle-down[data-v-3c7d3255]{width:var(--triangle-dim);height:var(--triangle-dim);background-color:var(--color-theme);clip-path:polygon(0 0,100% 0%,50% 100%)}div.children[data-v-3c7d3255]{margin-left:20px}#tagSelector-main[data-v-f90dfe41]{flex-grow:1}div.bubble[data-v-f454bc70]{padding:3px 5px;text-align:left;border-radius:7px;background-color:var(--color-background-soft);transition:all .2s;font-size:small;display:flex;justify-content:center;align-items:center;cursor:default}div.highlight[data-v-f454bc70]{background-color:#f836ff3f;box-shadow:0 0 5px var(--color-shadow)}div.muted[data-v-f454bc70]{opacity:.35}div.prefix[data-v-f454bc70]{padding:3px;background-color:var(--color-background-theme-thin);font-size:x-small;color:var(--color-text-theme);border-radius:3px;margin-right:5px}div#bubbleContainer[data-v-62e107cd]{display:flex;flex-wrap:wrap;align-items:center;gap:5px;padding:5px;border-radius:5px;overflow:visible}div#title-title[data-v-9523b989]{margin-left:5px;display:flex;justify-content:space-between;align-items:center}div#title-title h3[data-v-9523b989]{text-align:left;font-weight:700;color:var(--color-theme)}div#title-buttons[data-v-9523b989]{display:flex;gap:5px;opacity:.15;transition:opacity .5s;transition-delay:opacity .2s}div#title-buttons div.button[data-v-9523b989]:hover{text-decoration:underline;text-underline-offset:2px}div#title-buttons div.button[data-v-9523b989]{transition:all .2s;padding-left:5px;padding-right:5px;font-size:smaller;border-radius:5px;cursor:pointer}div#title-title:hover div#title-buttons[data-v-9523b989]{opacity:1}hr[data-v-9523b989]{margin-top:5px;border:1px solid var(--color-border);border-top:none}div#file-tags-main[data-v-9523b989]{padding:15px 10px;min-width:260px;width:fit-content;height:100%;display:flex;flex-direction:column;justify-content:space-between;border-radius:10px 0 0 10px;border:1px solid var(--color-border);border-top:none;border-left:none;border-bottom:none;background-color:var(--color-background-tagpanel);gap:10px}div.buttons[data-v-9523b989]{padding-left:5px;padding-right:5px}#btnClear[data-v-9523b989]{padding:5px;width:100%;border:0px solid var(--color-border);font-weight:700}@keyframes floatingWindowGradIn-c6dbcdc2{0%{visibility:hidden;transform:scale(.9);opacity:0}to{visibility:visible}}div#blocker[data-v-c6dbcdc2]{position:fixed;top:0;left:0;width:100vw;height:100%;background-color:#00000080;display:flex;justify-content:center;align-items:center}div.header[data-v-c6dbcdc2]{display:flex;flex-direction:row;justify-content:space-between;align-items:center;width:100%;padding:10px}.header label[data-v-c6dbcdc2],.header span[data-v-c6dbcdc2]{font-size:x-small;color:var(--color-text);opacity:.5}.header label[data-v-c6dbcdc2]{text-align:left}.floating-window[data-v-c6dbcdc2]{background-color:var(--color-background-soft);border:1px solid var(--color-border);border-radius:5px;display:flex;flex-direction:column;align-items:flex-start;box-shadow:0 1px 3px 2px var(--color-shadow);animation-duration:.1s;animation-timing-function:ease-out;animation-delay:0s;animation-iteration-count:1;animation-name:floatingWindowGradIn-c6dbcdc2}.window-content[data-v-c6dbcdc2]{max-width:calc(100vw - 50px);max-height:calc(100vh - 80px);overflow:auto}.close-button[data-v-c6dbcdc2]{min-width:2.6em;width:2.6em;height:1.8em;align-self:flex-start;background:none;border:1px solid var(--color-border);border-radius:.75em;cursor:pointer;padding:0;display:flex;align-items:center;justify-content:center}.close-button[data-v-c6dbcdc2]:hover{background-color:#c832504d;transition:all .2s}.close-icon[data-v-c6dbcdc2]{margin:0;font-size:medium;font-weight:700}div#query-dialog-main[data-v-81948a9f]{display:flex;flex-direction:column;height:100%}div#buttons[data-v-81948a9f]{display:flex;flex-direction:row;justify-content:space-around;margin-top:10px;border-top:1px solid var(--color-border)}div.button[data-v-81948a9f]{display:flex;justify-content:center;align-items:center;width:100%;padding:5px;cursor:pointer;background-color:var(--color-background-soft)}div.button[data-v-81948a9f]:hover{box-shadow:inset 0 0 5px 1px var(--color-shadow)}div.ok-button[data-v-81948a9f]:hover{background-color:var(--color-background-theme-highlight)}div.cancel-button[data-v-81948a9f]:hover{background-color:var(--color-danger-hover)}div.last-button[data-v-81948a9f]{border-left:1px solid var(--color-border)}div#tag-selector-with-entry-main[data-v-990ad4c4]{display:flex;flex-direction:column;align-items:flex-start;justify-content:center;width:100%;height:100%;gap:10px}textarea[data-v-990ad4c4],input[type=text][data-v-990ad4c4],div#tagSelector[data-v-990ad4c4]{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text);width:100%}div#tagSelector[data-v-990ad4c4]{min-width:300px;height:420px;padding:5px}label[data-v-990ad4c4]{font-weight:700}input[type=text][data-v-990ad4c4]{border:1px solid var(--color-border);border-radius:5px}div.entry[data-v-990ad4c4]{display:flex;flex-direction:row;align-items:center;width:100%;gap:5px}button[data-v-990ad4c4]{width:80px;cursor:pointer}button.to-be-confirmed[data-v-990ad4c4]{color:#ff0096;background-color:#00ffa6bf}div#blocker[data-v-c6b659c7]{position:fixed;top:0;left:0;width:100vw;height:100%;background-color:#00000080}#arrow[data-v-c6b659c7]{position:absolute;top:-10px;left:50%;margin-left:-10px;width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-bottom:10px solid var(--color-background-soft)}#floatingMenu[data-v-c6b659c7]{position:fixed;z-index:101;background-color:var(--color-background-soft);border:1px solid var(--color-border);border-radius:5px;box-shadow:0 1px 3px 2px var(--color-shadow)}.floatingMenuItem[data-v-c6b659c7]{cursor:pointer;padding:5px 15px;border-bottom:1px solid var(--color-border)}.floatingMenuItemLast[data-v-c6b659c7]{border-bottom:none}.floatingMenuItem[data-v-c6b659c7]:hover{background-color:var(--color-background-theme-highlight)}#inputDiv[data-v-e295a40e]{display:flex;flex-direction:row;width:100%;gap:10px;padding-left:15px;padding-right:15px}div.hr[data-v-e295a40e]{width:100%;height:1px;background-color:var(--color-border)}label[data-v-e295a40e]{font-weight:700}div.horizontal[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:10px;width:100%}div#bibtexSource[data-v-e295a40e]{font-size:small;margin-left:10px}div#bibtexSource div.button[data-v-e295a40e]{cursor:pointer;opacity:.2;transition:all .2s ease-in-out}div#bibtexSource div.button[data-v-e295a40e]:hover{cursor:pointer;opacity:1;color:var(--color-theme);text-decoration:underline}#inputLeft[data-v-e295a40e],#inputRight[data-v-e295a40e]{display:flex;flex-direction:column;width:100%;gap:10px}textarea[data-v-e295a40e],input[type=text][data-v-e295a40e]{border:1px solid var(--color-border);border-radius:5px;background-color:var(--color-background);color:var(--color-text);width:100%}div#bibtexArea[data-v-e295a40e]{display:flex;flex-direction:column;align-items:flex-start}div#bibtexArea textarea[data-v-e295a40e]{min-width:300px;width:100%;height:420px;padding:5px;font-size:medium;font-family:monospace}.wrapword[data-v-e295a40e]{white-space:-moz-pre-wrap!important;white-space:-webkit-pre-wrap;white-space:-pre-wrap;white-space:-o-pre-wrap;white-space:pre-wrap;word-wrap:break-word;word-break:break-all}div#urlArea[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:5px}div#urlArea>input[type=text][data-v-e295a40e]{width:100%}div#tagSelector[data-v-e295a40e]{width:100%;min-width:300px;height:420px;overflow:scroll;padding:5px}button#addNewTag[data-v-e295a40e]{width:80px}div.bibsource-container[data-v-e295a40e]{display:flex;flex-direction:row;align-items:center;gap:5px}.layout[data-v-9b2c5a9d]{display:flex;flex-direction:column;justify-content:center;align-items:center;gap:20px}#info[data-v-9b2c5a9d]{width:100%;display:flex;flex-direction:column;justify-content:center;align-items:flex-start;text-align:left}b[data-v-9b2c5a9d]{font-weight:700}#shortSummary[data-v-9b2c5a9d]{display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:left}#shortSummaryTitle[data-v-9b2c5a9d]{display:flex;flex-direction:row;justify-content:flex-start;align-items:center;gap:10px}.button[data-v-9b2c5a9d]{cursor:pointer;border-radius:3px}.button[data-v-9b2c5a9d]:hover{background-color:var(--color-background-theme-highlight)}details[data-v-9b2c5a9d]{width:100%}table[data-v-9b2c5a9d]{width:100%}td[data-v-9b2c5a9d]{vertical-align:top;padding-left:5px;padding-right:5px}td#authorTD[data-v-9b2c5a9d]{display:flex;flex-direction:row;justify-content:flex-start;align-items:flex-start;flex-wrap:wrap;gap:10px}td#authorTD div[data-v-9b2c5a9d]{display:block}tr#otherPubTR td[data-v-9b2c5a9d]{width:100%;padding:10px;border-radius:10px;border:1px solid var(--color-border);background-color:var(--color-background-mute)}.slideDown-enter-active[data-v-9b2c5a9d],.slideDown-leave-active[data-v-9b2c5a9d]{transition:all .15s ease}.slideDown-enter-from[data-v-9b2c5a9d],.slideDown-leave-to[data-v-9b2c5a9d]{transform:translateY(-10%);opacity:0}hr[data-v-564cf261]{margin:10px;border:1px solid var(--color-border)}div.row[data-v-564cf261]{display:flex;align-items:center;justify-content:center}div#moreMain[data-v-564cf261]{display:flex;flex-direction:column;align-items:center;justify-content:center;margin-top:8px;margin-bottom:10px;overflow-y:hidden}div#buttons[data-v-564cf261]{gap:10px}label.hint[data-v-564cf261]{font-size:xx-small;color:var(--color-border)}#abstract[data-v-564cf261]{max-width:1200px;text-align:justify;padding-left:10px;padding-right:10px}#abstract summary[data-v-564cf261]{font-weight:700;cursor:pointer;text-align:center}div#actions[data-v-564cf261]{gap:10px;background-color:var(--color-background-mute);margin:3px;padding-block:5px;padding-inline:50px;border-radius:20px;box-shadow:inset 0 1px 2px 0 var(--color-shadow)}[data-v-564cf261] a{cursor:pointer;border-radius:7px;padding-inline:5px;-webkit-user-select:none;user-select:none}[data-v-564cf261] a.btn{text-decoration:underline;text-underline-offset:2px;cursor:pointer}a.danger[data-v-564cf261]{color:var(--color-danger)}a.danger[data-v-564cf261]:hover{background-color:var(--color-danger-hover)}.actions-enter-active[data-v-564cf261],.actions-leave-active[data-v-564cf261]{transition:all .2s}.actions-enter-from[data-v-564cf261],.actions-leave-to[data-v-564cf261]{opacity:0;transform:translateY(-10px)}@keyframes expand-564cf261{0%{max-height:0px;opacity:0;margin:0}50%{max-height:48px;opacity:0}to{max-height:auto;opacity:1}}@keyframes contract-564cf261{0%{max-height:48px;opacity:1}50%{max-height:0px;opacity:0}to{margin:0;max-height:0px;opacity:0}}.expand-transition-enter-active[data-v-564cf261]{animation:expand-564cf261 .2s ease-in-out}.expand-transition-leave-active[data-v-564cf261]{animation:contract-564cf261 .2s ease-in-out}div.row[data-v-f2b3f69e]{display:flex;align-items:center;justify-content:flex-start;cursor:default}div#init[data-v-f2b3f69e]{display:flex;flex-wrap:nowrap;justify-content:space-between}div#init>div.left[data-v-f2b3f69e]{flex-wrap:nowrap;column-gap:5px;overflow:hidden}div#marks[data-v-f2b3f69e]:hover{cursor:pointer}div#fileRow[data-v-f2b3f69e]{border-radius:0;padding:3px;padding-inline:10px;width:100%}div.text[data-v-f2b3f69e]{padding:0;margin:0;text-align:left;text-overflow:ellipsis;overflow:hidden}div#status-container[data-v-f2b3f69e]{display:flex;flex-direction:row;align-items:center;gap:2px}div.status[data-v-f2b3f69e]{display:flex;align-items:center;justify-content:center;width:15px}img.icon[data-v-f2b3f69e]{height:15px;filter:invert(.5) opacity(.25) drop-shadow(0 0 0 var(--color-border))}img.redIcon[data-v-f2b3f69e]{filter:invert(33%) sepia(92%) saturate(3443%) hue-rotate(0deg) brightness(97%) contrast(101%)}img.placeholder[data-v-f2b3f69e]{height:8px}.more-enter-active[data-v-f2b3f69e],.more-leave-active[data-v-f2b3f69e]{transition:all .15s}.more-enter-from[data-v-f2b3f69e],.more-leave-to[data-v-f2b3f69e]{opacity:0}#title[data-v-f2b3f69e]{display:inline-block;white-space:wrap;word-break:break-word;overflow:hidden;text-overflow:ellipsis}@media (max-width: 768px){div#init>div.left[data-v-f2b3f69e]{width:100%;flex-wrap:wrap}div#init[data-v-f2b3f69e]{align-items:flex-start}div#status-container[data-v-f2b3f69e]{flex-direction:column;margin-block:5px;margin-left:5px;gap:1px}img.icon[data-v-f2b3f69e]{height:12px}img.placeholder[data-v-f2b3f69e]{height:12px;width:8px}}#datacard-container-main[data-v-006a79ab]{display:flex;flex-direction:column;align-items:center;justify-content:space-between;width:100%;height:100%;overflow-y:auto;overflow-x:hidden}#datacard-container[data-v-006a79ab]{display:flex;flex-direction:column;overflow-x:hidden;width:100%}label.relatedArticleScore[data-v-006a79ab]{border-radius:5px;padding-left:5px;padding-right:5px;display:flex;align-items:center;justify-content:center;background-color:var(--color-background-theme-highlight)}#datacard-container-footer[data-v-006a79ab]{display:flex;flex-direction:row;align-items:center;justify-content:center;width:100%;padding-block:5px;z-index:1;box-shadow:0 -0px 5px 0 var(--color-shadow)}#datacard-container-footer button[data-v-006a79ab]{border-radius:5px;padding-inline:30px;height:30px;padding-block:5px;font-weight:700;color:var(--color-text);border:none;display:flex;align-items:center;justify-content:center;transition:all .15s ease-in-out}#datacard-container-footer button[data-v-006a79ab]:hover{background-color:var(--color-background-theme-highlight);transform:scale(1.05)}#datacard-container-footer button[data-v-006a79ab]:active{transform:scale(.95)}#datacard-container-footer button[data-v-006a79ab]:disabled{color:var(--color-text-soft)}#datacard-container-footer button[data-v-006a79ab]:disabled:hover{background-color:transparent}.fade-enter-active[data-v-006a79ab],.fade-leave-active[data-v-006a79ab]{transition:all .5s ease-in-out}.fade-enter-from[data-v-006a79ab],.fade-leave-to[data-v-006a79ab]{opacity:0}span.button[data-v-f0fccbdf]{padding:3px 5px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:smaller;gap:2px}span.button[data-v-f0fccbdf]:hover{background-color:var(--color-background-theme-highlight);box-shadow:0 1px 3px 2px var(--color-shadow);transition:all .2s}img.icon[data-v-f0fccbdf]{height:20px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}@media (max-width: 600px){.iconLabel[data-v-f0fccbdf]{display:none}}#disk-usage-main[data-v-35d9044c]{display:flex;flex-direction:column;justify-content:center;align-items:flex-start;gap:0rem;width:100%;height:100%;overflow-y:auto}.disk-usage-bar[data-v-35d9044c]{width:100%;height:1rem;background-color:var(--color-background-progressbar);border-radius:5px;overflow:hidden}.disk-usage-fill[data-v-35d9044c]{height:100%;background-color:var(--color-progressbar);transition:width .3s ease-in-out}.disk-usage-text[data-v-35d9044c]{font-size:.75rem;text-align:center;height:100%;color:var(--color-text-soft);white-space:nowrap}div#usercard-main[data-v-02517de9]{margin-top:10px;display:flex;align-items:center;flex-direction:column;gap:.5rem;width:100%}div#info[data-v-02517de9]{display:flex;justify-content:center;align-items:center;flex-direction:row;gap:20px}label.admin_hint[data-v-02517de9]{font-size:x-small;padding-left:5px;padding-right:5px;height:12px;border-radius:5px;background-color:var(--color-background-theme);color:var(--color-theme)}div#info div#name-edit[data-v-02517de9]{display:flex;flex-direction:row;align-items:center;gap:10px}div#info div#user-desc[data-v-02517de9]{display:flex;flex-direction:column;align-items:flex-start;justify-self:flex-start}p#credential[data-v-02517de9]{font-family:monospace;color:var(--color-text-soft);cursor:pointer;font-size:.75rem}h1[data-v-02517de9]{font-weight:700}img.icon[data-v-02517de9]{height:25px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}img#edit-settings-icon[data-v-02517de9]{padding-top:8px;opacity:0;transition:all .2s ease-in-out}img#edit-settings-icon[data-v-02517de9]:hover{cursor:pointer}div#name-edit:hover img#edit-settings-icon[data-v-02517de9]{opacity:1}div#user-settings[data-v-02517de9]{margin:0 10px 10px;display:flex;flex-direction:column;text-align:left}div#user-settings hr[data-v-02517de9]{margin:0;padding:0}div#user-settings b[data-v-02517de9]{font-weight:700}div#user-settings input[type=text][data-v-02517de9]{width:300px;background-color:var(--color-background);height:36px}div#user-settings details summary[data-v-02517de9]{margin-top:5px;text-align:left;font-size:smaller}div#password-container[data-v-02517de9]{display:flex;flex-direction:column;gap:5px}div#password-container input[type=password][data-v-02517de9]{width:300px;background-color:var(--color-background)}.settings-container[data-v-f00f1fc8]{display:flex;flex-direction:row;align-items:center;justify-content:space-between;gap:2rem;min-width:300px;width:100%;padding-block:.2rem;padding-inline:1rem;border-radius:.5rem;transition:background-color .15s}.settings-container[data-v-f00f1fc8]:hover{background-color:var(--color-background-lighter)}div.widget[data-v-f00f1fc8]{display:flex;flex-grow:0;align-self:"flex-end";justify-self:"flex-end"}.settings-header[data-v-f00f1fc8]{text-align:left}.settings-header p[data-v-f00f1fc8]{font-size:.6rem;color:var(--color-text-soft);margin:0;margin-top:.1rem}.switch-toggle[data-v-58ea3d44]{position:relative;display:inline-block;width:2rem;height:1.2rem}.switch-toggle input[type=checkbox][data-v-58ea3d44]{display:none}.switch-toggle .switch[data-v-58ea3d44]{position:absolute;top:0;left:0;right:0;bottom:0;background-color:#ccc;border-radius:1rem;cursor:pointer;transition:background-color .3s}.switch-toggle .switch[data-v-58ea3d44]:before{position:absolute;content:"";height:.84rem;width:.84rem;left:.18rem;bottom:.18rem;background-color:#fff;border-radius:50%;transition:transform .3s}.switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]{background-color:#2196f3}.switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]:before{transform:translate(.8rem)}.dark .switch-toggle .switch[data-v-58ea3d44]{background-color:#666}.dark .switch-toggle .switch[data-v-58ea3d44]:before{background-color:#aaa}.dark .switch-toggle input[type=checkbox]:checked+.switch[data-v-58ea3d44]{background-color:#2a7795}div.main-toolbar.normal-layout[data-v-0d6cb588]{top:10px;left:10px;right:5px;border-radius:13px;padding-inline:10px;padding-right:10px}div.main-toolbar.compact-layout[data-v-0d6cb588]{top:0;left:0;right:0;border-radius:0;padding-inline:20px}div.main-toolbar[data-v-0d6cb588]{position:fixed;display:flex;align-items:center;justify-content:space-between;background-color:var(--color-background-soft);font-size:small;height:30px;z-index:1;transition:top .25s ease-in-out}div.main-toolbar.hidden[data-v-0d6cb588]{top:-30px}div.button[data-v-0d6cb588]{display:flex;align-items:center}div.nav-toggle[data-v-0d6cb588]{display:flex;align-items:center;justify-content:space-between;gap:1.5rem;background-color:var(--color-background-soft);font-size:small;height:30px;z-index:1;transition:top .25s ease-in-out}div.nav-toggle div.button[data-v-0d6cb588]{cursor:pointer;-webkit-user-select:none;user-select:none;font-weight:700;color:var(--color-text-soft)}div.nav-toggle div.button.active-nav[data-v-0d6cb588]{border-bottom:1px solid var(--color-theme);color:var(--color-theme)}@media only screen and (max-width: 767px){div.main-toolbar[data-v-0d6cb588]{left:0;right:0;border-radius:0}}#sp-container[data-v-d141d9f5]{display:flex;height:100%;width:100%;padding:0;margin:0}.splitter-pane[data-v-d141d9f5]{position:relative;flex-grow:1;padding:0;margin:0}.splitter[data-v-d141d9f5]{display:block;background-color:var(--color-border);transition-delay:0s}.splitter[data-v-d141d9f5]:hover,.splitter[data-v-d141d9f5]:active{background-color:var(--color-theme);transition-delay:.5s}div#ploty-chart[data-v-db3ba83e]{width:100%;height:100%;overflow:hidden;touch-action:none;-ms-touch-action:none}div#main-filtervis[data-v-97428746]{display:flex;width:100%;height:100%}.full[data-v-97428746]{width:100%;height:100%}div#plot3dDiv[data-v-97428746]{height:430px;width:100%;overflow:hidden;border-radius:10px;z-index:1;box-shadow:0 0 5px var(--color-shadow)}div#loadingDiv[data-v-97428746]{position:absolute;z-index:2;top:0;left:0;display:flex;flex-direction:row;align-items:center;justify-content:center}div#loadingDiv p.status[data-v-97428746]{font-size:large;font-weight:700}@media screen and (max-height: 900px){div#plot3dDiv[data-v-97428746]{height:260px}}div#searchbar[data-v-ab0dfe65]{display:flex;justify-content:center;align-items:center;margin:5px 0}div#searchbar-container[data-v-ab0dfe65]{display:flex;align-items:center;gap:10px;border:1px solid var(--color-border);border-radius:20px;padding:3px;margin-inline:10px;width:100%;height:2rem}select#searchType[data-v-ab0dfe65]{border:none;outline:none;width:100px;height:100%;border-radius:20px;font-weight:700;background-color:var(--color-background-ssoft);color:var(--color-theme);text-align-last:center}input#searchbar-input[data-v-ab0dfe65]{border:none;outline:none;width:100%;font-size:medium}input#searchbar-input[data-v-ab0dfe65]::placeholder{color:#78787880}div#noteEditor[data-v-d773806f]{display:flex;flex-direction:column;height:100%;width:100%}div.editor[data-v-d773806f]{text-align:left;align-items:center;justify-content:center;position:relative;overflow:hidden;height:100%}div.editor[data-v-d773806f]>*{flex:1;width:100%;height:100%}div#save-hint[data-v-d773806f]{width:100%;height:auto;position:absolute;bottom:24px;right:0;padding:.2rem;color:var(--color-text);padding-inline:.5rem;font-size:.8rem;font-weight:700;background-color:#c8325080;border-top-left-radius:.5rem;border-top-right-radius:.5rem}div#btn-container[data-v-d773806f]{display:flex;flex-direction:row;gap:0px;width:100%;background-color:var(--color-background);border-top:1px solid var(--color-border)}div#misc-toggle[data-v-d773806f]{display:flex;justify-content:center;align-items:center;height:1.2rem;width:100%;background-color:var(--color-background-soft);border-top:1px solid var(--color-border)}div#misc-toggle[data-v-d773806f]:hover{background-color:var(--color-background-theme)}div#triangle[data-v-d773806f]{width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-bottom:10px solid var(--color-theme)}div#triangle-down[data-v-d773806f]{width:0;height:0;border-left:10px solid transparent;border-right:10px solid transparent;border-top:10px solid var(--color-theme)}div#misc-container[data-v-d773806f]{display:flex;flex-direction:column;justify-content:flex-start;min-height:5rem;height:fit-content;background-color:var(--color-background);border-top:1px solid var(--color-border)}div.misc-file[data-v-d773806f]{padding-inline:.5rem;justify-content:space-between;border-bottom:1px solid var(--color-border);background-color:var(--color-background);color:var(--color-text);font-size:.8rem;gap:.5rem;display:flex}.misc-file-op-container[data-v-d773806f]{display:none;gap:.5rem}div.misc-file[data-v-d773806f]:hover{background-color:var(--color-background-theme-highlight)}div.misc-file:hover .misc-file-op-container[data-v-d773806f]{display:flex}button[data-v-d773806f],[data-v-d773806f] button{background-color:var(--color-background);border-radius:0%;width:100%;margin:0;border:.1px solid var(--color-border);height:2rem;color:var(--color-text);cursor:pointer}button[data-v-d773806f]:hover,[data-v-d773806f] button:hover{background-color:var(--color-background-theme-highlight)}label.frontmatter-label[data-v-d773806f]{display:none}a.frontmatter-link[data-v-d773806f]{background-color:var(--color-pure);box-shadow:0 2px 3px 0 var(--color-shadow);border-radius:15px;padding-inline:8px}a.frontmatter-link[data-v-d773806f]:hover{background-color:var(--color-background-theme-highlight)}div#summary-panel-main[data-v-165f5216]{width:100%;height:100%;display:flex;flex-direction:column;text-align:left;padding:10px;background-color:var(--color-background)}h2.title[data-v-165f5216]{font-size:1.2em;font-weight:700;margin:0;padding:0}div.authors-div[data-v-165f5216]{display:flex;flex-wrap:wrap;gap:5px}div.author-container[data-v-165f5216]{display:flex;align-items:center}span.author[data-v-165f5216]{text-decoration:underline;text-underline-offset:3px;white-space:nowrap;font-size:small}span.author-paper-count[data-v-165f5216]{font-size:small;color:var(--color-text-soft);padding-inline:3px;border-radius:5px}span.author-paper-count[data-v-165f5216]:hover{cursor:pointer;background-color:var(--color-background-soft)}div.publication[data-v-165f5216]{font-style:italic;font-size:small}div.docsize span[data-v-165f5216]{font-size:.8em;color:var(--color-text-soft);padding-inline:5px;padding-block:2px;border-radius:5px;border:1px solid var(--color-border)}body[data-v-3d4d3304]{height:100vh}#main-home[data-v-3d4d3304]{margin-top:40px;height:calc(100vh - 50px);width:calc(100vw - 20px);display:flex;flex-direction:column;border:1px solid var(--color-border);border-radius:15px;overflow:hidden;box-shadow:0 0 5px var(--color-shadow)}#main-home.compact[data-v-3d4d3304]{margin-top:30px;height:calc(100vh - 30px);width:100vw;border-radius:0}.panel1[data-v-3d4d3304]{width:100%;height:100%;align-self:center;margin:0}#doc-panel[data-v-3d4d3304]{display:flex;flex-direction:column;width:100%;gap:5px;overflow-x:hidden}div#doc-container[data-v-3d4d3304]{display:flex;flex-direction:column;height:100%}div#doc-top-bar[data-v-3d4d3304]{z-index:1;margin-top:0;padding-top:0;display:flex;justify-content:space-between;box-shadow:0 0 5px 0 var(--color-shadow);border-bottom:1px solid var(--color-border)}#blankPlaceholder[data-v-3d4d3304]{display:flex;flex-direction:column;align-items:center;justify-content:center;height:100%}#blankPlaceholder p[data-v-3d4d3304]{color:var(--color-text-soft);text-align:center;margin:10px}.fullHeight[data-v-3d4d3304]{height:100%}.fullWidth[data-v-3d4d3304]{width:100%}div.horizontal[data-v-3d4d3304]{display:flex}.left-in-enter-active[data-v-3d4d3304],.left-in-leave-active[data-v-3d4d3304]{transition:all 75ms ease-in-out}.left-in-enter-from[data-v-3d4d3304]{opacity:0;transform:translate(-10%)}@media screen and (max-width: 767px){#main-home[data-v-3d4d3304]{width:100vw;margin-top:30px;height:calc(100vh - 40px);border-radius:0;border-left:none;border-right:none}}#authorPapers[data-v-8a4a3cb8]{width:100%;max-height:80vh;min-width:360px}a[data-v-8a4a3cb8]{border-radius:1rem;padding-inline:.5rem;padding-block:.2rem}a[data-v-8a4a3cb8]:hover{cursor:pointer}a.link[data-v-8a4a3cb8]{padding:0}a.link[data-v-8a4a3cb8]:hover{text-decoration:underline;text-underline-offset:.1em;background-color:#0000}div#tag-selector[data-v-8a4a3cb8]{padding:5px 10px}div#feed-main[data-v-8a4a3cb8]{display:flex;align-items:center;padding:1rem;background-color:var(--color-background);border-left:5px solid var(--color-background);border-bottom:1px solid var(--color-border);border-radius:5px}div#feed-main[data-v-8a4a3cb8]:hover{transition:all .3s ease;border-left:5px solid var(--color-theme)}.articleBlock[data-v-8a4a3cb8]{width:90vw;max-width:1200px;display:flex;flex-direction:column;justify-content:flex-start;text-align:justify;gap:.3em}div.titleBlock[data-v-8a4a3cb8]{display:flex;flex-direction:column;align-items:flex-start;text-align:start;flex-wrap:wrap;gap:.25em}label.titleId[data-v-8a4a3cb8],.pubCount[data-v-8a4a3cb8]{color:#1ac4d0c9}span.authorSpan[data-v-8a4a3cb8]{display:inline-block;padding-left:.25em;padding-right:.25em}div.actions[data-v-8a4a3cb8]{display:flex;flex-direction:row;justify-content:flex-start;gap:1em}#relatedArticles[data-v-8a4a3cb8]{display:flex;flex-direction:row;justify-content:space-between;align-items:center;width:100%}label.relatedArticleScore[data-v-8a4a3cb8]{border-radius:5px;padding-left:5px;padding-right:5px;display:flex;align-items:center;justify-content:center;background-color:var(--color-background-theme-highlight)}#main[data-v-ed7e2b2f]{margin-top:40px;width:min(1200px,100vw - 20px);min-height:calc(100vh - 40px);display:flex;flex-direction:column;justify-content:flex-start}div#loadingPlaceholder[data-v-ed7e2b2f]{display:flex;flex-direction:column;justify-content:center;align-items:center;flex-grow:1}div#settings[data-v-ed7e2b2f]{display:flex;flex-direction:column;justify-content:center;align-items:center;gap:.5rem}div#settings input[data-v-ed7e2b2f],div#settings select[data-v-ed7e2b2f]{height:1.5rem;border-radius:.5rem;padding-inline:1rem;background-color:var(--color-background-soft);border:none;color:var(--color-text)}div#settings select[data-v-ed7e2b2f]{min-width:2rem;max-width:8rem;font-weight:700}div#settings input[type=text][data-v-ed7e2b2f]{height:2rem;border-radius:1rem;width:100%;margin-block:.5rem}h1[data-v-ed7e2b2f]{font-weight:700}img.icon[data-v-ed7e2b2f]{height:20px;filter:invert(.5) opacity(.35) drop-shadow(0 0 0 var(--color-border));transition:all .2s;cursor:pointer}img.icon.spin[data-v-ed7e2b2f]{animation:spin 1s linear infinite}img.icon[data-v-ed7e2b2f]:hover{filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-theme))}.error[data-v-34f6e322]{color:red}div.main[data-v-34f6e322]{text-align:center}div#login[data-v-34f6e322]{border:1px solid var(--color-border);box-shadow:0 3px 5px var(--color-shadow);border-radius:15px;padding:15px;text-align:center;background-color:var(--color-background-ssoft);margin-bottom:.5rem}input[type=text][data-v-34f6e322],input[type=password][data-v-34f6e322]{font-family:Gill Sans,sans-serif;font-size:medium;border-radius:1rem;min-width:8rem;border:1px solid var(--color-border);background-color:var(--color-background);transition:all .3s;padding-inline:.8rem;height:2rem}input[data-v-34f6e322]:focus{outline:none;border:1px solid var(--color-theme)}div.loginLine[data-v-34f6e322]{margin-top:.5rem}div.loginLine label[data-v-34f6e322]{font-weight:700}div.options[data-v-34f6e322]{margin:5px;display:flex;gap:10px}button[data-v-34f6e322]{width:100%;margin-top:.5rem;border-radius:1rem;height:2rem}input.key-input[data-v-34f6e322]{width:275px}details[data-v-34f6e322]{padding:5px}div#settings[data-v-34f6e322]{border-radius:5px;background-color:var(--color-background-mute);padding:5px}details summary[data-v-34f6e322]{text-align:left}details input[data-v-34f6e322]{width:160px}#port[data-v-34f6e322]{display:inline-block;width:50px}#registration-form[data-v-892e7367]{margin:0 auto;text-align:left;padding:1rem;padding-inline:1.5rem}#registration-form button[data-v-892e7367]{width:100%;height:2.5rem;margin-top:1rem;border-radius:1.25rem;border:1px solid var(--color-border);background-color:var(--color-background-ssoft);transition:all .3s;font-size:medium;cursor:pointer;box-shadow:0 2px 3px var(--color-shadow)}#registration-form button[data-v-892e7367]:hover{background-color:var(--color-background-theme)}td.horizontal[data-v-892e7367]{display:flex;flex-direction:row;gap:.5rem;align-items:center}#form-container[data-v-892e7367]{display:flex;flex-direction:column;gap:.25rem}.form-elem[data-v-892e7367]{display:flex;flex-direction:column-reverse}.form-elem span[data-v-892e7367]{margin-left:.5rem;font-size:small;color:var(--color-text)}.form-elem input[data-v-892e7367]{font-family:Gill Sans,sans-serif;font-size:medium;border-radius:1rem;min-width:8rem;border:1px solid var(--color-border);background-color:var(--color-background);transition:all .3s;padding-inline:.5rem;height:2rem}.form-elem input[data-v-892e7367]:focus{outline:none;border:1px solid var(--color-theme)}.form-elem input:focus+span[data-v-892e7367]{color:var(--color-theme)}div#show-password-container[data-v-892e7367]{margin-top:.5rem;display:flex;flex-direction:row;gap:.2rem;align-items:center}#login-main[data-v-def42eb3]{display:flex;height:100vh;width:100vw;justify-content:center;align-items:center}#info[data-v-def42eb3]{bottom:0;right:0;margin:.5em;font-size:smaller}div#login-main a[data-v-def42eb3]{cursor:pointer;padding-inline:.5rem;border-radius:.5rem}div#body[data-v-c3f015a3]{width:100%;height:100%}iframe[data-v-c3f015a3]{width:100%;height:100%;padding:0;margin:0}@media only screen and (max-width: 767px){iframe[data-v-c3f015a3]{border-radius:0}}div#main-reader[data-v-39571ec0]{bottom:0;padding-top:0;position:fixed;top:30px;left:0;right:0;background-color:var(--color-background)}@media only screen and (max-width: 767px){div#main-reader[data-v-39571ec0]{padding:0}}div#toolbarOps[data-v-39571ec0]{display:flex;align-items:center;justify-content:center}div#recently-read[data-v-39571ec0]{display:flex;align-items:center;justify-content:center;padding:0 10px;border-radius:5px;background-color:var(--color-background);color:var(--color-text);font-size:.8em;font-weight:700;cursor:pointer;text-wrap:nowrap;white-space:nowrap;overflow-x:hidden}div.horizontal[data-v-ab4897ef]{display:flex;flex-direction:row;align-items:center;gap:10px}h2[data-v-ab4897ef]{white-space:nowrap}div.center[data-v-ab4897ef]{display:flex;justify-content:center;align-items:center}div.full-width[data-v-ab4897ef]{width:100%}div.full-height[data-v-ab4897ef]{height:100%}div.left-align[data-v-ab4897ef]{text-align:left}img.avatar[data-v-ab4897ef]{width:32px;height:32px;border-radius:50%}label.admin_hint[data-v-ab4897ef]{font-size:small;font-weight:700;padding:3px 5px;border-radius:7px;background-color:var(--color-background-theme);color:var(--color-theme)}div#user-widget-header[data-v-ab4897ef]{display:flex;flex-direction:row;justify-content:center;align-items:center;gap:10px}div#user-widget-header b[data-v-ab4897ef]{font-weight:bolder;font-size:x-large}div#add-user-div[data-v-ab4897ef]{margin-top:5px;width:25px;height:25px;display:flex;justify-content:center;align-items:center;border-radius:5px;border:2px solid var(--color-border);background-color:var(--color-background-ssoft);font-weight:bolder;opacity:30%;transition:opacity .25s;transition-delay:.1s;cursor:pointer}div#add-user-div[data-v-ab4897ef]:hover{opacity:90%}table[data-v-ab4897ef]{border-collapse:collapse}tr.user-line[data-v-ab4897ef]:hover{border-radius:5px}tr.user-line[data-v-ab4897ef]:hover{background-color:var(--color-background-theme)}th[data-v-ab4897ef]{font-weight:700;text-align:center;vertical-align:middle;justify-self:center;padding:2px 5px}td[data-v-ab4897ef]{text-align:center;vertical-align:middle;justify-self:center;padding:2px 5px}td.username[data-v-ab4897ef]{font-weight:700;font-size:smaller;color:var(--color-text-soft)}b[data-v-ab4897ef]{font-weight:700}img.icon[data-v-ab4897ef]{height:20px;filter:invert(.5) opacity(.75) drop-shadow(0 0 0 var(--color-border))}div.edit-button[data-v-ab4897ef]{border-radius:30%;width:20px;height:20px;cursor:pointer;opacity:30%}div.edit-button[data-v-ab4897ef]:hover{opacity:100%}div#user-editor-main[data-v-ab4897ef]{padding-inline:2rem;padding-block:1rem;display:flex;flex-direction:column;align-items:flex-start;gap:10px}img.avatar-big[data-v-ab4897ef]{width:128px;height:128px;border-radius:5%}div#user-editor[data-v-ab4897ef]{display:flex;flex-direction:column;align-items:flex-start;gap:10px}div#mandatory-tag-edit[data-v-ab4897ef]{padding-left:5px;padding-right:5px;width:100%;border-radius:8px;background-color:var(--color-background)}div#delete-user-dialog-main[data-v-ab4897ef]{padding:10px;padding-inline:2rem}input[type=button]#delete-user-button[data-v-ab4897ef]{padding:5px;border-radius:5px;border:1px solid var(--color-border);background-color:var(--color-red-transparent);color:var(--color-danger);font-weight:700;width:100%}input[type=button]#delete-user-button[data-v-ab4897ef]:hover{background-color:var(--color-danger-hover)}input[type=text]#delete-user-input[data-v-ab4897ef]{padding:5px;border-radius:5px;border:1px solid var(--color-border)}div#create-user-main[data-v-ab4897ef]{padding-inline:1rem;padding-block:.7rem}table#create-user-table[data-v-ab4897ef]{width:100%;border-collapse:collapse}table#create-user-table tr td[data-v-ab4897ef]{text-align:left}input[type=text].create-user-input[data-v-ab4897ef]{padding:5px;width:100%;background-color:var(--color-background);min-width:200px}input[type=number][data-v-ab4897ef]{padding:5px;width:100%;background-color:var(--color-background);min-width:200px;border:none;color:var(--color-text);border-radius:5px}h1[data-v-2f65f22c]{font-size:2rem;font-weight:700;margin-top:1rem;padding-block:.8rem}h2[data-v-2f65f22c]{font-weight:700;margin-top:1rem;padding-block:.8rem;border-top:1px solid var(--color-border)}a[data-v-2f65f22c]{text-underline-offset:2px}a[data-v-2f65f22c]:hover{text-decoration:underline;background-color:unset}div#about-main[data-v-2f65f22c]{display:flex;flex-direction:column;justify-content:center;align-items:center;max-width:900px;margin-top:40px}b[data-v-2f65f22c]{font-weight:700}div.content[data-v-2f65f22c]{padding-inline:1rem;width:100%;text-align:left}div#versionHistory[data-v-2f65f22c]{padding:20px;display:flex;flex-direction:column}div#block[data-v-2f65f22c]{display:flex;flex-direction:column;justify-content:flex-start;align-items:flex-start}hr[data-v-2f65f22c]{width:100%;margin-top:10px;margin-bottom:10px;border:1px solid var(--color-border);border-top:none}summary[data-v-2f65f22c]{cursor:pointer;-webkit-user-select:none;user-select:none}div.link-container[data-v-2f65f22c]{display:flex;flex-direction:row;justify-content:center;align-items:center;margin-top:1rem;border:1px solid var(--color-border);border-radius:3rem;padding:.3rem;gap:.5rem;white-space:nowrap;width:100%}div#widget-container-main[data-v-257ac3c4]{box-shadow:0 2px 3px 0 var(--color-shadow);background-color:var(--color-background);border:1px solid var(--color-border);border-radius:20px;padding:20px;display:flex;align-items:center;justify-content:center;flex-wrap:wrap;flex-direction:row;max-width:1200px}@media only screen and (max-width: 767px){div#widget-container-main[data-v-257ac3c4]{border-radius:0;border:none;box-shadow:none;padding:0}}div#main-dashboard[data-v-6b501763]{margin-top:65px;display:flex;align-items:flex-start;flex-wrap:wrap;justify-content:center;flex-direction:row;width:calc(100vw - 20px);gap:20px}div.test[data-v-3b8741a7]{margin-top:1rem;font-size:medium}table[data-v-3b8741a7]{width:100%;border:1px solid var(--color-border);border-collapse:collapse}td[data-v-3b8741a7]{padding:.5rem;text-align:left;border:1px solid var(--color-border)}div.test form[data-v-3b8741a7]{display:flex;flex-direction:column;gap:.5rem}div.test form label[data-v-3b8741a7]{margin-top:.5rem}button[data-v-3b8741a7]{width:100%;height:2rem}input[data-v-3b8741a7],select[data-v-3b8741a7]{width:100%;height:1.8rem;border:1px solid var(--color-border)}
```

### Comparing `Lires-1.8.2/lires_web/dist/assets/js-yaml-B7yGoGZD.js` & `Lires-1.8.3/lires_web/dist/assets/js-yaml-B7yGoGZD.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/kind-of-l3izQsJJ.js` & `Lires-1.8.3/lires_web/dist/assets/kind-of-l3izQsJJ.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/linkify-it-DmNjr4Kv.js` & `Lires-1.8.3/lires_web/dist/assets/linkify-it-DmNjr4Kv.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/markdown-it-DI8MEbma.js` & `Lires-1.8.3/lires_web/dist/assets/markdown-it-DI8MEbma.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/markdown-it-image-figures-BD49Kf-b.js` & `Lires-1.8.3/lires_web/dist/assets/markdown-it-image-figures-BD49Kf-b.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/markdown-it-task-lists-BNI9E7ji.js` & `Lires-1.8.3/lires_web/dist/assets/markdown-it-task-lists-BNI9E7ji.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/markdown-it-xss-DEpVfk-m.js` & `Lires-1.8.3/lires_web/dist/assets/markdown-it-xss-DEpVfk-m.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/md-editor-v3-92WZKX8v.css` & `Lires-1.8.3/lires_web/dist/assets/md-editor-v3-92WZKX8v.css`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/md-editor-v3-CPol1xJ_.js` & `Lires-1.8.3/lires_web/dist/assets/md-editor-v3-CPol1xJ_.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/mdurl-k9Sl0PQj.js` & `Lires-1.8.3/lires_web/dist/assets/mdurl-k9Sl0PQj.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/medium-zoom-bWEtUbjf.js` & `Lires-1.8.3/lires_web/dist/assets/medium-zoom-bWEtUbjf.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/pinia-BHWH00Pk.js` & `Lires-1.8.3/lires_web/dist/assets/pinia-BHWH00Pk.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/plotly.js-dist-FakLekxN.js` & `Lires-1.8.3/lires_web/dist/assets/plotly.js-dist-FakLekxN.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/punycode.js-Dj65hjkv.js` & `Lires-1.8.3/lires_web/dist/assets/punycode.js-Dj65hjkv.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/section-matter-DWrNKXO4.js` & `Lires-1.8.3/lires_web/dist/assets/section-matter-DWrNKXO4.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/strnum-u8jQhLSb.js` & `Lires-1.8.3/lires_web/dist/assets/strnum-u8jQhLSb.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/style-mod-Bc2inJdb.js` & `Lires-1.8.3/lires_web/dist/assets/style-mod-Bc2inJdb.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/uc.micro-kMc2yuuw.js` & `Lires-1.8.3/lires_web/dist/assets/uc.micro-kMc2yuuw.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/vite-plugin-node-polyfills-Cgl3E5jI.js` & `Lires-1.8.3/lires_web/dist/assets/vite-plugin-node-polyfills-Cgl3E5jI.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/vue-router-DNoSD41y.js` & `Lires-1.8.3/lires_web/dist/assets/vue-router-DNoSD41y.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/w3c-keyname-Vcq4gwWv.js` & `Lires-1.8.3/lires_web/dist/assets/w3c-keyname-Vcq4gwWv.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/assets/xss-DnjGkJ2-.js` & `Lires-1.8.3/lires_web/dist/assets/xss-DnjGkJ2-.js`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/favicon.ico` & `Lires-1.8.3/lires_web/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `Lires-1.8.2/lires_web/dist/index.html` & `Lires-1.8.3/lires_web/dist/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
-    <link rel="icon" href="/favicon.ico">
-    <link rel="apple-touch-icon" href="/favicon.ico">
-    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
+    <!--<link rel="icon" href="/favicon.ico">-->
+    <link rel="manifest" href="/site.manifest.json" />
+
+    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
+
+    <meta rel="apple-touch-icon" href="/assets/icons/apple-touch-icon.png">
     <meta name="apple-mobile-web-app-capable" content="yes">
     <meta name="apple-mobile-web-app-status-bar-style" content="black">
+    <link name="apple-mobile-web-app-title" content="Lires">
     <title>Lires</title>
-    <script type="module" crossorigin src="/assets/index-DVZewPDh.js"></script>
+    <script type="module" crossorigin src="/assets/index-Tvuvqxrm.js"></script>
     <link rel="modulepreload" crossorigin href="/assets/vite-plugin-node-polyfills-Cgl3E5jI.js">
     <link rel="modulepreload" crossorigin href="/assets/@vue-D_lT-ze_.js">
     <link rel="modulepreload" crossorigin href="/assets/pinia-BHWH00Pk.js">
     <link rel="modulepreload" crossorigin href="/assets/vue-router-DNoSD41y.js">
     <link rel="modulepreload" crossorigin href="/assets/async-mutex-CSJywVGb.js">
     <link rel="modulepreload" crossorigin href="/assets/strnum-u8jQhLSb.js">
     <link rel="modulepreload" crossorigin href="/assets/fast-xml-parser-CJG3bOwu.js">
@@ -43,13 +47,13 @@
     <link rel="modulepreload" crossorigin href="/assets/is-extendable-CiA4f1iz.js">
     <link rel="modulepreload" crossorigin href="/assets/extend-shallow-DA8A8LGH.js">
     <link rel="modulepreload" crossorigin href="/assets/section-matter-DWrNKXO4.js">
     <link rel="modulepreload" crossorigin href="/assets/js-yaml-B7yGoGZD.js">
     <link rel="modulepreload" crossorigin href="/assets/strip-bom-string-BxrG9K6S.js">
     <link rel="modulepreload" crossorigin href="/assets/gray-matter-D4hcLa5V.js">
     <link rel="stylesheet" crossorigin href="/assets/md-editor-v3-92WZKX8v.css">
-    <link rel="stylesheet" crossorigin href="/assets/index-Umoxfe5H.css">
+    <link rel="stylesheet" crossorigin href="/assets/index-Bzo7HIUU.css">
   </head>
   <body>
     <div id="app"></div>
   </body>
 </html>
```

### Comparing `Lires-1.8.2/pyproject.toml` & `Lires-1.8.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "wheel", "pyyaml"]
+requires = ["setuptools", "wheel", "pyyaml", "pybind11"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 "lires" = "lires.exec:run"
-"lrs-reset" = "lires.cmd.generateDefaultConf:run"
+"lrs-config" = "lires.cmd.config:run"
 "lrs-utils" = "lires.cmd.miscUtils:main"
 "lrs-clear" = "lires.cmd.clear:main"
 "lrs-log" = "lires.cmd.log:main"
 "lrs-user" = "lires.cmd.userManage:run"
 "lrs-invite" = "lires.cmd.invite:run"
 "lrs-index" = "lires.cmd.index:main"
 "lrs-cluster" = "lires.cmd.cluster:main"
@@ -43,15 +43,14 @@
     "pyyaml",
     "aiohttp",
     "deprecated",
 ]
 
 [project.optional-dependencies]
 core = [
-    "tiny_vectordb >= 0.1.9",
     "pybtex",
     "pylatexenc",
     "tornado",
     "fastapi",
     "uvicorn",
     "aiofiles",
     "aiosqlite",
```

### Comparing `Lires-1.8.2/requirements.py` & `Lires-1.8.3/requirements.py`

 * *Files identical despite different names*

