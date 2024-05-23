# Comparing `tmp/spit-0.2.3.tar.gz` & `tmp/spit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spit-0.2.3.tar", last modified: Thu May  9 04:50:57 2024, max compression
+gzip compressed data, was "dist/spit-0.2.4.tar", last modified: Thu May 23 05:21:49 2024, max compression
```

## Comparing `spit-0.2.3.tar` & `spit-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:50:57.000000 spit-0.2.3/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-22 00:49:28.000000 spit-0.2.3/LICENSE
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-22 00:49:28.000000 spit-0.2.3/MANIFEST.in
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:50:57.000000 spit-0.2.3/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-22 00:49:28.000000 spit-0.2.3/README.md
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2024-05-09 04:50:57.000000 spit-0.2.3/setup.cfg
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2024-05-09 04:50:46.000000 spit-0.2.3/setup.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:50:57.000000 spit-0.2.3/spit/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.3/spit/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-22 00:49:28.000000 spit-0.2.3/spit/cluster_samples.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-22 00:49:28.000000 spit-0.2.3/spit/confounding_analysis.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    12927 2024-04-25 05:59:48.000000 spit-0.2.3/spit/dtu_detection.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     9555 2023-12-22 00:49:28.000000 spit-0.2.3/spit/filter_and_transform_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-22 00:49:28.000000 spit-0.2.3/spit/get_p_cutoff.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1723 2023-12-22 00:49:28.000000 spit-0.2.3/spit/import_infreps.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:50:57.000000 spit-0.2.3/spit/parameter_fitting/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4563 2024-04-25 01:46:05.000000 spit-0.2.3/spit/parameter_fitting/LOOCV.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.3/spit/parameter_fitting/__init__.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-22 00:49:28.000000 spit-0.2.3/spit/parameter_fitting/filter_and_simulate_tx_counts.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     7033 2024-04-14 19:07:27.000000 spit-0.2.3/spit/parameter_fitting/simulate_dtu_exp.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     4713 2024-04-25 01:36:00.000000 spit-0.2.3/spit/plot_spit_charts.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:50:57.000000 spit-0.2.3/spit/r_scripts/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     3254 2024-03-12 02:48:44.000000 spit-0.2.3/spit/r_scripts/hclust.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-22 00:49:28.000000 spit-0.2.3/spit/r_scripts/tximport_quant_files.R
--rw-r--r--   0 berilerdogdu   (501) staff       (20)    13315 2024-05-09 04:50:36.000000 spit-0.2.3/spit/run_spit.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2024-02-25 23:55:54.000000 spit-0.2.3/spit/spit_test.py
--rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-22 00:49:28.000000 spit-0.2.3/spit/transform_tx_counts_to_ifs.py
-drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/PKG-INFO
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/SOURCES.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/dependency_links.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)       45 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/entry_points.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/requires.txt
--rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2024-05-09 04:50:57.000000 spit-0.2.3/spit.egg-info/top_level.txt
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-23 05:21:49.000000 spit-0.2.4/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    35149 2023-12-22 00:49:28.000000 spit-0.2.4/LICENSE
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       78 2023-12-22 00:49:28.000000 spit-0.2.4/MANIFEST.in
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-23 05:21:49.000000 spit-0.2.4/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3788 2023-12-22 00:49:28.000000 spit-0.2.4/README.md
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       38 2024-05-23 05:21:49.000000 spit-0.2.4/setup.cfg
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      642 2024-05-23 05:21:03.000000 spit-0.2.4/setup.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-23 05:21:49.000000 spit-0.2.4/spit/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.4/spit/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1173 2023-12-22 00:49:28.000000 spit-0.2.4/spit/cluster_samples.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6999 2023-12-22 00:49:28.000000 spit-0.2.4/spit/confounding_analysis.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    12927 2024-04-25 05:59:48.000000 spit-0.2.4/spit/dtu_detection.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     9561 2024-05-23 05:20:42.000000 spit-0.2.4/spit/filter_and_transform_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      773 2023-12-22 00:49:28.000000 spit-0.2.4/spit/get_p_cutoff.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1723 2023-12-22 00:49:28.000000 spit-0.2.4/spit/import_infreps.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-23 05:21:49.000000 spit-0.2.4/spit/parameter_fitting/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4563 2024-04-25 01:46:05.000000 spit-0.2.4/spit/parameter_fitting/LOOCV.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        0 2023-12-22 00:49:28.000000 spit-0.2.4/spit/parameter_fitting/__init__.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6735 2023-12-22 00:49:28.000000 spit-0.2.4/spit/parameter_fitting/filter_and_simulate_tx_counts.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     7033 2024-04-14 19:07:27.000000 spit-0.2.4/spit/parameter_fitting/simulate_dtu_exp.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     4713 2024-04-25 01:36:00.000000 spit-0.2.4/spit/plot_spit_charts.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-23 05:21:49.000000 spit-0.2.4/spit/r_scripts/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     3254 2024-03-12 02:48:44.000000 spit-0.2.4/spit/r_scripts/hclust.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     1326 2023-12-22 00:49:28.000000 spit-0.2.4/spit/r_scripts/tximport_quant_files.R
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)    13315 2024-05-09 04:50:36.000000 spit-0.2.4/spit/run_spit.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     6172 2024-02-25 23:55:54.000000 spit-0.2.4/spit/spit_test.py
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)     2824 2023-12-22 00:49:28.000000 spit-0.2.4/spit/transform_tx_counts_to_ifs.py
+drwxr-xr-x   0 berilerdogdu   (501) staff       (20)        0 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      163 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/PKG-INFO
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      706 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/SOURCES.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        1 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/dependency_links.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)       45 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/entry_points.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)      146 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/requires.txt
+-rw-r--r--   0 berilerdogdu   (501) staff       (20)        5 2024-05-23 05:21:49.000000 spit-0.2.4/spit.egg-info/top_level.txt
```

### Comparing `spit-0.2.3/LICENSE` & `spit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/README.md` & `spit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/setup.py` & `spit-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='spit',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'matplotlib>=3.4.3',
         'matplotlib_venn>=0.11.6',
         'numpy>=1.20.3',
         'pandas>=1.3.4',
```

### Comparing `spit-0.2.3/spit/cluster_samples.py` & `spit-0.2.4/spit/cluster_samples.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/confounding_analysis.py` & `spit-0.2.4/spit/confounding_analysis.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/dtu_detection.py` & `spit-0.2.4/spit/dtu_detection.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/filter_and_transform_tx_counts.py` & `spit-0.2.4/spit/filter_and_transform_tx_counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     final_filtered_gene_counts.to_csv(os.path.join(args.O, "SPIT_analysis", "filtered_gene_counts.txt"), sep = '\t')
     
     if(args.p_dom > 0):
         final_filtered_ifs = final_filtered_ifs.round(2)
         selected_dom_iso_genes = select_genes_w_dom_iso(final_filtered_ifs, ctrl_samples, args.p_dom)
         dominance_selected_ifs = final_filtered_ifs[final_filtered_ifs.gene_id.isin(selected_dom_iso_genes)]
         dominance_selected_gene_counts = final_filtered_gene_counts[final_filtered_gene_counts.index.isin(selected_dom_iso_genes)]
-        dominance_selected_tx_counts = final_filtered_tx_counts[final_filtered_tx_counts.index.isin(selected_dom_iso_genes)]
+        dominance_selected_tx_counts = final_filtered_tx_counts[final_filtered_tx_counts.index.isin(dominance_selected_ifs.index)]
         if(args.write):
             print("After selecting for genes with a dominant transcript in control group:")
             print("\tNumber of transcripts", len(dominance_selected_ifs.index))
             print("\tNumber of genes: ", len(dominance_selected_ifs.gene_id.unique()))
         dominance_selected_ifs.to_csv(os.path.join(args.O, "SPIT_analysis", "dominance_selected_ifs.txt"), sep = '\t')
         dominance_selected_gene_counts.to_csv(os.path.join(args.O, "SPIT_analysis", "dominance_selected_gene_counts.txt"), sep = '\t')
         dominance_selected_tx_counts.to_csv(os.path.join(args.O, "SPIT_analysis", "dominance_selected_tx_counts.txt"), sep = '\t')
```

### Comparing `spit-0.2.3/spit/get_p_cutoff.py` & `spit-0.2.4/spit/get_p_cutoff.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/import_infreps.py` & `spit-0.2.4/spit/import_infreps.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/parameter_fitting/LOOCV.py` & `spit-0.2.4/spit/parameter_fitting/LOOCV.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/parameter_fitting/filter_and_simulate_tx_counts.py` & `spit-0.2.4/spit/parameter_fitting/filter_and_simulate_tx_counts.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/parameter_fitting/simulate_dtu_exp.py` & `spit-0.2.4/spit/parameter_fitting/simulate_dtu_exp.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/plot_spit_charts.py` & `spit-0.2.4/spit/plot_spit_charts.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/r_scripts/hclust.R` & `spit-0.2.4/spit/r_scripts/hclust.R`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/r_scripts/tximport_quant_files.R` & `spit-0.2.4/spit/r_scripts/tximport_quant_files.R`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/run_spit.py` & `spit-0.2.4/spit/run_spit.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/spit_test.py` & `spit-0.2.4/spit/spit_test.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit/transform_tx_counts_to_ifs.py` & `spit-0.2.4/spit/transform_tx_counts_to_ifs.py`

 * *Files identical despite different names*

### Comparing `spit-0.2.3/spit.egg-info/SOURCES.txt` & `spit-0.2.4/spit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

