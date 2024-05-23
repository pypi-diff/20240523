# Comparing `tmp/kmerdb-0.8.2.tar.gz` & `tmp/kmerdb-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerdb-0.8.2.tar", last modified: Tue May 14 00:19:22 2024, max compression
+gzip compressed data, was "kmerdb-0.8.3.tar", last modified: Thu May 23 20:28:24 2024, max compression
```

## Comparing `kmerdb-0.8.2.tar` & `kmerdb-0.8.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.213420 kmerdb-0.8.2/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.2/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.2/MANIFEST.in
--rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-14 00:19:22.213420 kmerdb-0.8.2/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    13884 2024-04-13 02:30:35.000000 kmerdb-0.8.2/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/kmerdb/
--rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.2/kmerdb/CITATION.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)   108276 2024-05-13 23:36:34.000000 kmerdb-0.8.2/kmerdb/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.2/kmerdb/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    60779 2024-05-13 23:14:16.000000 kmerdb-0.8.2/kmerdb/appmap.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.2/kmerdb/banners.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    14003 2024-05-13 23:07:17.000000 kmerdb-0.8.2/kmerdb/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)  1166202 2024-05-13 23:33:04.000000 kmerdb-0.8.2/kmerdb/distance.c
--rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.2/kmerdb/distance.pyx
--rw-rw-r--   0 matt      (1000) matt      (1000)    40091 2024-05-10 03:18:55.000000 kmerdb-0.8.2/kmerdb/fileutil.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    53348 2024-05-08 05:01:16.000000 kmerdb-0.8.2/kmerdb/graph.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.2/kmerdb/index.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/kmer.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.2/kmerdb/legacy.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/logger.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    19969 2024-04-13 20:20:14.000000 kmerdb-0.8.2/kmerdb/parse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.2/kmerdb/probability.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5632 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/python_distances.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.2/kmerdb/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/kmerdb.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-14 00:19:21.000000 kmerdb-0.8.2/kmerdb.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.2/kmerdb.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4635 2024-05-10 03:20:49.000000 kmerdb-0.8.2/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-05-14 00:19:22.213420 kmerdb-0.8.2/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-05-10 03:21:06.000000 kmerdb-0.8.2/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/test/
--rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.2/test/test_kmer.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 20:28:24.182445 kmerdb-0.8.3/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.3/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.3/MANIFEST.in
+-rw-r--r--   0 matt      (1000) matt      (1000)    30696 2024-05-23 20:28:24.182445 kmerdb-0.8.3/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    14673 2024-05-23 20:23:13.000000 kmerdb-0.8.3/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 20:28:24.182445 kmerdb-0.8.3/kmerdb/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.3/kmerdb/CITATION.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)   108843 2024-05-23 17:07:31.000000 kmerdb-0.8.3/kmerdb/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.3/kmerdb/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    61002 2024-05-23 16:44:05.000000 kmerdb-0.8.3/kmerdb/appmap.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.3/kmerdb/banners.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13977 2024-05-23 20:26:48.000000 kmerdb-0.8.3/kmerdb/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)  1166202 2024-05-23 17:09:04.000000 kmerdb-0.8.3/kmerdb/distance.c
+-rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.3/kmerdb/distance.pyx
+-rw-rw-r--   0 matt      (1000) matt      (1000)    40129 2024-05-23 17:02:08.000000 kmerdb-0.8.3/kmerdb/fileutil.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    53438 2024-05-23 17:01:04.000000 kmerdb-0.8.3/kmerdb/graph.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.3/kmerdb/index.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22838 2024-05-14 11:43:27.000000 kmerdb-0.8.3/kmerdb/kmer.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.3/kmerdb/legacy.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-13 02:29:52.000000 kmerdb-0.8.3/kmerdb/logger.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    19969 2024-04-13 20:20:14.000000 kmerdb-0.8.3/kmerdb/parse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.3/kmerdb/probability.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5632 2024-04-13 02:29:52.000000 kmerdb-0.8.3/kmerdb/python_distances.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.3/kmerdb/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 20:28:24.182445 kmerdb-0.8.3/kmerdb.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    30696 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.3/kmerdb.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-05-23 20:28:24.000000 kmerdb-0.8.3/kmerdb.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4635 2024-05-23 20:26:57.000000 kmerdb-0.8.3/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-05-23 20:28:24.182445 kmerdb-0.8.3/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-05-23 20:27:11.000000 kmerdb-0.8.3/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-23 20:28:24.182445 kmerdb-0.8.3/test/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.3/test/test_kmer.py
```

### Comparing `kmerdb-0.8.2/LICENSE.txt` & `kmerdb-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/PKG-INFO` & `kmerdb-0.8.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.2
+Version: 0.8.3
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
 Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
@@ -265,17 +265,17 @@
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
 Requires-Dist: sphinx>=4.3.2; extra == "dev"
 Requires-Dist: pytest>=5.3.5; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
-> Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph files
 
-NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count vectors and DeBruijn graph edge-list formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -286,101 +286,180 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
+k-mer counts from .fa(.gz)/.fq(.gz) sequence data can be stored in `.kdb` file format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. This file is compatible with `zlib`.
 
-`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
+Install with `pip install kmerdb`
+
+`kmerdb` is a Python CLI designed for k-mer counting and k-mer graph edge-lists. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of a `bgzf` formatted file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
 
 ## Usage
 
 ```bash
 # Usage    --help option    --debug mode
 kmerdb --help # [+ --debug mode]
-kmerdb usage -m graph
+kmerdb usage graph
 
-# Output:
+**** 
  o-O      |||
 o---O     |||             [|[          kmerdb           ]|]
 O---o     |||
- O-o      |||        version :     v0.8.0
+ O-o      |||        version :     v0.8.2
   O       |||
  o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
 o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
 O---o     |||      Website   : https://matthewralston.github.io/kmerdb
  O-o      |||
                                                                        lang :         python
                                                                           v :      >= v3.7.4
 
                       package manger : pip
                         version      : >= 24.0
-        package root : /path2py/lib/python3.12/site-packages/kmerdb
-        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+        package root : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb
+        exe file     : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb/__init__.py
 
-                      required packages : 8
-                   development packages : 14
+                      required packages : 9
+                   development packages : 9
 
-           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+           ARGV : ['/home/user/.local/share/virtualenvs/kdb-venv/bin/kmerdb', 'usage', 'graph']
         
-...
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+
+
+
 
 Beginning program...
 
-                          name : graph
-                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
-        
 
-* features
 
+
+                          [ name ] :         graph
+
+                   description : create a edge list in (block) .gz format from .fasta|.fa or .fastq format.
+
+
+
+
+   :     4 column output : [ row idx | k-mer id node #1 | k-mer id node #2 | edge weight (adjacency count) ]
+
+   :  make a deBruijn graph, count the number of k-mer adjacencies,  printing the edge list to STDOUT
+
+
+
+
+                  +=============+====================+====================+=================================+
+                  <    row idx  |  k-mer id node #1  |  k-mer id node #2  |  edge weight (adjacency count)  >
+                  |             |                    |                    |                                 |
+                  |             +
+                  |
+                  |
+                  |
+                  |
+                  |
+
+
+
+
+
+--------------------------
+
+
+                    kmerdb graph -k 12 input_1.fa [example_2.fastq] output.12.kdbg
+
+                    [-]    inputs : 
+
+                           Input file can .fastq (or .fa).   - gzip.  Output is a weighted edge list in .kdb format (gzipped .csv with YAML header)
+
+                    [-]    parameters : 
+
+                           uses < -k > for k-mer size, --quiet to reduce runtime, -v, -vv to control logging. --
+
+
+
+                    [-]    [ usage ]  :  kmerdb graph -k $K --quiet <input_1.fa.gz> [input_2.fq.gz] <output_edge_list_file.12.kdbg>
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+name: arguments
+type: array
+items:
+- name: k
+  type: int
+  value: choice of k-mer size
+- name: quiet
+  type: flag
+  value: Write additional debug level information to stderr?
+
+
+
+
+name: inputs
+type: array
+items:
+- name: <.fasta|.fastq>
+  type: array
+  value: gzipped or uncompressed input .fasta or .fastq file(s)
+- name: .kdbg
+  type: file
+  value: Output edge-list filepath.
+
+
+
+
+name: features
+type: array
+items:
 - name: k-mer count arrays, linear, produced as file is read through sliding window.
     (Un)compressed support for .fa/.fq.
   shortname: parallel faux-OP sliding window k-mer shredding
   description: Sequential k-mers from the input .fq|.fa files are added to the De
     Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
     (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
     for the entire file are given for each file read, + a transparent data structure.
-		
 - name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
   shortname: weighted undirected graph
   description: an edge list of a De Bruijn graph is generated from all k-mers in the
     forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
     in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
     graph and the edges provided by the data.
 
-
-
-
-* steps
-
-- name: read input file(s) from filesystem into k-mer arrays
-  shortname: shred inputs into k-mer count arrays
-  description: shred input sequences into k-mer count vector
-  
-- name: merge k-mer arrays and aggregate metadata
-  shortname: merge k-mer count arrays for aggregate metadata (header)
-  description: merge counts of nullomers, unique kmers, and total kmers.
-  
-- name: collate the weighted edge lists after reading multiple files. Output data
-    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
-  shortname: extract undirected weighted graph
-  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
-    edges, and the number of times the pair was observed from forward sequences in
-    the provided dataset
-	
-- name: print 'table' Final stats and close output file
-  shortname: metrics and shutdown
-  description: print final statistics, typically metadata values, and ensure file
-    is closed.
-
+...
 
 
 
 #   +
 
 # [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
@@ -398,15 +477,15 @@
 
 # View header (config.py[kdb_metadata_schema#L84])
 kmerdb header profile_1.8.kdb
 
 ## Optional normalization, dim reduction, and distance matrix features:
 
 # K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
-kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson STDIN
 # 
 # kmerdb matrix DESeq2 *.8.kdb
 # kmerdb matrix PCA *.8.kdb
 # kmerdb matrix tSNE *.8.kdb
 #   # <pass> just makes a k-mer count matrix from k-mer count vectors.
 # 
 
@@ -424,26 +503,38 @@
 #    BioPython Phylip tree + upgma
 kmerdb hierarchical -i dist.tsv
 
 
 ```
 
 
+## Usage example
+
+![kmerdb.gif](kmerdb.gif)
+
+
+
+
 ## Installation
 
 ### OSX and Linux release:
 
 ```sh
-pip install --python-version 3.7.4 --pre kmerdb
+pip install kmerdb
 ```
 
 #### Optional DESeq2 normalization
 
-DESeq2 is an optional R dependency for rpy2-mediated normalization.
+DESeq2 is an optional R dependency for rpy2-mediated normalization. Make sure development libraries are installed from the repository.
+
 
+```
+pip install -r requirements-dev.txt
+```
+Next, install DESeq2 via bioconductor.
 ```r
 if (!requireNamespace("BiocManager", quietly = TRUE))
     install.packages("BiocManager")
 
 BiocManager::install("DESeq2")
 ```
 
@@ -461,15 +552,15 @@
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
 Important features to usage that may be important may not be fully documented as the project is in beta.
 
 For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
-Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
+Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
 
 
 ## Development
```

### Comparing `kmerdb-0.8.2/README.md` & `kmerdb-0.8.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # README - kmerdb
-> Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph files
 
-NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count vectors and DeBruijn graph edge-list formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -16,101 +16,180 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
+k-mer counts from .fa(.gz)/.fq(.gz) sequence data can be stored in `.kdb` file format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. This file is compatible with `zlib`.
 
-`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
+Install with `pip install kmerdb`
+
+`kmerdb` is a Python CLI designed for k-mer counting and k-mer graph edge-lists. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of a `bgzf` formatted file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
 
 ## Usage
 
 ```bash
 # Usage    --help option    --debug mode
 kmerdb --help # [+ --debug mode]
-kmerdb usage -m graph
+kmerdb usage graph
 
-# Output:
+**** 
  o-O      |||
 o---O     |||             [|[          kmerdb           ]|]
 O---o     |||
- O-o      |||        version :     v0.8.0
+ O-o      |||        version :     v0.8.2
   O       |||
  o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
 o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
 O---o     |||      Website   : https://matthewralston.github.io/kmerdb
  O-o      |||
                                                                        lang :         python
                                                                           v :      >= v3.7.4
 
                       package manger : pip
                         version      : >= 24.0
-        package root : /path2py/lib/python3.12/site-packages/kmerdb
-        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+        package root : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb
+        exe file     : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb/__init__.py
 
-                      required packages : 8
-                   development packages : 14
+                      required packages : 9
+                   development packages : 9
 
-           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+           ARGV : ['/home/user/.local/share/virtualenvs/kdb-venv/bin/kmerdb', 'usage', 'graph']
         
-...
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+
+
+
 
 Beginning program...
 
-                          name : graph
-                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
-        
 
-* features
 
+
+                          [ name ] :         graph
+
+                   description : create a edge list in (block) .gz format from .fasta|.fa or .fastq format.
+
+
+
+
+   :     4 column output : [ row idx | k-mer id node #1 | k-mer id node #2 | edge weight (adjacency count) ]
+
+   :  make a deBruijn graph, count the number of k-mer adjacencies,  printing the edge list to STDOUT
+
+
+
+
+                  +=============+====================+====================+=================================+
+                  <    row idx  |  k-mer id node #1  |  k-mer id node #2  |  edge weight (adjacency count)  >
+                  |             |                    |                    |                                 |
+                  |             +
+                  |
+                  |
+                  |
+                  |
+                  |
+
+
+
+
+
+--------------------------
+
+
+                    kmerdb graph -k 12 input_1.fa [example_2.fastq] output.12.kdbg
+
+                    [-]    inputs : 
+
+                           Input file can .fastq (or .fa).   - gzip.  Output is a weighted edge list in .kdb format (gzipped .csv with YAML header)
+
+                    [-]    parameters : 
+
+                           uses < -k > for k-mer size, --quiet to reduce runtime, -v, -vv to control logging. --
+
+
+
+                    [-]    [ usage ]  :  kmerdb graph -k $K --quiet <input_1.fa.gz> [input_2.fq.gz] <output_edge_list_file.12.kdbg>
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+name: arguments
+type: array
+items:
+- name: k
+  type: int
+  value: choice of k-mer size
+- name: quiet
+  type: flag
+  value: Write additional debug level information to stderr?
+
+
+
+
+name: inputs
+type: array
+items:
+- name: <.fasta|.fastq>
+  type: array
+  value: gzipped or uncompressed input .fasta or .fastq file(s)
+- name: .kdbg
+  type: file
+  value: Output edge-list filepath.
+
+
+
+
+name: features
+type: array
+items:
 - name: k-mer count arrays, linear, produced as file is read through sliding window.
     (Un)compressed support for .fa/.fq.
   shortname: parallel faux-OP sliding window k-mer shredding
   description: Sequential k-mers from the input .fq|.fa files are added to the De
     Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
     (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
     for the entire file are given for each file read, + a transparent data structure.
-		
 - name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
   shortname: weighted undirected graph
   description: an edge list of a De Bruijn graph is generated from all k-mers in the
     forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
     in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
     graph and the edges provided by the data.
 
-
-
-
-* steps
-
-- name: read input file(s) from filesystem into k-mer arrays
-  shortname: shred inputs into k-mer count arrays
-  description: shred input sequences into k-mer count vector
-  
-- name: merge k-mer arrays and aggregate metadata
-  shortname: merge k-mer count arrays for aggregate metadata (header)
-  description: merge counts of nullomers, unique kmers, and total kmers.
-  
-- name: collate the weighted edge lists after reading multiple files. Output data
-    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
-  shortname: extract undirected weighted graph
-  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
-    edges, and the number of times the pair was observed from forward sequences in
-    the provided dataset
-	
-- name: print 'table' Final stats and close output file
-  shortname: metrics and shutdown
-  description: print final statistics, typically metadata values, and ensure file
-    is closed.
-
+...
 
 
 
 #   +
 
 # [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
@@ -128,15 +207,15 @@
 
 # View header (config.py[kdb_metadata_schema#L84])
 kmerdb header profile_1.8.kdb
 
 ## Optional normalization, dim reduction, and distance matrix features:
 
 # K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
-kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson STDIN
 # 
 # kmerdb matrix DESeq2 *.8.kdb
 # kmerdb matrix PCA *.8.kdb
 # kmerdb matrix tSNE *.8.kdb
 #   # <pass> just makes a k-mer count matrix from k-mer count vectors.
 # 
 
@@ -154,26 +233,38 @@
 #    BioPython Phylip tree + upgma
 kmerdb hierarchical -i dist.tsv
 
 
 ```
 
 
+## Usage example
+
+![kmerdb.gif](kmerdb.gif)
+
+
+
+
 ## Installation
 
 ### OSX and Linux release:
 
 ```sh
-pip install --python-version 3.7.4 --pre kmerdb
+pip install kmerdb
 ```
 
 #### Optional DESeq2 normalization
 
-DESeq2 is an optional R dependency for rpy2-mediated normalization.
+DESeq2 is an optional R dependency for rpy2-mediated normalization. Make sure development libraries are installed from the repository.
+
 
+```
+pip install -r requirements-dev.txt
+```
+Next, install DESeq2 via bioconductor.
 ```r
 if (!requireNamespace("BiocManager", quietly = TRUE))
     install.packages("BiocManager")
 
 BiocManager::install("DESeq2")
 ```
 
@@ -191,15 +282,15 @@
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
 Important features to usage that may be important may not be fully documented as the project is in beta.
 
 For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
-Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
+Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
 
 
 ## Development
```

### Comparing `kmerdb-0.8.2/kmerdb/__init__.py` & `kmerdb-0.8.3/kmerdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2228,15 +2228,15 @@
 
     #matrix_parser.add_argument("--normalize-with", type=str, choices=["ecopy", "DESeq2"], default="DESeq2", help="Normalize with which method? DEFAULT: DESeq2")
     matrix_parser.add_argument("--no-normalized-ints", action="store_true", default=False, help="Don't round normalized counts to the nearest integer")
     matrix_parser.add_argument("-k", default=None, type=int, help="The k-dimension that the files have in common")
     matrix_parser.add_argument("-n", default=None, type=int, help="The number of dimensions to reduce with PCA or t-SNE. DEFAULT: an elbow graph will be generated if -n is not provided to help the user choose -n")
 
     matrix_parser.add_argument("--perplexity", default=5, type=int, help="The choice of the perplexity for t-SNE based dimensionality reduction")
-    matrix_parser.add_argument("method", choices=["PCA", "tSNE", "DESeq2", "pass", "Frequency"], default=None, help="Choice of distance metric between two profiles")
+    matrix_parser.add_argument("method", choices=["PCA", "tSNE", "DESeq2", "pass", "Frequency"], default=None, help="Choice of dimensionality reduction, normalization method (DESeq2), or pass (no action)")
     matrix_parser.add_argument("input", nargs="*", default=[], metavar="<kdbfile1 kdbfile2 ...|input.tsv|STDIN>", help="Two or more .kdb files, or another count matrix in tsv/csv")
     matrix_parser.set_defaults(func=get_matrix)
     
     # rarefy_parser = subparsers.add_parser("rarefy", help="Generate rarefaction information using ecopy.diversity.rarefy for the supplied .kdb files")
     # rarefy_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     # rarefy_parser.add_argument("-d", "--delimiter", default="\t", type=str, help="The choice of delimiter to parse the DataFrame with")
     # rarefy_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
@@ -2376,15 +2376,26 @@
     """
     Print detailed debugging information prior to program log.
     """
 
 
     #signal.signal(signal.SIGINT, graceful_interrupt)
     #signal.signal(signal.SIGTERM, graceful_termination)
-    subcommand_name = vars(args)['func'].__name__
+
+
+    # Extract the __init__ function invoked from argparsed arguments.
+    function_name = vars(args)['func'].__name__
+
+    # Now, map to the correct subcommand name via config
+
+    if function_name in ["usage", "help", "citation"]:
+        subcommand_name = function_name
+    else:
+        subcommand_name = config.subcommands[config.subcommand_functions.index(function_name)]
+
 
 
     from kmerdb import config
     logger = kdbLogger.Loggah(logfile=args.log_file or None, level=args.verbose)
         
 
     from kmerdb import appmap
@@ -2432,32 +2443,35 @@
             raise e
         except OSError as e:
 
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 5
         
             raise e
+        except IOError as e:
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            exit_code = 6
+            raise e
+        
         except ArgumentError as e:
 
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
-            exit_code = 6
+            exit_code = 7
         
             raise e
         except AssertionError as e:
 
-            print("CAUGHT ASSERTION ERROR")
-            
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
-            exit_code = 7
+            exit_code = 8
         
             raise e
         except FileNotFoundError as e:
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             
-            exit_code = 8
+            exit_code = 9
             raise e
         except Exception as e:
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = -1
         
             raise e
         finally:
```

### Comparing `kmerdb-0.8.2/kmerdb/__main__.py` & `kmerdb-0.8.3/kmerdb/__main__.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/appmap.py` & `kmerdb-0.8.3/kmerdb/appmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,38 +160,34 @@
 ===============================
 """
 
 
 
 
 
-command_1_name = "profile"
-command_2_name = "make_graph"
-command_3_name = "get_matrix"
-command_4_name = "distance"
-command_5_name = "view"
-command_6_name = "header"
-command_7_name = "kmeans"
-command_8_name = "hierarchical"
-command_9_name = "index"
-command_10_name = "shuf"
+command_1_name, command_2_name, command_3_name, command_4_name, command_5_name, command_6_name, command_7_name, command_8_name, command_9_name, command_10_name, command_11_name, command_12_name = config.subcommands
 
 COMMANDS = [
     command_1_name, #"profile",
     command_2_name, #"make_graph",
     command_3_name, #"get_matrix",
     command_4_name, #"distance",
     command_5_name, #"view",
     command_6_name, #"header",
     command_7_name, #"kmeans",
     command_8_name, #"hierarchical",
     command_9_name, #"index",
     command_10_name, #"shuf",
+    command_11_name, #"usage",
+    command_12_name #"help"
 ]
 
+
+
+
         
 command_1_description = "create a k-mer count vector from fasta input. g-zipped/.bgzf   -  4 column table with YAML header."
 command_1_description_long = """
 
       :           4 columns output table       :    [   row idx   |   k-mer id  |    count   |  frequency  ]
 
       :    print a k-mer count vector to STDOUT
@@ -1868,65 +1864,64 @@
 
     ]
 
 })
 
 ALL_PARAMS = {
     "profile": COMMAND_1_PARAMS["items"],
-    "make_graph": COMMAND_2_PARAMS["items"],
-    "get_matrix": COMMAND_3_PARAMS["items"],
+    "graph": COMMAND_2_PARAMS["items"],
+    "matrix": COMMAND_3_PARAMS["items"],
     "distance": COMMAND_4_PARAMS["items"],
+    "kmeans": COMMAND_7_PARAMS["items"],
+    "hierarchical": COMMAND_8_PARAMS["items"],    
     "view": COMMAND_5_PARAMS["items"],
     "header": COMMAND_6_PARAMS["items"],
-    "kmeans": COMMAND_7_PARAMS["items"],
-    "hierarchical": COMMAND_8_PARAMS["items"],
     "index": COMMAND_9_PARAMS["items"],
     "shuf": COMMAND_10_PARAMS["items"]
-
 }
 
 ALL_INPUTS = {
     "profile": COMMAND_1_INPUTS["items"],
-    "make_graph": COMMAND_2_INPUTS["items"],
-    "get_matrix": COMMAND_3_INPUTS["items"],
+    "graph": COMMAND_2_INPUTS["items"],
+    "matrix": COMMAND_3_INPUTS["items"],
     "distance": COMMAND_4_INPUTS["items"],
-    "view": COMMAND_5_INPUTS["items"],
-    "header": COMMAND_6_INPUTS["items"],
     "kmeans": COMMAND_7_INPUTS["items"],
     "hierarchical": COMMAND_8_INPUTS["items"],
+    "view": COMMAND_5_INPUTS["items"],
+    "header": COMMAND_6_INPUTS["items"],
     "index": COMMAND_9_INPUTS["items"],
     "shuf": COMMAND_10_INPUTS["items"]
 }
 
 ALL_FEATURES = {
     "profile": COMMAND_1_FEATURES["items"],
-    "make_graph": COMMAND_2_FEATURES["items"],
-    "get_matrix": COMMAND_3_FEATURES["items"],
-    "distances": COMMAND_4_FEATURES["items"],
-    "view": COMMAND_5_FEATURES["items"],
-    "header": COMMAND_6_FEATURES["items"],
+    "graph": COMMAND_2_FEATURES["items"],
+    "matrix": COMMAND_3_FEATURES["items"],
+    "distance": COMMAND_4_FEATURES["items"],
     "kmeans": COMMAND_7_FEATURES["items"],
     "hierarchical": COMMAND_8_FEATURES["items"],
+    "view": COMMAND_5_FEATURES["items"],
+    "header": COMMAND_6_FEATURES["items"],
     "index": COMMAND_9_FEATURES["items"],
     "shuf": COMMAND_10_FEATURES["items"]
 
 
 }
 
 
 ALL_STEPS = {
 
     "profile": COMMAND_1_STEPS["items"],
-    "make_graph": COMMAND_2_STEPS["items"],
-    "get_matrix": COMMAND_3_STEPS["items"],
-    "distances": COMMAND_4_STEPS["items"],
-    "view": COMMAND_5_STEPS["items"],
-    "header": COMMAND_6_STEPS["items"],
+    "graph": COMMAND_2_STEPS["items"],
+    "matrix": COMMAND_3_STEPS["items"],
+    "distance": COMMAND_4_STEPS["items"],
     "kmeans": COMMAND_7_STEPS["items"],
     "hierarchical": COMMAND_8_STEPS["items"],
+    "view": COMMAND_5_STEPS["items"],
+    "header": COMMAND_6_STEPS["items"],
     "index": COMMAND_9_STEPS["items"],
     "shuf": COMMAND_10_STEPS["items"]
 }
 
 
 
 
@@ -2390,31 +2385,33 @@
         
         #assert subcommand in config.subcommand_functions, "Unknown subcommand"
 
         if self._loggable:
             self.logger.log_it("Program error! Collecting error metadata and formatting...", "ERROR")
         # This is the "Error blocks" metadata
 
-        # print(subcommand)
-        # print(config.VERSION)
-        # print(config.REQUIRES_PYTHON)
-        # print(feature)
-        # print(ALL_FEATURES[subcommand][feature]["name"])
-        # print(ALL_FEATURES[subcommand][feature]["shortname"])
-        # print(ALL_FEATURES[subcommand][feature]["description"])
-        # print(step)
-        # print(ALL_STEPS[subcommand][step]["name"])
-        # print(ALL_STEPS[subcommand][step]["shortname"])
-        # print(ALL_STEPS[subcommand][step]["description"])
-        #     # The *total* number of logged lines produced by the program and returned to the global 'logs' var in __init__.py
-        # print(self.logfile)
-        # print(str(tb))
-        # print(error_file_name)
-        # print(error_line_number)
-        # print(e.__str__())
+
+        sys.stderr.write("Aggregating program metadata, if this fails without error without the --debug flag, please report to the GitHub issue tracker with the title 'Error summary convenience function'.")
+        sys.stderr(subcommand)
+        sys.stderr(config.VERSION)
+        sys.stderr(config.REQUIRES_PYTHON)
+        sys.stderr(feature)
+        sys.stderr(ALL_FEATURES[subcommand][feature]["name"])
+        sys.stderr(ALL_FEATURES[subcommand][feature]["shortname"])
+        sys.stderr(ALL_FEATURES[subcommand][feature]["description"])
+        sys.stderr(step)
+        sys.stderr(ALL_STEPS[subcommand][step]["name"])
+        sys.stderr(ALL_STEPS[subcommand][step]["shortname"])
+        sys.stderr(ALL_STEPS[subcommand][step]["description"])
+            # The *total* number of logged lines produced by the program and returned to the global 'logs' var in __init__.py
+        sys.stderr(self.logfile)
+        sys.stderr(str(tb))
+        sys.stderr(error_file_name)
+        sys.stderr(error_line_number)
+        sys.stderr(e.__str__())
 
         
         e_sum = {
             "subcommand": subcommand,
             "kmerdb-version": config.VERSION,
             "python-version": config.REQUIRES_PYTHON,
             "feature": feature,
```

### Comparing `kmerdb-0.8.2/kmerdb/banners.py` & `kmerdb-0.8.3/kmerdb/banners.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/config.py` & `kmerdb-0.8.3/kmerdb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,26 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 '''
 
 
 
-VERSION="0.8.2"
+VERSION="0.8.3"
 REQUIRES_PYTHON="3.7.4"
 header_delimiter = "\n" + ("="*24) + "\n"
 
 
 requirements_count = 9
 requirements_dev_count = 9 # 4/9/24 there are some duplicates sure, but the requirements evolve faster than the dev do, are more essential for function, and I dont change the -dev file much. 
 
-subcommands = ["usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"] # kmeans and hierarchical and probability commands deprecated
-subcommand_functions = ["expanded_help", "profile", "make_graph", "get_matrix", "index_file", "shuf", "get_matrix", "distances"]
+# 12 subcommands, and associated function names in __init__.py
+subcommands = ["profile", "graph", "matrix", "distance", "kmeans", "hierarchical", "view", "header", "index", "shuf", "usage", "help"]
+subcommand_functions = ["profile", "make_graph", "get_matrix", "distances", "kmeans", "hierarchical", "view", "header", "index_file", "shuf", "expanded_help", "expanded_help"]
 
-#subcommand_functions = ("profile", "make_graph", "get_matrix", "index_file", "distances", "kmeans", "hierarchical",)
 default_logline_choices = (20, 50, 100, 200)
 KDB_COLUMN_NUMBER = 4
 
 
 
 graph_schema = {
     "type": "object",
```

### Comparing `kmerdb-0.8.2/kmerdb/distance.c` & `kmerdb-0.8.3/kmerdb/distance.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "kmerdb.distance",
         "sources": [
             "kmerdb/distance.pyx"
         ]
     },
     "module_name": "kmerdb.distance"
@@ -1674,177 +1674,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1877,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18030,261 +18030,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18293,29 +18293,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18326,15 +18326,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18343,29 +18343,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18376,15 +18376,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18393,29 +18393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18426,15 +18426,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18443,29 +18443,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18476,15 +18476,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18493,29 +18493,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18526,217 +18526,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18752,15 +18752,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18768,68 +18768,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18837,15 +18837,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18860,15 +18860,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18884,15 +18884,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18900,68 +18900,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18969,15 +18969,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18992,15 +18992,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19016,15 +19016,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19032,68 +19032,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19101,15 +19101,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19124,170 +19124,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22077,26 +22077,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-78ou8665/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `kmerdb-0.8.2/kmerdb/distance.pyx` & `kmerdb-0.8.3/kmerdb/distance.pyx`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/fileutil.py` & `kmerdb-0.8.3/kmerdb/fileutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,16 @@
                         #logger.debug("Reading {0}th line...".format(j))
                         try:
                             line = next(self)
                         except StopIteration as e:
                             if self._loggable:
                                 self.logger.log_it("Finished loading initial profile through slurp-on-init", "ERROR")
                                 self.logger.log_it("Read profile from: {0}".format(self._filepath), "ERROR")
-                            raise e
+                            #raise e
+                            continue
                         if line is None:
                             if self._loggable:
                                 self.logger.log_it("'next' was None... Internal Error", "ERROR")
                             raise RuntimeError("Could not complete parsing of file. Internal Error")
                         # Don't forget to not parse the metadata column [:-1]
 
                         l = line.rstrip().split("\t")
```

### Comparing `kmerdb-0.8.2/kmerdb/graph.py` & `kmerdb-0.8.3/kmerdb/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,16 +590,19 @@
 
             current_kmer_id = kmer_ids[i]
             current_kmer = kmer.id_to_kmer(current_kmer_id, k)
             pair = (current_kmer, kmer.id_to_kmer(kmer_ids[i+1], k)) 
             pair_ids = tuple(map(kmer.kmer_to_id, pair))
             
             common_seq = current_kmer[1:]
-            sys.stderr.write("Kmer_id: = kmer_ids[i]     =        {0}\n".format(current_kmer_id))
-            sys.stderr.write(" -----pair: = '{0}'  <-> '{1}'\n".format(pair[0], pair[1]))
+
+
+            if quiet is False:
+                sys.stderr.write("Kmer_id: = kmer_ids[i]     =        {0}\n".format(current_kmer_id))
+                sys.stderr.write(" -----pair: = '{0}'  <-> '{1}'\n".format(pair[0], pair[1]))
             all_edges_in_kspace[pair_ids] = 0
             # Create the neighbor lists from the list of chars, prepended or appended to the k-mer suffix/prefix
             """
             BOGUS ASSERTIONS AND NONGUARANTEES...
             """
             assert len(current_kmer) == k
             assert len(common_seq) == k-1
@@ -725,17 +728,18 @@
 
 
             maxlen = 15 # Placeholder
             p1str = str(pair_ids[0])
             p2str = str(pair_ids[1])
             p1str = p1str + (maxlen - len(p1str))*" "
             p2str = p2str + (maxlen - len(p2str))*" "
-            
-            sys.stderr.write("k-mer 'pair' ({0}, {1}) adjacency from input file(s) verified".format(p1str, p2str))
-            sys.stderr.write("\r")
+
+            if quiet is False:
+                sys.stderr.write("k-mer 'pair' ({0}, {1}) adjacency from input file(s) verified".format(p1str, p2str))
+                sys.stderr.write("\r")
             continue
 
 
     if error_count > 0:
         sys.stderr.write("\n\n\nNOTE: ADJACENCY ERRORS DETECTED: Found {0} 'improper' k-mer pairs/adjacencies from the input file(s),\n where subsequent k-mers in the k-mer id array (produced from the sliding window method over input seqs/reads) did not share k-1 residues in common.\n These *may* be introduced in the array from the last k-mer of one seq/read (in the .fa/.fq) and the first k-mer of the next seq/read.\n".format(error_count))
     sys.stderr.write("\n\n\n")
     sys.stderr.write("All edges populated *and* accumulated across k-mer id arrays from inputs.\n")
@@ -1199,15 +1203,16 @@
 
             try:
                 line = next(self)
 
             except StopIteration as e:
                 if self._loggable:
                     self.logger.log_it("Finished loading .kdbg through slurp (on init)", "ERROR")
-                raise e
+                #raise e
+                pass
             if line is None:
                 if self._loggable:
                     self.logger.log_it("'next' returned None. Panic", "WARNING")
 
                 raise RuntimeError("kmerdb.graph.KDBGReader.slurp Panicked on new line")
```

### Comparing `kmerdb-0.8.2/kmerdb/index.py` & `kmerdb-0.8.3/kmerdb/index.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/kmer.py` & `kmerdb-0.8.3/kmerdb/kmer.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,21 +475,22 @@
 # jgs \\|//   \\|///  \\\|//\\\|/// \|///  \\\|//  \\|//  \\\|// 
 # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 # """,
 #               "",
 
 #         )
 
-        sys.stderr.write("kmerdb.kmer.neighbors creating neighbors for k-mer {0} : '{1}'...".format(kmer_id, kmer) + "\n")
-        sys.stderr.write(" ========================\n\n")
-        sys.stderr.write(", ".join(list(map(str, new_type1_ids))) + "\n")
-        sys.stderr.write(", ".join(list(map(str, new_type2_ids))) + "\n\n")
-        sys.stderr.write(" ------------------------\n\n")
         
         if quiet is not True:
+            sys.stderr.write("kmerdb.kmer.neighbors creating neighbors for k-mer {0} : '{1}'...".format(kmer_id, kmer) + "\n")
+            sys.stderr.write(" ========================\n\n")
+            sys.stderr.write(", ".join(list(map(str, new_type1_ids))) + "\n")
+            sys.stderr.write(", ".join(list(map(str, new_type2_ids))) + "\n\n")
+            sys.stderr.write(" ------------------------\n\n")
+
             sys.stderr.write("""
         k-id : {0}
         kmer : \"    {1}        \"
 
         'neighbors'
 
         {2}
```

### Comparing `kmerdb-0.8.2/kmerdb/legacy.py` & `kmerdb-0.8.3/kmerdb/legacy.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/logger.py` & `kmerdb-0.8.3/kmerdb/logger.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/parse.py` & `kmerdb-0.8.3/kmerdb/parse.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/probability.py` & `kmerdb-0.8.3/kmerdb/probability.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/python_distances.py` & `kmerdb-0.8.3/kmerdb/python_distances.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb/util.py` & `kmerdb-0.8.3/kmerdb/util.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/kmerdb.egg-info/PKG-INFO` & `kmerdb-0.8.3/kmerdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.2
+Version: 0.8.3
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
 Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
@@ -265,17 +265,17 @@
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
 Requires-Dist: sphinx>=4.3.2; extra == "dev"
 Requires-Dist: pytest>=5.3.5; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
-> Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph files
 
-NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count vectors and DeBruijn graph edge-list formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -286,101 +286,180 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
+k-mer counts from .fa(.gz)/.fq(.gz) sequence data can be stored in `.kdb` file format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. This file is compatible with `zlib`.
 
-`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
+Install with `pip install kmerdb`
+
+`kmerdb` is a Python CLI designed for k-mer counting and k-mer graph edge-lists. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of a `bgzf` formatted file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
 
 ## Usage
 
 ```bash
 # Usage    --help option    --debug mode
 kmerdb --help # [+ --debug mode]
-kmerdb usage -m graph
+kmerdb usage graph
 
-# Output:
+**** 
  o-O      |||
 o---O     |||             [|[          kmerdb           ]|]
 O---o     |||
- O-o      |||        version :     v0.8.0
+ O-o      |||        version :     v0.8.2
   O       |||
  o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
 o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
 O---o     |||      Website   : https://matthewralston.github.io/kmerdb
  O-o      |||
                                                                        lang :         python
                                                                           v :      >= v3.7.4
 
                       package manger : pip
                         version      : >= 24.0
-        package root : /path2py/lib/python3.12/site-packages/kmerdb
-        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+        package root : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb
+        exe file     : /home/user/.local/share/virtualenvs/kdb-venv/lib/python3.12/site-packages/kmerdb/__init__.py
 
-                      required packages : 8
-                   development packages : 14
+                      required packages : 9
+                   development packages : 9
 
-           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+           ARGV : ['/home/user/.local/share/virtualenvs/kdb-venv/bin/kmerdb', 'usage', 'graph']
         
-...
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+O---o
+ O-o
+  O
+ o-O
+o---O
+
+
+
 
 Beginning program...
 
-                          name : graph
-                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
-        
 
-* features
 
+
+                          [ name ] :         graph
+
+                   description : create a edge list in (block) .gz format from .fasta|.fa or .fastq format.
+
+
+
+
+   :     4 column output : [ row idx | k-mer id node #1 | k-mer id node #2 | edge weight (adjacency count) ]
+
+   :  make a deBruijn graph, count the number of k-mer adjacencies,  printing the edge list to STDOUT
+
+
+
+
+                  +=============+====================+====================+=================================+
+                  <    row idx  |  k-mer id node #1  |  k-mer id node #2  |  edge weight (adjacency count)  >
+                  |             |                    |                    |                                 |
+                  |             +
+                  |
+                  |
+                  |
+                  |
+                  |
+
+
+
+
+
+--------------------------
+
+
+                    kmerdb graph -k 12 input_1.fa [example_2.fastq] output.12.kdbg
+
+                    [-]    inputs : 
+
+                           Input file can .fastq (or .fa).   - gzip.  Output is a weighted edge list in .kdb format (gzipped .csv with YAML header)
+
+                    [-]    parameters : 
+
+                           uses < -k > for k-mer size, --quiet to reduce runtime, -v, -vv to control logging. --
+
+
+
+                    [-]    [ usage ]  :  kmerdb graph -k $K --quiet <input_1.fa.gz> [input_2.fq.gz] <output_edge_list_file.12.kdbg>
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+name: arguments
+type: array
+items:
+- name: k
+  type: int
+  value: choice of k-mer size
+- name: quiet
+  type: flag
+  value: Write additional debug level information to stderr?
+
+
+
+
+name: inputs
+type: array
+items:
+- name: <.fasta|.fastq>
+  type: array
+  value: gzipped or uncompressed input .fasta or .fastq file(s)
+- name: .kdbg
+  type: file
+  value: Output edge-list filepath.
+
+
+
+
+name: features
+type: array
+items:
 - name: k-mer count arrays, linear, produced as file is read through sliding window.
     (Un)compressed support for .fa/.fq.
   shortname: parallel faux-OP sliding window k-mer shredding
   description: Sequential k-mers from the input .fq|.fa files are added to the De
     Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
     (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
     for the entire file are given for each file read, + a transparent data structure.
-		
 - name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
   shortname: weighted undirected graph
   description: an edge list of a De Bruijn graph is generated from all k-mers in the
     forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
     in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
     graph and the edges provided by the data.
 
-
-
-
-* steps
-
-- name: read input file(s) from filesystem into k-mer arrays
-  shortname: shred inputs into k-mer count arrays
-  description: shred input sequences into k-mer count vector
-  
-- name: merge k-mer arrays and aggregate metadata
-  shortname: merge k-mer count arrays for aggregate metadata (header)
-  description: merge counts of nullomers, unique kmers, and total kmers.
-  
-- name: collate the weighted edge lists after reading multiple files. Output data
-    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
-  shortname: extract undirected weighted graph
-  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
-    edges, and the number of times the pair was observed from forward sequences in
-    the provided dataset
-	
-- name: print 'table' Final stats and close output file
-  shortname: metrics and shutdown
-  description: print final statistics, typically metadata values, and ensure file
-    is closed.
-
+...
 
 
 
 #   +
 
 # [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
@@ -398,15 +477,15 @@
 
 # View header (config.py[kdb_metadata_schema#L84])
 kmerdb header profile_1.8.kdb
 
 ## Optional normalization, dim reduction, and distance matrix features:
 
 # K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
-kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson STDIN
 # 
 # kmerdb matrix DESeq2 *.8.kdb
 # kmerdb matrix PCA *.8.kdb
 # kmerdb matrix tSNE *.8.kdb
 #   # <pass> just makes a k-mer count matrix from k-mer count vectors.
 # 
 
@@ -424,26 +503,38 @@
 #    BioPython Phylip tree + upgma
 kmerdb hierarchical -i dist.tsv
 
 
 ```
 
 
+## Usage example
+
+![kmerdb.gif](kmerdb.gif)
+
+
+
+
 ## Installation
 
 ### OSX and Linux release:
 
 ```sh
-pip install --python-version 3.7.4 --pre kmerdb
+pip install kmerdb
 ```
 
 #### Optional DESeq2 normalization
 
-DESeq2 is an optional R dependency for rpy2-mediated normalization.
+DESeq2 is an optional R dependency for rpy2-mediated normalization. Make sure development libraries are installed from the repository.
+
 
+```
+pip install -r requirements-dev.txt
+```
+Next, install DESeq2 via bioconductor.
 ```r
 if (!requireNamespace("BiocManager", quietly = TRUE))
     install.packages("BiocManager")
 
 BiocManager::install("DESeq2")
 ```
 
@@ -461,15 +552,15 @@
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
 Important features to usage that may be important may not be fully documented as the project is in beta.
 
 For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
-Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
+Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
 
 
 ## Development
```

### Comparing `kmerdb-0.8.2/kmerdb.egg-info/SOURCES.txt` & `kmerdb-0.8.3/kmerdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.2/pyproject.toml` & `kmerdb-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # requires numpy and cython for custom cython correlation function
 
 requires = ["setuptools>=69.2.0", "numpy>=1.21.2", "Cython>=3.0.8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kmerdb"
-version = "0.8.2"
+version = "0.8.3"
 description = "Yet another corretion to the 'yet another correction to just a k-mer counter...'"
 readme = "README.md"
 authors = [{name="Matt Ralston <mralston.development@gmail.com>", email="mralston.development@gmail.com"}]
 license = { file = "LICENSE.txt" }
 classifiers = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
```

### Comparing `kmerdb-0.8.2/setup.py` & `kmerdb-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 long_description = 'See README.md for details'
 URL = 'https://github.com/MatthewRalston/kmerdb'
 CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz"
 EMAIL = 'mralston.development@gmail.com'
 AUTHOR = 'fross'
 REQUIRES_PYTHON = ">=3.7.4"
 #REQUIRES_PYTHON = '>=3.12.2'
-VERSION = "0.8.2"
+VERSION = "0.8.3"
 KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer"]
 CLASSIFIERS = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
 	    "Development Status :: 7 - Inactive",
 	    "Environment :: Console",
 	    "Intended Audience :: Developers",
```

### Comparing `kmerdb-0.8.2/test/test_kmer.py` & `kmerdb-0.8.3/test/test_kmer.py`

 * *Files identical despite different names*

