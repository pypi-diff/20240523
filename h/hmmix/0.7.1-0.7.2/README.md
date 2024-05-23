# Comparing `tmp/hmmix-0.7.1.tar.gz` & `tmp/hmmix-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hmmix-0.7.1.tar", last modified: Fri May 17 22:36:02 2024, max compression
+gzip compressed data, was "hmmix-0.7.2.tar", last modified: Thu May 23 21:37:29 2024, max compression
```

## Comparing `hmmix-0.7.1.tar` & `hmmix-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.7.1/LICENSE.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41064 2024-05-17 22:36:02.000000 hmmix-0.7.1/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    40530 2024-05-17 22:33:23.000000 hmmix-0.7.1/README.md
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2024-05-17 22:36:02.000000 hmmix-0.7.1/setup.cfg
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2024-05-17 22:35:48.000000 hmmix-0.7.1/setup.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2024-05-17 18:48:53.000000 hmmix-0.7.1/src/bcf_vcf.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    17258 2024-05-17 22:29:01.000000 hmmix-0.7.1/src/helper_functions.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    18509 2024-05-15 21:18:28.000000 hmmix-0.7.1/src/hmm_functions.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/hmmix.egg-info/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41064 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/PKG-INFO
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      380 2024-05-17 22:36:02.000000 hmmix-0.7.1/src/hmmix.egg-info/SOURCES.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/dependency_links.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       36 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/entry_points.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/requires.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2024-05-17 22:36:01.000000 hmmix-0.7.1/src/hmmix.egg-info/top_level.txt
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21120 2024-05-17 22:35:42.000000 hmmix-0.7.1/src/main.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2024-05-15 21:18:33.000000 hmmix-0.7.1/src/make_mutationrate.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4431 2024-05-15 22:49:25.000000 hmmix-0.7.1/src/make_test_data.py
-drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-17 22:36:02.000000 hmmix-0.7.1/test/
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     1280 2024-05-13 00:59:38.000000 hmmix-0.7.1/test/test.py
--rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.7.1/test/test_main.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-23 21:37:29.575491 hmmix-0.7.2/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    35149 2022-05-11 17:42:22.000000 hmmix-0.7.2/LICENSE.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41621 2024-05-23 21:37:29.575491 hmmix-0.7.2/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41087 2024-05-23 18:34:58.000000 hmmix-0.7.2/README.md
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       38 2024-05-23 21:37:29.575491 hmmix-0.7.2/setup.cfg
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      994 2024-05-23 21:36:40.000000 hmmix-0.7.2/setup.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-23 21:37:29.575491 hmmix-0.7.2/src/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     8599 2024-05-17 18:48:53.000000 hmmix-0.7.2/src/bcf_vcf.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    17394 2024-05-23 17:23:23.000000 hmmix-0.7.2/src/helper_functions.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21971 2024-05-23 21:27:08.000000 hmmix-0.7.2/src/hmm_functions.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-23 21:37:29.575491 hmmix-0.7.2/src/hmmix.egg-info/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    41621 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/PKG-INFO
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      380 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/SOURCES.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)        1 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/dependency_links.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       37 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/entry_points.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       29 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/requires.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)       77 2024-05-23 21:37:29.000000 hmmix-0.7.2/src/hmmix.egg-info/top_level.txt
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)    21657 2024-05-23 21:37:17.000000 hmmix-0.7.2/src/main.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     2007 2024-05-15 21:18:33.000000 hmmix-0.7.2/src/make_mutationrate.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     4431 2024-05-23 21:33:10.000000 hmmix-0.7.2/src/make_test_data.py
+drwxrwxr-x   0 laurits_skov  (1000) laurits_skov  (1000)        0 2024-05-23 21:37:29.575491 hmmix-0.7.2/test/
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)     1280 2024-05-13 00:59:38.000000 hmmix-0.7.2/test/test.py
+-rw-rw-r--   0 laurits_skov  (1000) laurits_skov  (1000)      541 2022-06-08 21:55:04.000000 hmmix-0.7.2/test/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hmmix-0.7.1/LICENSE.txt` & `hmmix-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.1/PKG-INFO` & `hmmix-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.7.1
+Version: 0.7.2
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -244,15 +244,15 @@
 18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
-We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
+We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments. Please note that even thought we simulated 50 Mb of sequence the last window in the decoded output is at window 49991000 for chromosome 1 and 49979000 for chromosome 2. This is because hmmix uses the position of the last SNP to determine the length of the chromosome. The last SNP on chromosome 1 is 49990559 and the last SNP on chromosome 2 is 49978752.
 
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
@@ -297,15 +297,15 @@
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
 
 NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
 
-But keep reading along if you want to know HOW the files were generated!
+But keep reading along if you want to know HOW the files were generated! Another important thing to note is that hmmix is relying on VCFtools which only support VCF files up to format V4.2 - so if you have VCFfiles in version 4.3 you will need to change this in your header!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json
```

### Comparing `hmmix-0.7.1/README.md` & `hmmix-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
-We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
+We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments. Please note that even thought we simulated 50 Mb of sequence the last window in the decoded output is at window 49991000 for chromosome 1 and 49979000 for chromosome 2. This is because hmmix uses the position of the last SNP to determine the length of the chromosome. The last SNP on chromosome 1 is 49990559 and the last SNP on chromosome 2 is 49978752.
 
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
@@ -281,15 +281,15 @@
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
 
 NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
 
-But keep reading along if you want to know HOW the files were generated!
+But keep reading along if you want to know HOW the files were generated! Another important thing to note is that hmmix is relying on VCFtools which only support VCF files up to format V4.2 - so if you have VCFfiles in version 4.3 you will need to change this in your header!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json
```

### Comparing `hmmix-0.7.1/setup.py` & `hmmix-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='hmmix', 
-    version = '0.7.1',
+    version = '0.7.2',
     description='Find introgressed segments',
     py_modules=['bcf_vcf', 'helper_functions', 'hmm_functions', 'main', 'make_mutationrate', 'make_test_data'],
     package_dir={'': 'src'},
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `hmmix-0.7.1/src/bcf_vcf.py` & `hmmix-0.7.2/src/bcf_vcf.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.1/src/helper_functions.py` & `hmmix-0.7.2/src/helper_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,14 +423,17 @@
 
 
 
 
 # Check which type of input we are dealing with
 def combined_files(ancestralfiles, vcffiles):
 
+    if len(ancestralfiles) == len(vcffiles) and len(vcffiles) == 1 and ancestralfiles != ['']:
+        return ancestralfiles, vcffiles
+
     # Get ancestral and vcf consensus
     prefix1, postfix1, values1 = get_consensus(vcffiles)
     prefix2, postfix2, values2 = get_consensus(ancestralfiles)
 
     # No ancestral files
     if ancestralfiles == ['']:
         ancestralfiles = [None for _ in vcffiles]
```

### Comparing `hmmix-0.7.1/src/hmm_functions.py` & `hmmix-0.7.2/src/hmm_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -123,14 +123,17 @@
             forwards_in[t,:] = init_start  * probabilities[t,:]
             scale_param[t] = np.sum( forwards_in[t,:])
             forwards_in[t,:] = forwards_in[t,:] / scale_param[t]  
         else:
             forwards_in[t,:], scale_param[t] =  fwd_step(forwards_in[t-1,:], probabilities[t,:], transitions) 
 
     return forwards_in, scale_param
+
+
+
     
 
 @njit
 def bwd_step(beta_next, E, trans_mat, n):
     beta = (trans_mat * E) @ beta_next
     return beta / n
 
@@ -317,15 +320,15 @@
         previous_loglikelihood = new_loglikelihood
 
     # Write the optimal parametersf
     return hmm_parameters
     
 
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
-# Decode
+# Decode (posterior decoding)
 # ----------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters):
 
     
     # Posterior decode the file
     emissions = Emission_probs_poisson(hmm_parameters.emissions, obs, weights, mutrates)
@@ -364,14 +367,106 @@
             variants_segment = flatten_list(variants[start_index:end_index])
 
             segments.append([newchrom, genome_start,  genome_end, genome_length, hmm_parameters.state_names[state], mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants_segment]) 
     
     return segments
 
 
+# ----------------------------------------------------------------------------------------------------------------------------------------------------------------
+# Decode (Viterbi)
+# ----------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+@njit
+def fwd_step_keep_track(alpha_prev, E, trans_mat):
+    
+    # scaling factor
+    n = np.sum((alpha_prev @ trans_mat) * E)
+    
+    results = np.zeros(len(E))
+    back_track_states = np.zeros(len(E))
+
+    for current_s in range(len(E)):
+        for prev_s in range(len(E)):
+            new_prob = alpha_prev[prev_s] * trans_mat[prev_s, current_s] * E[current_s] / n
+
+            if new_prob > results[current_s]:
+                results[current_s] = new_prob
+                back_track_states[current_s] = prev_s
+
+    return results, back_track_states
+
+
+@njit
+def viterbi(probabilities, transitions, init_start):
+    n = len(probabilities)
+    forwards_in = np.zeros( (n, len(init_start)) ) 
+    backtracks = np.zeros( (n, len(init_start)), dtype=np.int32) 
+
+    for t in range(n):
+        if t == 0:
+            forwards_in[t,:] = init_start  * probabilities[t,:]
+            scale_param = np.sum( forwards_in[t,:])
+            forwards_in[t,:] = forwards_in[t,:] / scale_param
+        else:
+            forwards_in[t,:], backtracks[t,:] =  fwd_step_keep_track(forwards_in[t-1,:], probabilities[t,:], transitions) 
+
+    return forwards_in, backtracks
+
+def DecodeModel_viterbi(obs, chroms, starts, variants, mutrates, weights, hmm_parameters):
+
+    # Posterior decode the file
+    emissions = Emission_probs_poisson(hmm_parameters.emissions, obs, weights, mutrates)
+    viterbi_probs, backtracks = viterbi(emissions, hmm_parameters.transitions, hmm_parameters.starting_probabilities)
+    window_size = starts[2] - starts[1]
+    
+    viterbi_path = np.zeros(len(obs), dtype = int)
+    viterbi_path[-1] = np.argmax(viterbi_probs[-1,:])
+    
+    for t in range(len(obs) - 2, 0, -1):
+        viterbi_path[t] = backtracks[t + 1, viterbi_path[t + 1]]
+
+    
+
+    segments = []
+    for (chrom, chrom_start_index, chrom_length_index) in find_runs(chroms):
+
+        # Diploid or haploid
+        if '_hap' in chrom:
+            newchrom, ploidity = chrom.split('_')
+        else:
+            ploidity = 'diploid'
+            newchrom = chrom
+
+        state_with_highest_prob = viterbi_path[chrom_start_index:chrom_start_index + chrom_length_index]
+
+        for (state, start_index, length_index) in find_runs(state_with_highest_prob):
+            
+            start_index = start_index + chrom_start_index
+            end_index = start_index + length_index
+
+            genome_start = starts[start_index]
+            genome_length =  length_index * window_size
+            genome_end = genome_start + genome_length
+
+            called_sequence = int(np.sum(weights[start_index:end_index]) * window_size)
+            average_mutation_rate = round(np.mean(mutrates[start_index:end_index]), 3)
+
+            snp_counter = np.sum(obs[start_index:end_index])
+            mean_prob = 1
+            variants_segment = flatten_list(variants[start_index:end_index])
+
+            segments.append([newchrom, genome_start,  genome_end, genome_length, hmm_parameters.state_names[state], mean_prob, snp_counter, ploidity, called_sequence, average_mutation_rate, variants_segment]) 
+    
+    return segments
+
+
+
+
+
+
 
 
 
 def Write_Decoded_output(outputprefix, segments, obs_file = None, admixpop_file = None, extrainfo = False):
 
     # Load archaic data
     if admixpop_file is not None:
```

### Comparing `hmmix-0.7.1/src/hmmix.egg-info/PKG-INFO` & `hmmix-0.7.2/src/hmmix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmix
-Version: 0.7.1
+Version: 0.7.2
 Summary: Find introgressed segments
 Home-page: https://github.com/LauritsSkov/Introgression-detection
 Author: Laurits Skov and Moises Coll Macia
 Author-email: lauritsskov2@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -244,15 +244,15 @@
 18         -17401.3835    0.994   0.006   0.0398  0.4587  0.9999    0.9808
 
 
 # run without mutrate and weights (only do this for simulated data)
 > hmmix train  -obs=obs.txt -param=Initialguesses.json -out=trained.json
 ```
 
-We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments:
+We can now decode the data with the best parameters that maximize the likelihood and find the archaic segments. Please note that even thought we simulated 50 Mb of sequence the last window in the decoded output is at window 49991000 for chromosome 1 and 49979000 for chromosome 2. This is because hmmix uses the position of the last SNP to determine the length of the chromosome. The last SNP on chromosome 1 is 49990559 and the last SNP on chromosome 2 is 49978752.
 
 ```note
 > hmmix decode -obs=obs.txt -weights=weights.bed -mutrates=mutrates.bed -param=trained.json
 ----------------------------------------
 > state_names = ['Human', 'Archaic']
 > starting_probabilities = [0.994, 0.006]
 > transitions = [[1.0, 0.0], [0.019, 0.981]]
@@ -297,15 +297,15 @@
 ---
 
 The whole pipeline we will run looks like this. In the following section we will go through all the steps on the way
 
 NOTE: The outgroup files, mutation rate files, reference genomes, ancestral alleles and callability files and ancestral allele files are now premade!
 They can be downloaded in hg38 and hg19 here: <https://doi.org/10.5281/zenodo.11212339>
 
-But keep reading along if you want to know HOW the files were generated!
+But keep reading along if you want to know HOW the files were generated! Another important thing to note is that hmmix is relying on VCFtools which only support VCF files up to format V4.2 - so if you have VCFfiles in version 4.3 you will need to change this in your header!
 
 ```note
 hmmix create_outgroup -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa -refgenome=hg19_refgenome/*fa
 hmmix mutation_rate -outgroup=outgroup.txt  -weights=strickmask.bed -window_size=1000000 -out mutationrate.bed
 hmmix create_ingroup  -ind=individuals.json -vcf=*.bcf -weights=strickmask.bed -out=obs -outgroup=outgroup.txt -ancestral=hg19_ancestral/homo_sapiens_ancestor_*.fa
 hmmix train  -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -out=trained.HG00096.json 
 hmmix decode -obs=obs.HG00096.txt -weights=strickmask.bed -mutrates=mutationrate.bed -param=trained.HG00096.json
```

### Comparing `hmmix-0.7.1/src/main.py` & `hmmix-0.7.2/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import argparse
 import numpy as np
 
-from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output, inhomogeneous
+from hmm_functions import TrainModel, DecodeModel, write_HMM_to_file, read_HMM_parameters_from_file, Write_Decoded_output, inhomogeneous, DecodeModel_viterbi
 from bcf_vcf import make_out_group, make_ingroup_obs
 from make_test_data import create_test_data
 from make_mutationrate import make_mutation_rate
 from helper_functions import Load_observations_weights_mutrates, handle_individuals_input, handle_infiles, combined_files
 
 
-VERSION = '0.7.1'
+VERSION = '0.7.2'
 
 
 def print_script_usage():
     toprint = f'''
 Script for identifying introgressed archaic segments (version: {VERSION})
 
 > Turorial:
@@ -66,14 +66,15 @@
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
     -out                outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)
     -window_size        size of bins (default is 1000 bp)
     -haploid            Change from using diploid data to haploid data (default is diploid)
     -admixpop           Annotate using vcffile with admixing population (default is none)
     -extrainfo          Add variant position for each SNP (default is off)
+    -viterbi            decode using the viterbi algorithm (default is posterior decoding)
 
 > inhomogeneous                
     -obs                [required] file with observation data
     -chrom              Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3 (default is use all chromosomes)
     -weights            file with callability (defaults to all positions being called)
     -mutrates           file with mutation rates (default is mutation rate is uniform)
     -param              markov parameters file (default is human/neanderthal like parameters)
@@ -146,14 +147,15 @@
     decode_subparser.add_argument("-mutrates", metavar='',help="file with mutation rates (default is mutation rate is uniform)")
     decode_subparser.add_argument("-param", metavar='',help="markov parameters file (default is human/neanderthal like parameters)", type=str)
     decode_subparser.add_argument("-out", metavar='',help="outputfile prefix <out>.hap1.txt and <out>.hap2.txt if -haploid option is used or <out>.diploid.txt (default is stdout)", default = '/dev/stdout')
     decode_subparser.add_argument("-window_size", metavar='',help="size of bins (default is 1000 bp)", type=int, default = 1000)
     decode_subparser.add_argument("-haploid",help="Change from using diploid data to haploid data (default is diploid)", action='store_true', default = False)
     decode_subparser.add_argument("-admixpop",help="Annotate using vcffile with admixing population (default is none)")
     decode_subparser.add_argument("-extrainfo",help="Add archaic information on each SNP", action='store_true', default = False)
+    decode_subparser.add_argument("-viterbi",help="Decode using the Viterbi algorithm", action='store_true', default = False)
 
     # inhomogeneous markov chain
     inhomogen_subparser = subparser.add_parser('inhomogeneous', help='Make inhomogen markov chain')
     inhomogen_subparser.add_argument("-obs",help="[required] file with observation data", type=str, required = True)
     inhomogen_subparser.add_argument("-chrom",help="Subset to chromosome or comma separated list of chromosomes e.g chr1 or chr1,chr2,chr3", type=str, default='All')
     inhomogen_subparser.add_argument("-weights", metavar='',help="file with callability (defaults to all positions being called)")
     inhomogen_subparser.add_argument("-mutrates", metavar='',help="file with mutation rates (default is mutation rate is uniform)")
@@ -206,28 +208,35 @@
 
     # Decode observations using parameters
     # ------------------------------------------------------------------------------------------------------------
     elif args.mode == 'decode':
 
         obs, chroms, starts, variants, mutrates, weights  = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid, args.chrom)
         hmm_parameters = read_HMM_parameters_from_file(args.param)
-        
+
         print('-' * 40)
         print(hmm_parameters)  
         print(f'> chromosomes to use: {args.chrom}')
         print('> number of windows:', len(obs), '. Number of snps = ', sum(obs))
         print('> total callability:', round(np.sum(weights) / len(obs),2) )
         print('> average mutation rate per bin:', round(np.sum(mutrates * weights) / np.sum(weights), 2) )
         print('> Output prefix is',args.out) 
         print('> Window size is',args.window_size, 'bp') 
-        print('> Haploid',args.haploid) 
+        print('> Haploid',args.haploid)      
+        if args.viterbi:
+            print('> Decode using viterbi algorithm') 
+        else:
+            print('> Decode with posterior decoding') 
         print('-' * 40)
 
         # Find segments and write output
-        segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
+        if args.viterbi:
+            segments = DecodeModel_viterbi(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
+        else:
+            segments = DecodeModel(obs, chroms, starts, variants, mutrates, weights, hmm_parameters)
         Write_Decoded_output(args.out, segments, args.obs, args.admixpop, args.extrainfo)
 
     # inhomogeneous markov chain
     # ------------------------------------------------------------------------------------------------------------
     elif args.mode == 'inhomogeneous':
 
         obs, chroms, starts, variants, mutrates, weights  = Load_observations_weights_mutrates(args.obs, args.weights, args.mutrates, args.window_size, args.haploid, args.chrom)
@@ -289,14 +298,15 @@
 
         # Get a list of ingroup individuals
         ingroup_individuals = handle_individuals_input(args.ind,'ingroup')
 
         # Get a list of vcffiles and ancestral files and intersect them
         vcffiles = handle_infiles(args.vcf)
         ancestralfiles = handle_infiles(args.ancestral)
+
         ancestralfiles, vcffiles  = combined_files(ancestralfiles, vcffiles)
 
         print('-' * 40)
         print('> Ingroup individuals:', len(ingroup_individuals))
         print('> Using vcf and ancestral files')
         for vcffile, ancestralfile in zip(vcffiles, ancestralfiles):
             print('vcffile:',vcffile, 'ancestralfile:',ancestralfile)
```

### Comparing `hmmix-0.7.1/src/make_mutationrate.py` & `hmmix-0.7.2/src/make_mutationrate.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.1/src/make_test_data.py` & `hmmix-0.7.2/src/make_test_data.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.1/test/test.py` & `hmmix-0.7.2/test/test.py`

 * *Files identical despite different names*

### Comparing `hmmix-0.7.1/test/test_main.py` & `hmmix-0.7.2/test/test_main.py`

 * *Files identical despite different names*

