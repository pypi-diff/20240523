# Comparing `tmp/yappgen-0.3.3.tar.gz` & `tmp/yappgen-0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappgen-0.3.3.tar", last modified: Tue Apr 23 14:17:52 2024, max compression
+gzip compressed data, was "yappgen-0.4.dev0.tar", last modified: Thu May 23 16:25:53 2024, max compression
```

## Comparing `yappgen-0.3.3.tar` & `yappgen-0.4.dev0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 14:17:52.602680 yappgen-0.3.3/
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    26526 2023-04-12 12:19:27.000000 yappgen-0.3.3/LICENSE
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     1116 2024-04-23 14:17:52.602680 yappgen-0.3.3/PKG-INFO
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      804 2024-04-23 13:44:26.000000 yappgen-0.3.3/README.md
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 14:17:52.602680 yappgen-0.3.3/bin/
--rwxrwxr-x   0 bservin   (1001) bservin   (1001)     6130 2023-04-12 12:19:27.000000 yappgen-0.3.3/bin/fphtrain
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     5021 2023-04-12 12:19:27.000000 yappgen-0.3.3/bin/yapp
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      186 2024-04-23 14:17:52.602680 yappgen-0.3.3/setup.cfg
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      812 2024-04-23 13:44:26.000000 yappgen-0.3.3/setup.py
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 14:17:52.602680 yappgen-0.3.3/yapp/
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      138 2024-04-23 14:16:46.000000 yappgen-0.3.3/yapp/__init__.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    36668 2024-04-23 14:13:13.000000 yappgen-0.3.3/yapp/family_phaser.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     8029 2024-04-23 13:48:37.000000 yappgen-0.3.3/yapp/gamete.py
--rwxrwxr-x   0 bservin   (1001) bservin   (1001)    10173 2023-04-12 12:19:27.000000 yappgen-0.3.3/yapp/lmm.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     5669 2024-04-23 14:12:17.000000 yappgen-0.3.3/yapp/mendel.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     6721 2024-04-23 14:13:29.000000 yappgen-0.3.3/yapp/origins.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    15770 2024-04-23 13:44:26.000000 yappgen-0.3.3/yapp/pedigree.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    20467 2024-04-23 13:49:53.000000 yappgen-0.3.3/yapp/recombination.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     7179 2024-04-23 14:13:50.000000 yappgen-0.3.3/yapp/sperm.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)    11770 2024-04-23 14:14:57.000000 yappgen-0.3.3/yapp/vcf.py
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     5873 2023-04-12 12:19:27.000000 yappgen-0.3.3/yapp/wcsp.py
-drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-04-23 14:17:52.602680 yappgen-0.3.3/yappgen.egg-info/
--rw-rw-r--   0 bservin   (1001) bservin   (1001)     1116 2024-04-23 14:17:52.000000 yappgen-0.3.3/yappgen.egg-info/PKG-INFO
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      417 2024-04-23 14:17:52.000000 yappgen-0.3.3/yappgen.egg-info/SOURCES.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-04-23 14:17:52.000000 yappgen-0.3.3/yappgen.egg-info/dependency_links.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2023-04-12 12:23:00.000000 yappgen-0.3.3/yappgen.egg-info/not-zip-safe
--rw-rw-r--   0 bservin   (1001) bservin   (1001)      106 2024-04-23 14:17:52.000000 yappgen-0.3.3/yappgen.egg-info/requires.txt
--rw-rw-r--   0 bservin   (1001) bservin   (1001)        5 2024-04-23 14:17:52.000000 yappgen-0.3.3/yappgen.egg-info/top_level.txt
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    26526 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/LICENSE
+-rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      803 2024-04-24 07:23:10.000000 yappgen-0.4.dev0/README.md
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      781 2024-05-23 16:25:50.000000 yappgen-0.4.dev0/pyproject.toml
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      186 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/setup.cfg
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/yapp/
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      158 2024-05-23 16:13:53.000000 yappgen-0.4.dev0/src/yapp/__init__.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     5143 2024-05-23 16:07:40.000000 yappgen-0.4.dev0/src/yapp/cmd.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    36885 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/family_phaser.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)     6130 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/fphtrain.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     8029 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/gamete.py
+-rwxrwxr-x   0 bservin   (1001) bservin   (1001)    10173 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/lmm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5844 2024-04-24 07:25:07.000000 yappgen-0.4.dev0/src/yapp/mendel.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    17102 2024-05-23 16:05:13.000000 yappgen-0.4.dev0/src/yapp/origins.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    15828 2024-04-24 07:23:10.000000 yappgen-0.4.dev0/src/yapp/pedigree.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    20484 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/recombination.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     7179 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/sperm.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)    11770 2024-04-24 07:23:14.000000 yappgen-0.4.dev0/src/yapp/vcf.py
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)     5873 2023-04-12 12:19:27.000000 yappgen-0.4.dev0/src/yapp/wcsp.py
+drwxrwxr-x   0 bservin   (1001) bservin   (1001)        0 2024-05-23 16:25:53.271154 yappgen-0.4.dev0/src/yappgen.egg-info/
+-rw-r--r--   0 bservin   (1001) bservin   (1001)     1331 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/PKG-INFO
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)      510 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/SOURCES.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        1 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/dependency_links.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       69 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/entry_points.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)       93 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/requires.txt
+-rw-rw-r--   0 bservin   (1001) bservin   (1001)        5 2024-05-23 16:25:53.000000 yappgen-0.4.dev0/src/yappgen.egg-info/top_level.txt
```

### Comparing `yappgen-0.3.3/LICENSE` & `yappgen-0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/README.md` & `yappgen-0.4.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 @BertrandServin). If you want to contribute ideas or code, you are
 welcome if you know python :)
 
 yapp and its utilities implement some models and methods that have been
 invented by other people. If you use yapp it is important that you
 acknowledge their work by citing the appropriate
 references. These will depend on the way you use the software, see the
-[documentation](https://yapp-doc.netlify.app).
+[documentation](https://yapp.readthedocs.io).
```

### Comparing `yappgen-0.3.3/bin/fphtrain` & `yappgen-0.4.dev0/src/yapp/fphtrain.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/bin/yapp` & `yappgen-0.4.dev0/src/yapp/cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     # Origins
     parser_origins = subparsers.add_parser(
         "origins", help="Trace down ancestral origins from phased data in pedigree"
     )
     parser_origins.add_argument(
         "prfx", type=str, help="prefix for input / output files"
     )
+    parser_origins.add_argument(
+        "-L", type=int, help="consider IBD if IBS matches >= m markers",
+        metavar="m",
+        default = 10
+    )
     parser_origins.set_defaults(func=origins.main)
 
     # Sperm
     parser_sperm = subparsers.add_parser(
         "sperm", help='Infer parental chromosomes from "sperm typing" data'
     )
     parser_sperm.add_argument("prfx", type=str, help="prefix for input / output files")
@@ -129,15 +134,16 @@
         default=0.99,
     )
     parser_sperm.set_defaults(func=sperm.main)
 
     return parser
 
 
-def main(args):
+def main():
+    args = sys.argv
     parser = yapp_parser()
     if len(args) < 2:
         parser.print_help()
         sys.exit(1)
     myopts = parser.parse_args(args[1:])
     # Set up logging
     logger = logging.getLogger("yapp")
@@ -158,11 +164,7 @@
         ch.setLevel(logging.INFO)
         ch.setFormatter(formatter)
         logger.addHandler(ch)
 
     logger.info(f"Starting YAPP {myopts.command} analysis")
     myopts.func(myopts)
     logger.info(f"Finished YAPP {myopts.command} analysis")
-
-
-if __name__ == "__main__":
-    main(sys.argv)
```

### Comparing `yappgen-0.3.3/yapp/family_phaser.py` & `yappgen-0.4.dev0/src/yapp/family_phaser.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,38 +220,46 @@
         rew = np.ones((self.len, 2), dtype=float)  # Backward
         sca = np.ones(self.len, dtype=float)  # scaling
 
         # Compute forward probabilities
         fwd[0, 0] = 0.5 * emissions[0, 0]
         fwd[0, 1] = 0.5 * emissions[0, 1]
         sca[0] = 1.0 / (fwd[0, 0] + fwd[0, 1])
-        fwd[0,] *= sca[0]
+        fwd[
+            0,
+        ] *= sca[0]
         for m in range(1, self.len):
             fwd[m, 0] = (
                 fwd[m - 1, 0] * transitions[m - 1, 0, 0]
                 + fwd[m - 1, 1] * transitions[m - 1, 1, 0]
             ) * emissions[m, 0]
             fwd[m, 1] = (
                 fwd[m - 1, 0] * transitions[m - 1, 0, 1]
                 + fwd[m - 1, 1] * transitions[m - 1, 1, 1]
             ) * emissions[m, 1]
             sca[m] = 1.0 / (fwd[m, 0] + fwd[m, 1])
-            fwd[m,] *= sca[m]
+            fwd[
+                m,
+            ] *= sca[m]
         # Compute backward probabilities
-        rew[self.len - 1,] /= sca[m - 1]
+        rew[
+            self.len - 1,
+        ] /= sca[m - 1]
         for m in range(self.len - 1, 0, -1):
             rew[m - 1, 0] = (
                 transitions[m - 1, 0, 0] * emissions[m, 0] * rew[m, 0]
                 + transitions[m - 1, 0, 1] * emissions[m, 1] * rew[m, 1]
             )
             rew[m - 1, 1] = (
                 transitions[m - 1, 1, 0] * emissions[m, 0] * rew[m, 0]
                 + transitions[m - 1, 1, 1] * emissions[m, 1] * rew[m, 1]
             )
-            rew[m - 1,] *= sca[m - 1]
+            rew[
+                m - 1,
+            ] *= sca[m - 1]
         # loglik = -np.sum(np.log(sca))
         # Compute Posterior probabilities
         post_si = fwd * rew
         post_si /= np.sum(post_si, axis=1, keepdims=True)  # required ?
 
         # 3. Viterbi Algorithm
         # viterbi variables
@@ -272,15 +280,19 @@
                 delta[m - 1, 1] + np.log(transitions[m - 1, 1, 1]),
             ]
             psi[m, 0] = np.argmax(val_0)
             psi[m, 1] = np.argmax(val_1)
             delta[m, 0] = val_0[psi[m, 0]] + np.log(emissions[m, 0])
             delta[m, 1] = val_1[psi[m, 1]] + np.log(emissions[m, 1])
         # termination / backtracking
-        soluce[-1] = np.argmax(delta[-1,])
+        soluce[-1] = np.argmax(
+            delta[
+                -1,
+            ]
+        )
         for m in range(self.len - 1, 0, -1):
             soluce[m - 1] = psi[m, soluce[m]]
         result = [(x, post_si[i, x]) for i, x in enumerate(soluce)]
         return result
 
     def update_paternal_gamete(self, prop_gam):
         return self.update_gamete(prop_gam, 0)
@@ -389,15 +401,17 @@
         prfx : str
            Prefix of input files
         **kwargs : arguments
            Optional arguments to pass to yapp.vcf.vcf2fph
         """
         vcf_file = f"{prfx}.vcf.gz"
         fam_file = f"{prfx}.fam"
-        obj = cls(vcf_file, fam_file, prfx, region=region, focalID=focalID, err=err)
+        obj = cls(
+            vcf_file, fam_file, prfx, region=region, focalID=focalID, err=err, rho=rho
+        )
         print(obj.data.tree())
         return obj
 
     @property
     def regions(self):
         return self.data["regions"]
 
@@ -477,15 +491,17 @@
         obj.__class__ = cls
         return obj
 
     def get_genotypes(self, region):
         data = {}
         genotypes = np.array(self.data["genotypes"][region])
         for i, name in enumerate(self.data["samples"]):
-            data[name] = genotypes[i,]
+            data[name] = genotypes[
+                i,
+            ]
         return data
 
     def get_mendelian_genotypes(self, region):
         genotypes = self.get_genotypes(region)
         for node in self.pedigree:
             pg = genotypes[node.indiv]
             for child in node.children:
```

### Comparing `yappgen-0.3.3/yapp/gamete.py` & `yappgen-0.4.dev0/src/yapp/gamete.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/yapp/lmm.py` & `yappgen-0.4.dev0/src/yapp/lmm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/yapp/mendel.py` & `yappgen-0.4.dev0/src/yapp/mendel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import os
 import logging
 from collections import defaultdict
 from multiprocessing import Pool
 import numpy as np
 from scipy.stats import binom
+from numba import jit
 from cyvcf2 import VCF
 from . import vcf, pedigree
 
 logger = logging.getLogger(__name__)
 
-
 def genotype_vector(genotypes):
     return np.array([vcf.geno2int(*g[:2]) for g in genotypes], dtype=int)
 
-
 def mendel_errors(args):
     genotypes, pairs = args
     pairs = np.array(pairs)
     genotypes = np.array(genotypes)
     from_genotypes = np.array(genotypes)[pairs[:, 0], :2]
     to_genotypes = np.array(genotypes)[pairs[:, 1], :2]
     fg = genotype_vector(from_genotypes)
     tg = genotype_vector(to_genotypes)
-    nobs = (fg > 0) & (tg > 0)
+    nobs = ((fg == 0) | (fg == 2)) & ((tg == 0) | (tg == 2))
     nerr = ((fg == 0) & (tg == 2)) | ((fg == 2) & (tg == 0))
     return nerr, nobs
 
 
-def identify_bad_pairs(pairs, merr, fpr=1e-3):
+def identify_bad_pairs(pairs, merr, fpr=1e-3, iterate = False):
     """Identify outliers for mendelian errors.
 
     Starting from all pairs, outliers are identified iteratively as follows:
 
     1. Compute overal error rate
     2. For each pair compute the p-value (from Binomial) that data comes
        from the binomial
     3. reject the null is p-value < fpr/len(pairs) (Bonferroni correction)
     4. Remove pairs for which the null is rejected from the pair list
 
-    These steps are iterated until no pair is removed from the set.
+    If iterate, these steps are iterated until no pair is removed from the set.
 
     Arguments
     ---------
     pairs : list of objects
         family links
     merr : array len(pairs) x 2
         array of number of errors (merr[:,0]) and number of
@@ -68,15 +67,15 @@
         for i, (p, e) in enumerate(zip(current_pairs, current_merr)):
             pval = binom.sf(n=e[1], p=tx_err, k=e[0])
             if pval < pval_th:
                 logger.debug(f"{p} : pbinom({e[0]}, size={e[1]},  p={tx_err}) = {pval}")
                 pair2rm.append(p)
                 tmp_pairs.remove(p)
                 keepidx[i] = False
-        if keepidx.all():
+        if not iterate or keepidx.all():
             break
         logger.debug(f"Start with {len(current_pairs)} -> {len(tmp_pairs)}")
         current_pairs = tmp_pairs[:]
         current_merr = current_merr[keepidx, :]
     return pair2rm
 
 
@@ -101,31 +100,33 @@
     for node in ped:
         if indiv_idx[node.indiv] < 0:
             continue
         for c in node.children:
             if indiv_idx[c.indiv] < 0:
                 continue
             pairs.append((indiv_idx[node.indiv], indiv_idx[c.indiv]))
+
+    logger.info(f"Found {len(pairs)} offspring-parents pairs to check")
     # pairs = np.array(pairs, dtype=int)
 
     geno_getter = ((s.genotypes, pairs) for s in myvcf)
     merr = np.zeros((len(pairs), 2), dtype=int)
     with Pool(args.c) as workers:
         for nerr, nobs in workers.imap_unordered(
-            mendel_errors, geno_getter, chunksize=50
+            mendel_errors, geno_getter#, chunksize=1000
         ):
             merr[:, 0] += nerr
             merr[:, 1] += nobs
     tx_err = np.sum(merr[:, 0]) / np.sum(merr[:, 1])
     # pval_th = 0.001/pairs.shape[0]
 
     logger.info(f"Global Mendel Error rate : {tx_err:.2g}")
     # unset_links=[]
     unset_links = identify_bad_pairs(pairs, merr)
-    with open(f"{prfx}.mendel.err", "w") as fout:
+    with open(f"{prfx}_yapp_mendel.err", "w") as fout:
         print("parent offspring nerr nobs err.rate pvalue removed", file=fout)
         for p, e in zip(pairs, merr):
             pval = binom.sf(n=e[1], p=tx_err, k=e[0])
             print(
                 f"{myvcf.samples[p[0]]} "
                 f"{myvcf.samples[p[1]]} "
                 f"{e[0]} {e[1]} {e[0]/e[1]:.2g} {pval:.2g} "
```

### Comparing `yappgen-0.3.3/yapp/pedigree.py` & `yappgen-0.4.dev0/src/yapp/pedigree.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,11 +507,12 @@
         individual in the pedigree
 
         """
         try:
             node = self.nodes[indiv]
         except KeyError:
             raise ValueError(f"Focal individual {indiv} not found in pedigree")
-        sys.setrecursionlimit(len(self.nodes) + 1)
+        if len(self.nodes) > sys.getrecursionlimit():
+            sys.setrecursionlimit(len(self.nodes) + 1)
         relatives = self._get_relatives(node)
         fam = Pedigree.from_pednodes(relatives)
         return fam
```

### Comparing `yappgen-0.3.3/yapp/recombination.py` & `yappgen-0.4.dev0/src/yapp/recombination.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,30 +317,30 @@
                         if len(infomk) > 0:
                             infomk_l = min(infomk)
                             infomk_r = max(infomk)
                             par.add_offspring_coverage(
                                 node.indiv, chrom, pos[infomk_l], pos[infomk_r]
                             )
 
-    def write_results(self, prefix):
-        with open(prefix + "_yapp_recomb_coverage.txt", "w") as fout:
+    def write_results(self):
+        with open(self.phaser.prefix + "_yapp_recomb_coverage.txt", "w") as fout:
             print("parent sex offspring chrom left right", file=fout)
             for name, par in self.parents.items():
                 for off in par.coverage:
                     for chrom in par.coverage[off]:
                         print(
                             f"{name} "
                             f"{((par.sex==None) and 'U') or ((par.sex==MALE) and 'M' or 'F')} "  # noqa
                             f"{off} "
                             f"{chrom} "
                             f"{par.coverage[off][chrom][0]} "
                             f"{par.coverage[off][chrom][1]}",
                             file=fout,
                         )
-        with open(prefix + "_yapp_recombinations.txt", "w") as fout:
+        with open(self.phaser.prefix + "_yapp_recombinations.txt", "w") as fout:
             print("parent sex offspring chrom left right", file=fout)
             for name, par in self.parents.items():
                 for off in par.meioses:
                     for co in sorted(par.meioses[off]):
                         print(
                             f"{name} "
                             f"{((par.sex==None) and 'U') or ((par.sex==MALE) and 'M' or 'F')} "  # noqa
@@ -571,11 +571,11 @@
                 raise
             return float(self.right - w_left) / (self.right - self.left)
 
 
 def main(args):
     prfx = args.prfx
 
-    phaser_db = prfx + ".db"
+    phaser_db = prfx + "_yapp.db"
     analyzer = RecombAnalyser(phaser_db)
     analyzer.run(recrate=args.rho, call=args.minsp)
-    analyzer.write_results(prfx)
+    analyzer.write_results()
```

### Comparing `yappgen-0.3.3/yapp/sperm.py` & `yappgen-0.4.dev0/src/yapp/sperm.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/yapp/vcf.py` & `yappgen-0.4.dev0/src/yapp/vcf.py`

 * *Files identical despite different names*

### Comparing `yappgen-0.3.3/yapp/wcsp.py` & `yappgen-0.4.dev0/src/yapp/wcsp.py`

 * *Files identical despite different names*

