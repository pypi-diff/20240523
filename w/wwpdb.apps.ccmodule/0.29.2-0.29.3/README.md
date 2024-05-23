# Comparing `tmp/wwpdb_apps_ccmodule-0.29.2.tar.gz` & `tmp/wwpdb_apps_ccmodule-0.29.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_ccmodule-0.29.2.tar", last modified: Fri May 10 20:00:02 2024, max compression
+gzip compressed data, was "wwpdb_apps_ccmodule-0.29.3.tar", last modified: Thu May 23 20:26:49 2024, max compression
```

## Comparing `wwpdb_apps_ccmodule-0.29.2.tar` & `wwpdb_apps_ccmodule-0.29.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.031664 wwpdb_apps_ccmodule-0.29.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1262 2024-05-10 20:00:02.031664 wwpdb_apps_ccmodule-0.29.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       80 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-10 20:00:02.031664 wwpdb_apps_ccmodule-0.29.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2595 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.019664 wwpdb_apps_ccmodule-0.29.2/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/
--rw-r--r--   0 vsts      (1001) docker     (127)     5950 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
--rw-r--r--   0 vsts      (1001) docker     (127)   123267 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (127)   105616 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    73678 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12269 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/extract/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/extract/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2951 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/extract/ccOps.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.023664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    94879 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7123 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7305 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12540 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13230 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/
--rw-r--r--   0 vsts      (1001) docker     (127)     4801 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     4885 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2842 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3367 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15516 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompReports.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8568 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/
--rw-r--r--   0 vsts      (1001) docker     (127)    10865 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearch.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13150 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6259 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8708 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/DbSession.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/
--rw-r--r--   0 vsts      (1001) docker     (127)     9350 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6407 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     7201 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28701 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
--rw-r--r--   0 vsts      (1001) docker     (127)      586 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/Exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7960 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/
--rw-r--r--   0 vsts      (1001) docker     (127)     7378 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/ChemCompView.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5748 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)   138698 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    96593 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     4642 2024-05-10 19:58:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-10 20:00:02.027664 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1262 2024-05-10 20:00:01.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2370 2024-05-10 20:00:01.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-10 20:00:01.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-10 19:59:50.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-05-10 20:00:01.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-10 20:00:01.000000 wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1262 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       80 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-23 20:26:49.096454 wwpdb_apps_ccmodule-0.29.3/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2595 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.080454 wwpdb_apps_ccmodule-0.29.3/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.080454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.080454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      153 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.084454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5950 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   123267 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   105616 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    73678 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12269 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.084454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11302 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.084454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/extract/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/extract/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2951 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/extract/ccOps.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.084454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    94879 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7123 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7305 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12540 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13230 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.088454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4801 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     4885 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2842 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3367 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15516 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompReports.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8568 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.088454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10865 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13150 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6259 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8708 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/DbSession.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.088454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/
+-rw-r--r--   0 vsts      (1001) docker     (127)     9350 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6407 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7201 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28701 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1136 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      586 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/Exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7960 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7378 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/ChemCompView.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5748 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)   138829 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    96593 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     4642 2024-05-23 20:25:30.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 20:26:49.092454 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1262 2024-05-23 20:26:48.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2370 2024-05-23 20:26:49.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 20:26:48.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 20:26:33.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-05-23 20:26:48.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-23 20:26:48.000000 wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_ccmodule-0.29.2/PKG-INFO` & `wwpdb_apps_ccmodule-0.29.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.29.2
+Version: 0.29.3
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_apps_ccmodule-0.29.2/setup.py` & `wwpdb_apps_ccmodule-0.29.3/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssign.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/depict/ChemCompDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/depict/ChemCompDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/extract/ccOps.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/extract/ccOps.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompDataExport.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompDataImport.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompEditStore.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/io/ChemCompIo.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/ChemCompReports.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/ChemCompReports.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearch.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/search/DbSession.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/search/DbSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompConfig.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/Exceptions.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/ChemCompView.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/ChemCompView.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -2165,14 +2165,17 @@
             self.__lfh.write("--------------------------------------------\n")
             self.__lfh.write("+ChemCompWebAppWorker.__exitLigMod() - starting\n")
         #
         if (mode == 'completed'):
             state = "closed(0)"
         elif (mode == 'unfinished'):
             state = "waiting"
+        else:
+            state = "unknown"
+            self.__lfh.write("+ChemCompWebAppWorker.__exitLigMod() - unknown state\n")
         #
         bIsWorkflow = self.__isWorkflow()
         #
         self.__getSession()
         sessionId = self.__sessionId
         depId = self.__reqObj.getValue("identifier")
         instId = self.__reqObj.getValue("instance")
```

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb/apps/ccmodule/webapp/wsgi.py` & `wwpdb_apps_ccmodule-0.29.3/wwpdb/apps/ccmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/PKG-INFO` & `wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.29.2
+Version: 0.29.3
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_apps_ccmodule-0.29.2/wwpdb.apps.ccmodule.egg-info/SOURCES.txt` & `wwpdb_apps_ccmodule-0.29.3/wwpdb.apps.ccmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

