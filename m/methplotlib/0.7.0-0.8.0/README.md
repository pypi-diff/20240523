# Comparing `tmp/methplotlib-0.7.0.tar.gz` & `tmp/methplotlib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/methplotlib-0.7.0.tar", last modified: Fri Nov 15 14:25:30 2019, max compression
+gzip compressed data, was "dist/methplotlib-0.8.0.tar", last modified: Fri Nov 22 07:56:59 2019, max compression
```

## Comparing `methplotlib-0.7.0.tar` & `methplotlib-0.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:25:30.000000 methplotlib-0.7.0/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       18 2019-01-29 07:23:46.000000 methplotlib-0.7.0/MANIFEST.in
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     3614 2019-11-15 14:25:30.000000 methplotlib-0.7.0/PKG-INFO
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     2505 2019-10-30 09:04:07.000000 methplotlib-0.7.0/README.md
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-01-29 07:23:46.000000 methplotlib-0.7.0/methplotlib/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     4949 2019-10-30 08:25:10.000000 methplotlib-0.7.0/methplotlib/annotation.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib/differential/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:11:34.000000 methplotlib-0.7.0/methplotlib/differential/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1774 2019-11-15 14:13:29.000000 methplotlib-0.7.0/methplotlib/differential/differential.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      400 2019-11-15 14:15:00.000000 methplotlib-0.7.0/methplotlib/helpers.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3158 2019-10-29 15:07:05.000000 methplotlib-0.7.0/methplotlib/import_methylation.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     5835 2019-11-07 07:19:45.000000 methplotlib-0.7.0/methplotlib/methplotlib.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     9246 2019-09-25 06:54:56.000000 methplotlib-0.7.0/methplotlib/plots.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3998 2019-11-13 11:47:42.000000 methplotlib-0.7.0/methplotlib/qc.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3382 2019-09-20 11:09:25.000000 methplotlib-0.7.0/methplotlib/utils.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-11-15 14:11:48.000000 methplotlib-0.7.0/methplotlib/version.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     3614 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      815 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       62 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/entry_points.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       82 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/requires.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       20 2019-11-15 14:25:30.000000 methplotlib-0.7.0/methplotlib.egg-info/top_level.txt
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:25:30.000000 methplotlib-0.7.0/scripts/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:11:34.000000 methplotlib-0.7.0/scripts/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1369 2019-11-15 14:17:53.000000 methplotlib-0.7.0/scripts/allele_specific_modification
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      896 2019-09-11 05:16:33.000000 methplotlib-0.7.0/scripts/annotate_calls_by_phase.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3247 2019-09-25 13:37:46.000000 methplotlib-0.7.0/scripts/calculate_methylation_frequency.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1474 2019-11-15 14:16:23.000000 methplotlib-0.7.0/scripts/differential_modification
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1462 2019-10-29 15:13:16.000000 methplotlib-0.7.0/scripts/genome-wide-QC.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      926 2019-10-29 14:51:00.000000 methplotlib-0.7.0/scripts/sorting_and_multiple_testing_correction.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1956 2019-09-27 13:57:39.000000 methplotlib-0.7.0/scripts/split_calls_by_phase.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       38 2019-11-15 14:25:30.000000 methplotlib-0.7.0/setup.cfg
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1704 2019-11-15 14:11:34.000000 methplotlib-0.7.0/setup.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-22 07:56:59.000000 methplotlib-0.8.0/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       18 2019-01-29 07:23:46.000000 methplotlib-0.8.0/MANIFEST.in
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     3621 2019-11-22 07:56:59.000000 methplotlib-0.8.0/PKG-INFO
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     2512 2019-11-22 07:43:36.000000 methplotlib-0.8.0/README.md
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-22 07:56:59.000000 methplotlib-0.8.0/methplotlib/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-01-29 07:23:46.000000 methplotlib-0.8.0/methplotlib/__init__.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     4831 2019-11-22 07:44:47.000000 methplotlib-0.8.0/methplotlib/annotation.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-22 07:56:59.000000 methplotlib-0.8.0/methplotlib/differential/
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:11:34.000000 methplotlib-0.8.0/methplotlib/differential/__init__.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1774 2019-11-15 14:13:29.000000 methplotlib-0.8.0/methplotlib/differential/differential.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      400 2019-11-15 14:15:00.000000 methplotlib-0.8.0/methplotlib/helpers.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3338 2019-11-22 07:45:37.000000 methplotlib-0.8.0/methplotlib/import_methylation.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     6686 2019-11-22 07:45:12.000000 methplotlib-0.8.0/methplotlib/methplotlib.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     9246 2019-09-25 06:54:56.000000 methplotlib-0.8.0/methplotlib/plots.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3998 2019-11-13 11:47:42.000000 methplotlib-0.8.0/methplotlib/qc.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3674 2019-11-22 07:46:48.000000 methplotlib-0.8.0/methplotlib/utils.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-11-22 07:46:56.000000 methplotlib-0.8.0/methplotlib/version.py
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-22 07:56:59.000000 methplotlib-0.8.0/methplotlib.egg-info/
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     3621 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      815 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       62 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/entry_points.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       82 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/requires.txt
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       20 2019-11-22 07:56:58.000000 methplotlib-0.8.0/methplotlib.egg-info/top_level.txt
+drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-22 07:56:59.000000 methplotlib-0.8.0/scripts/
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)        0 2019-11-15 14:11:34.000000 methplotlib-0.8.0/scripts/__init__.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1369 2019-11-15 14:17:53.000000 methplotlib-0.8.0/scripts/allele_specific_modification
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      896 2019-09-11 05:16:33.000000 methplotlib-0.8.0/scripts/annotate_calls_by_phase.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3247 2019-09-25 13:37:46.000000 methplotlib-0.8.0/scripts/calculate_methylation_frequency.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1474 2019-11-15 14:16:23.000000 methplotlib-0.8.0/scripts/differential_modification
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1462 2019-10-29 15:13:16.000000 methplotlib-0.8.0/scripts/genome-wide-QC.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      926 2019-10-29 14:51:00.000000 methplotlib-0.8.0/scripts/sorting_and_multiple_testing_correction.py
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1956 2019-09-27 13:57:39.000000 methplotlib-0.8.0/scripts/split_calls_by_phase.py
+-rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       38 2019-11-22 07:56:59.000000 methplotlib-0.8.0/setup.cfg
+-rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1704 2019-11-15 14:11:34.000000 methplotlib-0.8.0/setup.py
```

### Comparing `methplotlib-0.7.0/PKG-INFO` & `methplotlib-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methplotlib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Plot methylation data obtained from nanopolish
 Home-page: https://github.com/wdecoster/methplotlib
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.com/wdecoster/methplotlib.svg?branch=master)](https://travis-ci.com/wdecoster/methplotlib)
         [![Anaconda-Server Badge](https://anaconda.org/bioconda/methplotlib/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)
@@ -38,16 +38,16 @@
           --split               split, rather than overlay the methylation frequency tracks
           --smooth SMOOTH       Smoothen the datapoints of frequencies, but reduce the details (integer, default=5)
         ```
         
         ## Snakemake workflow
         For streamlining nanopolish a Snakefile is included (using snakemake). The workflow uses a config file, of which an example is in this repository.
         
-        ## Test data
-        The `test` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
+        ## Example data
+        The `examples` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
         
         ## Companion scripts
         The `scripts` folder contains scripts for phasing modification calls in haplotypes based on [WhatsHap](https://whatshap.readthedocs.io/en/latest/) phasing, allele specific modification testing for phased data and differential modification testing across subjects.
         
         ## TO DO - CONTRIBUTIONS WELCOME
         - Outlier detection (in windows) across samples
```

### Comparing `methplotlib-0.7.0/README.md` & `methplotlib-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   --split               split, rather than overlay the methylation frequency tracks
   --smooth SMOOTH       Smoothen the datapoints of frequencies, but reduce the details (integer, default=5)
 ```
 
 ## Snakemake workflow
 For streamlining nanopolish a Snakefile is included (using snakemake). The workflow uses a config file, of which an example is in this repository.
 
-## Test data
-The `test` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
+## Example data
+The `examples` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
 
 ## Companion scripts
 The `scripts` folder contains scripts for phasing modification calls in haplotypes based on [WhatsHap](https://whatshap.readthedocs.io/en/latest/) phasing, allele specific modification testing for phased data and differential modification testing across subjects.
 
 ## TO DO - CONTRIBUTIONS WELCOME
 - Outlier detection (in windows) across samples
```

### Comparing `methplotlib-0.7.0/methplotlib/annotation.py` & `methplotlib-0.8.0/methplotlib/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import pyranges as pr
 import itertools
 import sys
 from plotly.colors import DEFAULT_PLOTLY_COLORS as plcolors
 import gzip
 import logging
 
 
@@ -116,12 +117,11 @@
     colordict = {g: c for g, c in zip(genes, plcolors * 100)}
     for t in transcripts:
         t.color = colordict[t.gene]
 
 
 def parse_bed(bed, window):
     logging.info("Parsing BED file")
-    df = pd.read_csv(bed, sep="\t", names=['chromosome', 'begin', 'end', 'name', 'score', 'strand'])
-    return df.loc[df['begin'].between(window.begin, window.end)
-                  | df['end'].between(window.begin, window.end)] \
-        .drop(columns=['chromosome', 'score', 'strand']) \
-        .itertuples(index=False, name=None)
+    gr = pr.read_bed(bed)[window.chromosome, window.begin:window.end]
+    df = gr.unstrand().df
+    df = df.drop(columns=["Chromosome", "Score"])
+    return df.itertuples(index=False, name=None)
```

### Comparing `methplotlib-0.7.0/methplotlib/differential/differential.py` & `methplotlib-0.8.0/methplotlib/differential/differential.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/methplotlib/import_methylation.py` & `methplotlib-0.8.0/methplotlib/import_methylation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pandas as pd
+import pyranges as pr
 import numpy as np
 import sys
 import logging
 
 
 class Methylation(object):
     def __init__(self, table, data_type, name, called_sites):
@@ -20,49 +21,55 @@
     smoothening the result by a rolling average
 
     input can also be raw data per read, optionally phased
     which will return a dataframe with 'read', 'chromosome', 'pos', 'log_lik_ratio', 'strand'
     """
     try:
         table = pd.read_csv(filename, sep="\t")
+        gr = pr.PyRanges(table.rename(columns={"start": "Start", "chromosome": "Chromosome",
+                                               "end": "End", "Strand": "strand"}))
         logging.info("Read the file in a dataframe.")
+
         if window:
-            table = table.loc[(table["chromosome"] == window.chromosome) &
-                              table["start"].between(window.begin, window.end)]
-        table["pos"] = np.floor(table[['start', 'end']].mean(axis=1)).astype('i8')
+            gr = gr[window.chromosome, window.begin:window.end]
+        gr.pos = np.floor(gr.drop().df[["Start", "End"]].mean(axis=1))
+        table = gr.df
+
         if 'log_lik_ratio' in table:  # indicating the file is 'raw' or 'phased'
 
-            if 'PS' in table:  # indicating the file contains phased calls
+            table = table.drop(columns=['Start', 'End', 'log_lik_methylated',
+                                        'log_lik_unmethylated', 'num_calling_strands',
+                                        'num_motifs', 'sequence'])
+            if 'PS' in gr:  # indicating the file contains phased calls
                 data_type = 'phased'
                 logging.info("File contains phased raw data.")
             else:
                 data_type = 'raw'
                 logging.info("File contains raw data.")
             return Methylation(
-                table=table.drop(columns=['start', 'end', 'log_lik_methylated',
-                                          'log_lik_unmethylated', 'num_calling_strands',
-                                          'num_motifs', 'sequence'])
-                .sort_values(['read_name', 'pos']),
+                table=table.sort_values(['read_name', 'pos']),
                 data_type=data_type,
                 name=name,
                 called_sites=len(table))
         else:  # assuming the file is from calculate_methylation_frequency
             logging.info("File contains frequency data.")
+            called_sites = table.called_sites
+            table = table.drop(columns=['Start', 'End', 'num_motifs_in_group',
+                                        'called_sites', 'called_sites_methylated',
+                                        'group_sequence'])
             return Methylation(
-                table=table.drop(columns=['start', 'end', 'num_motifs_in_group',
-                                          'called_sites', 'called_sites_methylated',
-                                          'group_sequence'])
+                table=table
                 .sort_values('pos')
                 .groupby('pos')
                 .mean()
                 .rolling(window=smoothen, center=True)
                 .mean(),
                 data_type="frequency",
                 name=name,
-                called_sites=table["called_sites"].sum())
+                called_sites=called_sites.sum())
     except Exception:
         sys.stderr.write("\n\n\nInput file {} not recognized!\n".format(filename))
         sys.stderr.write("\n\n\nDetailed error:\n")
         raise
 
 
 def get_data(methylation_files, names, window, smoothen=5):
```

### Comparing `methplotlib-0.7.0/methplotlib/methplotlib.py` & `methplotlib-0.8.0/methplotlib/methplotlib.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,37 @@
 import methplotlib.qc as qc
 from methplotlib.import_methylation import get_data
 import logging
 
 
 def main():
     args = utils.get_args()
+
+    if args.example:
+        import pkg_resources
+        import sys
+
+        meth = pkg_resources.resource_filename("methplotlib", "examples/ACTB_calls.tsv.gz")
+        meth_freq = pkg_resources.resource_filename("methplotlib", "examples/meth_freq.tsv.gz")
+        bed = pkg_resources.resource_filename("methplotlib", "examples/DNAse_cluster.bed.gz")
+        annotation = pkg_resources.resource_filename("methplotlib", "examples/g38_locus.gtf.gz")
+
+        example = """
+methplotlib -m {meth} \\
+               {meth_freq} \\
+            -n calls frequencies \\
+            -w chr7:5,525,542-5,543,028 \\
+            -g {annotation} \\
+            --simplify \\
+            -b {bed}""".strip().format(meth=meth, meth_freq=meth_freq,
+                                       annotation=annotation, bed=bed)
+
+        print(example)
+        sys.exit(0)
+
     utils.init_logs(args)
     windows = utils.make_windows(args.window)
     for window in windows:
         logging.info("Processing {}".format(window.string))
         meth_data = get_data(args.methylation, args.names, window, args.smooth)
         logging.info("Collected methylation data for {} datasets".format(len(meth_data)))
         qc_plots(meth_data, window)
```

### Comparing `methplotlib-0.7.0/methplotlib/plots.py` & `methplotlib-0.8.0/methplotlib/plots.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/methplotlib/qc.py` & `methplotlib-0.8.0/methplotlib/qc.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/methplotlib/utils.py` & `methplotlib-0.8.0/methplotlib/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,38 +35,41 @@
     parser.add_argument("-v", "--version",
                         help="Print version and exit.",
                         action="version",
                         version='methplotlib {}'.format(__version__))
     parser.add_argument("-m", "--methylation",
                         nargs='+',
                         help="nanopolish methylation calls or frequency output",
-                        required=True)
+                        required=True if "--example" not in sys.argv else False)
     parser.add_argument("-n", "--names",
                         nargs='+',
                         help="names of datasets in --methylation",
-                        required=True)
+                        required=True if "--example" not in sys.argv else False)
     parser.add_argument("-w", "--window",
                         help="window (region) to which the visualisation has to be restricted",
-                        required=True)
+                        required=True if "--example" not in sys.argv else False)
     parser.add_argument("-g", "--gtf",
                         help="add annotation based on a gtf file matching to your reference genome")
     parser.add_argument("-b", "--bed",
                         help="add annotation based on a bed file matching to your reference genome")
     parser.add_argument("--simplify",
                         help="simplify annotation track to show genes rather than transcripts",
                         action="store_true")
     parser.add_argument("--split",
                         help="split, rather than overlay the methylation tracks",
                         action="store_true")
     parser.add_argument("--smooth",
                         help="When plotting frequencies points are averaged using a rolling window",
                         type=int,
                         default=5)
+    parser.add_argument("--example",
+                        action="store_true",
+                        help="Show example command and exit.")
     args = parser.parse_args()
-    if not len(args.names) == len(args.methylation):
+    if not args.example and not len(args.names) == len(args.methylation):
         sys.exit("INPUT ERROR: Expecting the same number of names as datasets!")
     return args
 
 
 def init_logs(args):
     """Initiate log file and log arguments."""
     start_time = dt.fromtimestamp(time()).strftime('%Y%m%d_%H%M')
```

### Comparing `methplotlib-0.7.0/methplotlib.egg-info/PKG-INFO` & `methplotlib-0.8.0/methplotlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methplotlib
-Version: 0.7.0
+Version: 0.8.0
 Summary: Plot methylation data obtained from nanopolish
 Home-page: https://github.com/wdecoster/methplotlib
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: [![Build Status](https://travis-ci.com/wdecoster/methplotlib.svg?branch=master)](https://travis-ci.com/wdecoster/methplotlib)
         [![Anaconda-Server Badge](https://anaconda.org/bioconda/methplotlib/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)
@@ -38,16 +38,16 @@
           --split               split, rather than overlay the methylation frequency tracks
           --smooth SMOOTH       Smoothen the datapoints of frequencies, but reduce the details (integer, default=5)
         ```
         
         ## Snakemake workflow
         For streamlining nanopolish a Snakefile is included (using snakemake). The workflow uses a config file, of which an example is in this repository.
         
-        ## Test data
-        The `test` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
+        ## Example data
+        The `examples` folder contains calls and frequencies for the human ACTB gene from PromethION sequencing of NA19240. An example command is available.
         
         ## Companion scripts
         The `scripts` folder contains scripts for phasing modification calls in haplotypes based on [WhatsHap](https://whatshap.readthedocs.io/en/latest/) phasing, allele specific modification testing for phased data and differential modification testing across subjects.
         
         ## TO DO - CONTRIBUTIONS WELCOME
         - Outlier detection (in windows) across samples
```

### Comparing `methplotlib-0.7.0/methplotlib.egg-info/SOURCES.txt` & `methplotlib-0.8.0/methplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/allele_specific_modification` & `methplotlib-0.8.0/scripts/allele_specific_modification`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/annotate_calls_by_phase.py` & `methplotlib-0.8.0/scripts/annotate_calls_by_phase.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/calculate_methylation_frequency.py` & `methplotlib-0.8.0/scripts/calculate_methylation_frequency.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/differential_modification` & `methplotlib-0.8.0/scripts/differential_modification`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/genome-wide-QC.py` & `methplotlib-0.8.0/scripts/genome-wide-QC.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/sorting_and_multiple_testing_correction.py` & `methplotlib-0.8.0/scripts/sorting_and_multiple_testing_correction.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/scripts/split_calls_by_phase.py` & `methplotlib-0.8.0/scripts/split_calls_by_phase.py`

 * *Files identical despite different names*

### Comparing `methplotlib-0.7.0/setup.py` & `methplotlib-0.8.0/setup.py`

 * *Files identical despite different names*

