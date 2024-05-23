# Comparing `tmp/wwpdb_utils_dp-0.51.tar.gz` & `tmp/wwpdb_utils_dp-0.51.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_utils_dp-0.51.tar", last modified: Sun Apr 28 10:15:06 2024, max compression
+gzip compressed data, was "wwpdb_utils_dp-0.51.1.dev1.tar", last modified: Thu May 23 12:01:37 2024, max compression
```

## Comparing `wwpdb_utils_dp-0.51.tar` & `wwpdb_utils_dp-0.51.1.dev1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/
--rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2215 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.758348 wwpdb_utils_dp-0.51/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.762348 wwpdb_utils_dp-0.51/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/DepositorSyncUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5366 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxModelComplexity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)   212032 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-04-28 10:13:55.000000 wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-28 10:15:06.770349 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      959 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-28 10:14:52.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-28 10:15:06.000000 wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2215 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.801035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.801035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5366 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxModelComplexity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   212836 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      161 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 12:01:24.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb_utils_dp-0.51/LICENSE` & `wwpdb_utils_dp-0.51.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/PKG-INFO` & `wwpdb_utils_dp-0.51.1.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.51
+Version: 0.51.1.dev1
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_dp-0.51/setup.py` & `wwpdb_utils_dp-0.51.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/DepositorSyncUtil.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DepositorSyncUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxModelComplexity.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxModelComplexity.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         description="Calculates the complexity of a model file and outputs a CIF file with information",
     )
     parser.add_argument("--model", required=True, help="model file to calculate complexity")
     parser.add_argument("--output", required=True, help="output file to record complexity")
     parser.add_argument(
         "--threshold",
         type=float,
-        default=1e6,
+        default=1e8,
         help="threshold value to use as cutoff (1.0E+6 default)",
     )
     args = parser.parse_args()
 
     threshold = args.threshold
     modelpath = args.model
     output = args.output
```

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files 0% similar despite different names*

```diff
@@ -2567,15 +2567,15 @@
                 "struct_sheet_range",
                 "struct_conn",
                 "struct_site",
                 "struct_site_gen",
             ]
 
             strpCt = PdbxStripCategory(verbose=self.__verbose, log=self.__lfh)
-            strpCt.strip(oPath2Full, oPathFull, stripList)
+            strpCt.strip(oPath2Full, oPathFull, stripList)  # This is defined for this op  # pylint: disable=used-before-assignment
 
         if (op == "annot-rcsb2pdbx-strip") or (op == "annot-rcsbeps2pdbx-strip"):
             # remove these derived categories for now --
             stripList = [
                 "pdbx_coord",
                 "pdbx_nonstandard_list",
                 "pdbx_protein_info",
@@ -2682,15 +2682,15 @@
             if op == "annot-wwpdb-validate-all-v2":
                 if os.access(edmapCoefPath, os.F_OK):
                     self.__resultPathList.append(edmapCoefPath)
                 else:
                     self.__resultPathList.append("missing")
 
             # Cleanup workdir
-            if deleteRunDir:
+            if deleteRunDir:  # This is defined for this op  # pylint: disable=used-before-assignment
                 try:
                     logger.info("+RcsbDpUtility.__annotationStep() removing working path %s\n", runDir)
                     shutil.rmtree(runDir, ignore_errors=True)
                     return True
                 except Exception:
                     logger.info("+RcsbDpUtility.__annotationStep() removal failed for working path %s\n", runDir)
 
@@ -2709,25 +2709,25 @@
             #
 
         elif op == "annot-sf-convert":
             self.__resultPathList = []
             #
             # Push the output converted and diagnostic files onto the resultPathList.
             #
-            if os.access(sfCifPath, os.F_OK):
+            if os.access(sfCifPath, os.F_OK):  # This is defined for this op  # pylint: disable=used-before-assignment
                 self.__resultPathList.append(sfCifPath)
             else:
                 self.__resultPathList.append("missing")
 
-            if os.access(sfDiagPath, os.F_OK):
+            if os.access(sfDiagPath, os.F_OK):  # This is defined for this op  # pylint: disable=used-before-assignment
                 self.__resultPathList.append(sfDiagPath)
             else:
                 self.__resultPathList.append("missing")
 
-            if os.access(mtzDmpPath, os.F_OK):
+            if os.access(mtzDmpPath, os.F_OK):  # This is defined for this op  # pylint: disable=used-before-assignment
                 self.__resultPathList.append(mtzDmpPath)
             else:
                 self.__resultPathList.append("missing")
 
         elif op == "annot-make-maps":
             #
             self.__resultPathList = []
@@ -2776,15 +2776,15 @@
                     if os.access(fp, os.R_OK):
                         self.__resultPathList.append(fp)
 
         elif op == "annot-make-ligand-maps":
             # Here we manage copying the maps non-polymer CIF snippets and a defining index file to the user
             # specified output path --
             if self.__verbose:
-                logger.info("+RcsbDpUtility._annotationStep()  - for operation %s return path %s\n", op, outDataPathFull)
+                logger.info("+RcsbDpUtility._annotationStep()  - for operation %s return path %s\n", op, outDataPathFull)  # Is defined for op  # pylint: disable=used-before-assignment
             pat = os.path.join(self.__wrkPath, "*.map")
             self.__resultMapPathList = glob.glob(pat)
             if self.__debug:
                 logger.info("+RcsbDpUtility._annotationStep()  - pat %s resultMapPathList %s\n", pat, self.__resultMapPathList)
             #
             pat = os.path.join(self.__wrkPath, "[0-9]*.cif")
             self.__resultCifPathList = glob.glob(pat)
@@ -2793,15 +2793,15 @@
             #
             try:
                 if not os.path.isdir(outDataPathFull):
                     os.makedirs(outDataPathFull, 0o755)
                 # index file --
                 ipT = os.path.join(self.__wrkPath, "LIG_PEPTIDE.cif")
                 if os.access(ipT, os.R_OK):
-                    shutil.copyfile(ipT, outIndexPathFull)
+                    shutil.copyfile(ipT, outIndexPathFull)  # This is defined for this op  # pylint: disable=used-before-assignment
                 else:
                     if self.__verbose:
                         logger.info("+RcsbDpUtility._annotationStep()  - missing map index file %s\n", ipT)
 
                 # map files
                 for fp in self.__resultMapPathList:
                     if fp.endswith("_2fofc.map"):
@@ -2822,15 +2822,15 @@
                         logger.info("+RcsbDpUtility._annotationStep()  - returning cif snippet file %s\n", ofp)
 
             except Exception as e:
                 logger.exception("_annotationStep() - failing return of files for operation %s with %s", op, str(e))
 
         elif op in ["annot-chem-shifts-atom-name-check", "annot-chem-shifts-upload-check"]:
             if os.access(lCheckPath, os.R_OK):
-                shutil.copyfile(lCheckPath, chkPath)
+                shutil.copyfile(lCheckPath, chkPath)  # This is defined for this op  # pylint: disable=used-before-assignment
             #
 
         elif op == "annot-depict-molecule-json":
             self.__resultPathList = []
             #
             outFile = os.path.join(self.__wrkPath, oPath)
             if os.access(outFile, os.F_OK):
@@ -3427,14 +3427,18 @@
             cmd = f"python -m wwpdb.utils.emdb.checkemupload.checkemupload {inpMapFilePath}"
             if inpModelFilePath:
                 cmd += f" --model {inpModelFilePath}"
             if inpHalfMapFilePath1 and inpHalfMapFilePath2:
                 cmd += f" --halfmaps {inpHalfMapFilePath1} {inpHalfMapFilePath2}"
             if outFilePath:
                 cmd += f" --output {outFilePath}"
+            cmd += f" 2> {ePath} 1> {oPath}"
+            cmd += f" ; cat {ePath} > {lPath}"
+            cmd += f" ; cat {oPath} >> {lPath}"
+
         else:
             pass
 
         if op not in (
             "em2em-spider",
             "mapfix-big",
             "fsc_check",
@@ -3781,15 +3785,15 @@
                 sDictSdb = self.__nameToDictPath("deposit")
                 dDictSdb = self.__nameToDictPath("archive_current")
             elif dictName == "archive_next":
                 sDictSdb = self.__nameToDictPath("archive_next")
                 dDictSdb = self.__nameToDictPath("archive_next")
 
             cmdPath = os.path.join(self.__packagePath, "dict", "bin", "cifexch2")
-            thisCmd = " ; " + cmdPath + " -dicSdb " + sDictSdb + " -pdbxDicSdb " + dDictSdb + " -reorder  -strip -op in  -pdbids "
+            thisCmd = " ; " + cmdPath + " -dicSdb " + sDictSdb + " -pdbxDicSdb " + dDictSdb + " -reorder  -strip -op in  -pdbids "  # If not set, crash is ok  # noqa: E501 pylint: disable=possibly-used-before-assignment
             cmd += thisCmd + " -input " + iPath + " -output " + oPath
             cmd += " > " + tPath + " 2>&1 ; cat " + tPath + " >> " + lPath
 
         elif op == "cif2pdbx":
             #   need to have an input file list.
             cmdPath = os.path.join(self.__localAppsPath, "bin", "cifexch-v3.2")
             thisCmd = " ; " + cmdPath + " -ddlodb " + self.__pathDdlSdb + " -dicodb " + self.__pathPdbxDictSdb
```

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/RunRemote.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.51
+Version: 0.51.1.dev1
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_dp-0.51/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

