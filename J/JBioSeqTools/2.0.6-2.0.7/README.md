# Comparing `tmp/JBioSeqTools-2.0.6.tar.gz` & `tmp/JBioSeqTools-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-2.0.6.tar", last modified: Thu May 23 08:44:54 2024, max compression
+gzip compressed data, was "JBioSeqTools-2.0.7.tar", last modified: Thu May 23 08:55:00 2024, max compression
```

## Comparing `JBioSeqTools-2.0.6.tar` & `JBioSeqTools-2.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.321811 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      733 2024-05-23 08:44:53.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2024-05-23 08:44:52.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 08:44:53.000000 JBioSeqTools-2.0.6/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.6/LICENSE
--rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1027 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.331920 JBioSeqTools-2.0.6/jbst/
--rw-rw-rw-   0        0        0     1489 2024-05-23 08:44:07.000000 JBioSeqTools-2.0.6/jbst/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.373246 JBioSeqTools-2.0.6/jbst/data/
--rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/backbone.xlsx
--rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/codons.xlsx
--rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/enzymes.xlsx
--rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/linkers.xlsx
--rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/polya.xlsx
--rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/promoters.xlsx
--rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/regulators.xlsx
--rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/rnai_scoring.xlsx
--rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/selectors.xlsx
--rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/data/sh_loops.xlsx
--rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.6/jbst/data/vector_capacity.xlsx
--rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.6/jbst/data/vectors.xlsx
--rw-rw-rw-   0        0        0    14686 2024-05-22 22:01:35.000000 JBioSeqTools-2.0.6/jbst/install.py
--rw-rw-rw-   0        0        0    99326 2024-05-23 08:39:50.000000 JBioSeqTools-2.0.6/jbst/seq_tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:44:54.380195 JBioSeqTools-2.0.6/jbst/tests/
--rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/tests/__init__.py
--rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.6/jbst/tests/fasta_vector_test.fasta
--rw-rw-rw-   0        0        0   770959 2024-05-22 21:27:37.000000 JBioSeqTools-2.0.6/jbst/tests/jseq_tests.py
--rw-rw-rw-   0        0        0   126514 2024-05-23 08:40:47.000000 JBioSeqTools-2.0.6/jbst/vector_build.py
--rw-rw-rw-   0        0        0       42 2024-05-23 08:44:54.386712 JBioSeqTools-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1600 2024-05-23 08:43:45.000000 JBioSeqTools-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:55:00.529596 JBioSeqTools-2.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-23 08:55:00.476591 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1027 2024-05-23 08:54:58.000000 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2024-05-23 08:54:59.000000 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 08:54:58.000000 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-23 08:54:59.000000 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 08:54:59.000000 JBioSeqTools-2.0.7/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1027 2024-05-23 08:55:00.529596 JBioSeqTools-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 08:55:00.484591 JBioSeqTools-2.0.7/jbst/
+-rw-rw-rw-   0        0        0     1489 2024-05-23 08:54:30.000000 JBioSeqTools-2.0.7/jbst/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:55:00.517355 JBioSeqTools-2.0.7/jbst/data/
+-rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/codons.xlsx
+-rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/enzymes.xlsx
+-rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/polya.xlsx
+-rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/promoters.xlsx
+-rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/rnai_scoring.xlsx
+-rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/selectors.xlsx
+-rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/data/sh_loops.xlsx
+-rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.7/jbst/data/vector_capacity.xlsx
+-rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.7/jbst/data/vectors.xlsx
+-rw-rw-rw-   0        0        0    14686 2024-05-22 22:01:35.000000 JBioSeqTools-2.0.7/jbst/install.py
+-rw-rw-rw-   0        0        0    99099 2024-05-23 08:53:01.000000 JBioSeqTools-2.0.7/jbst/seq_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:55:00.525599 JBioSeqTools-2.0.7/jbst/tests/
+-rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/tests/__init__.py
+-rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.7/jbst/tests/fasta_vector_test.fasta
+-rw-rw-rw-   0        0        0   770959 2024-05-22 21:27:37.000000 JBioSeqTools-2.0.7/jbst/tests/jseq_tests.py
+-rw-rw-rw-   0        0        0   126514 2024-05-23 08:40:47.000000 JBioSeqTools-2.0.7/jbst/vector_build.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 08:55:00.530598 JBioSeqTools-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-05-23 08:54:36.000000 JBioSeqTools-2.0.7/setup.py
```

### Comparing `JBioSeqTools-2.0.6/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-2.0.7/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.6
+Version: 2.0.7
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.6/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-2.0.7/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/LICENSE` & `JBioSeqTools-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/PKG-INFO` & `JBioSeqTools-2.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.6
+Version: 2.0.7
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.6/README.md` & `JBioSeqTools-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/__init__.py` & `JBioSeqTools-2.0.7/jbst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                                     __/ |                                   
                                    |___/                                   
 """
 
 print(pattern)
 
 print('')
-print('Welcome in JBioSeqTools v.2.0.6 library')
+print('Welcome in JBioSeqTools v.2.0.7 library')
 print('')
 print('Loading required packages...')
 
 
 
 
 import os
```

### Comparing `JBioSeqTools-2.0.6/jbst/data/backbone.xlsx` & `JBioSeqTools-2.0.7/jbst/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/codons.xlsx` & `JBioSeqTools-2.0.7/jbst/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/enzymes.xlsx` & `JBioSeqTools-2.0.7/jbst/data/enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/fluorescent_tag.xlsx` & `JBioSeqTools-2.0.7/jbst/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/linkers.xlsx` & `JBioSeqTools-2.0.7/jbst/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/polya.xlsx` & `JBioSeqTools-2.0.7/jbst/data/polya.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/promoters.xlsx` & `JBioSeqTools-2.0.7/jbst/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/regulators.xlsx` & `JBioSeqTools-2.0.7/jbst/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/restriction_enzymes.xlsx` & `JBioSeqTools-2.0.7/jbst/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/rnai_scoring.xlsx` & `JBioSeqTools-2.0.7/jbst/data/rnai_scoring.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/selectors.xlsx` & `JBioSeqTools-2.0.7/jbst/data/selectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/sh_loops.xlsx` & `JBioSeqTools-2.0.7/jbst/data/sh_loops.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/vector_capacity.xlsx` & `JBioSeqTools-2.0.7/jbst/data/vector_capacity.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/data/vectors.xlsx` & `JBioSeqTools-2.0.7/jbst/data/vectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/install.py` & `JBioSeqTools-2.0.7/jbst/install.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/seq_tools.py` & `JBioSeqTools-2.0.7/jbst/seq_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -2161,18 +2161,14 @@
         print('\nLack of restriction places to choose')
         
     return np.asarray(enzyme_list)       
 
 
 
 
-sequence = project['transcripts']['sequences']['vector_sequence'][trans]
-restriction_df = project['transcripts']['sequences']['full_restriction'][trans]
-enzyme_list = project['transcripts']['sequences']['enzymes'][trans] 
-
 
 def repair_sequences(sequence, metadata, restriction_df, enzyme_list, species):
     
     if species.lower() in ['both', 'both2', 'multi']:
         species = 'human'
         
     codons = metadata['codons']
```

### Comparing `JBioSeqTools-2.0.6/jbst/tests/fasta_vector_test.fasta` & `JBioSeqTools-2.0.7/jbst/tests/fasta_vector_test.fasta`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/tests/jseq_tests.py` & `JBioSeqTools-2.0.7/jbst/tests/jseq_tests.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/jbst/vector_build.py` & `JBioSeqTools-2.0.7/jbst/vector_build.py`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.6/setup.py` & `JBioSeqTools-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.6' 
+VERSION = '2.0.7' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the Python library for biological sequence optimization (GC % content & codon frequency), restriction places removal, DNA/RNA structure prediction, and RNAi selection. It also allows the building of many plasmid vectors with the possibility of choosing sequences such as transcript, promoter, enhancer, molecular fluorescent tag, etc. Finally, the user obtains a ready-for-order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
```

