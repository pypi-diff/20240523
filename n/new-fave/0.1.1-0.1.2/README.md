# Comparing `tmp/new_fave-0.1.1.tar.gz` & `tmp/new_fave-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_fave-0.1.1.tar", max compression
+gzip compressed data, was "new_fave-0.1.2.tar", max compression
```

## Comparing `new_fave-0.1.1.tar` & `new_fave-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2024-02-21 16:07:06.894339 new_fave-0.1.1/LICENSE
--rw-r--r--   0        0        0     3228 2024-05-22 14:03:09.249328 new_fave-0.1.1/README.md
--rw-r--r--   0        0        0     1434 2024-05-22 14:03:09.250138 new_fave-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      574 2024-05-21 21:01:28.578047 new_fave-0.1.1/src/new_fave/__init__.py
--rw-r--r--   0        0        0    12368 2024-05-21 21:01:28.578205 new_fave-0.1.1/src/new_fave/extract.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578240 new_fave-0.1.1/src/new_fave/measurements/__init__.py
--rw-r--r--   0        0        0    28341 2024-05-22 14:03:09.250533 new_fave-0.1.1/src/new_fave/measurements/vowel_measurement.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578638 new_fave-0.1.1/src/new_fave/optimize/__init__.py
--rw-r--r--   0        0        0     3548 2024-05-21 21:01:28.578967 new_fave-0.1.1/src/new_fave/optimize/optimize.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.579017 new_fave-0.1.1/src/new_fave/patterns/__init__.py
--rw-r--r--   0        0        0     2147 2024-05-21 21:01:28.579186 new_fave-0.1.1/src/new_fave/patterns/common_processing.py
--rw-r--r--   0        0        0     4841 2024-05-21 21:01:28.579358 new_fave-0.1.1/src/new_fave/patterns/fave_audio_textgrid.py
--rw-r--r--   0        0        0     5154 2024-05-21 21:01:28.579511 new_fave-0.1.1/src/new_fave/patterns/fave_corpus.py
--rw-r--r--   0        0        0     5626 2024-05-21 21:01:28.579682 new_fave-0.1.1/src/new_fave/patterns/fave_subcorpora.py
--rw-r--r--   0        0        0     6623 2024-05-21 21:01:28.579857 new_fave-0.1.1/src/new_fave/patterns/writers.py
--rw-r--r--   0        0        0     4801 2024-05-21 21:01:28.580184 new_fave-0.1.1/src/new_fave/resources/cmu2labov.yml
--rw-r--r--   0        0        0    11332 2024-05-21 21:01:28.580389 new_fave-0.1.1/src/new_fave/resources/cmu2phila.yml
--rw-r--r--   0        0        0      891 2024-05-21 21:01:28.580616 new_fave-0.1.1/src/new_fave/resources/cmu_parser.yml
--rw-r--r--   0        0        0      275 2024-05-21 21:01:28.580851 new_fave-0.1.1/src/new_fave/resources/fasttrack_config.yml
--rw-r--r--   0        0        0      427 2024-05-21 21:01:28.581070 new_fave-0.1.1/src/new_fave/resources/fave_measurement.yml
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581108 new_fave-0.1.1/src/new_fave/speaker/__init__.py
--rw-r--r--   0        0        0     4443 2024-05-21 21:01:28.581421 new_fave-0.1.1/src/new_fave/speaker/speaker.py
--rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581454 new_fave-0.1.1/src/new_fave/utils/__init__.py
--rw-r--r--   0        0        0       50 2024-05-21 21:01:28.581731 new_fave-0.1.1/src/new_fave/utils/corpus.py
--rw-r--r--   0        0        0      440 2024-05-21 21:01:28.581968 new_fave-0.1.1/src/new_fave/utils/fasttrack_config.py
--rw-r--r--   0        0        0     2516 2024-05-21 21:01:28.582099 new_fave-0.1.1/src/new_fave/utils/local_resources.py
--rw-r--r--   0        0        0     3082 2024-05-21 21:01:28.582378 new_fave-0.1.1/src/new_fave/utils/textgrid.py
--rw-r--r--   0        0        0     4677 1970-01-01 00:00:00.000000 new_fave-0.1.1/setup.py
--rw-r--r--   0        0        0     4170 1970-01-01 00:00:00.000000 new_fave-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-21 16:07:06.894339 new_fave-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3228 2024-05-22 14:03:09.249328 new_fave-0.1.2/README.md
+-rw-r--r--   0        0        0     1595 2024-05-23 15:58:20.109870 new_fave-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      574 2024-05-21 21:01:28.578047 new_fave-0.1.2/src/new_fave/__init__.py
+-rw-r--r--   0        0        0    12368 2024-05-21 21:01:28.578205 new_fave-0.1.2/src/new_fave/extract.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578240 new_fave-0.1.2/src/new_fave/measurements/__init__.py
+-rw-r--r--   0        0        0    31010 2024-05-23 15:58:20.110092 new_fave-0.1.2/src/new_fave/measurements/vowel_measurement.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.578638 new_fave-0.1.2/src/new_fave/optimize/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-23 15:58:20.110310 new_fave-0.1.2/src/new_fave/optimize/optimize.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.579017 new_fave-0.1.2/src/new_fave/patterns/__init__.py
+-rw-r--r--   0        0        0     2147 2024-05-21 21:01:28.579186 new_fave-0.1.2/src/new_fave/patterns/common_processing.py
+-rw-r--r--   0        0        0     4841 2024-05-21 21:01:28.579358 new_fave-0.1.2/src/new_fave/patterns/fave_audio_textgrid.py
+-rw-r--r--   0        0        0     5154 2024-05-21 21:01:28.579511 new_fave-0.1.2/src/new_fave/patterns/fave_corpus.py
+-rw-r--r--   0        0        0     5626 2024-05-21 21:01:28.579682 new_fave-0.1.2/src/new_fave/patterns/fave_subcorpora.py
+-rw-r--r--   0        0        0     6623 2024-05-21 21:01:28.579857 new_fave-0.1.2/src/new_fave/patterns/writers.py
+-rw-r--r--   0        0        0     4801 2024-05-21 21:01:28.580184 new_fave-0.1.2/src/new_fave/resources/cmu2labov.yml
+-rw-r--r--   0        0        0    11332 2024-05-21 21:01:28.580389 new_fave-0.1.2/src/new_fave/resources/cmu2phila.yml
+-rw-r--r--   0        0        0      891 2024-05-21 21:01:28.580616 new_fave-0.1.2/src/new_fave/resources/cmu_parser.yml
+-rw-r--r--   0        0        0      275 2024-05-23 15:58:20.110491 new_fave-0.1.2/src/new_fave/resources/fasttrack_config.yml
+-rw-r--r--   0        0        0      427 2024-05-21 21:01:28.581070 new_fave-0.1.2/src/new_fave/resources/fave_measurement.yml
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581108 new_fave-0.1.2/src/new_fave/speaker/__init__.py
+-rw-r--r--   0        0        0     4443 2024-05-21 21:01:28.581421 new_fave-0.1.2/src/new_fave/speaker/speaker.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:01:28.581454 new_fave-0.1.2/src/new_fave/utils/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-21 21:01:28.581731 new_fave-0.1.2/src/new_fave/utils/corpus.py
+-rw-r--r--   0        0        0      440 2024-05-21 21:01:28.581968 new_fave-0.1.2/src/new_fave/utils/fasttrack_config.py
+-rw-r--r--   0        0        0     2516 2024-05-21 21:01:28.582099 new_fave-0.1.2/src/new_fave/utils/local_resources.py
+-rw-r--r--   0        0        0     3082 2024-05-21 21:01:28.582378 new_fave-0.1.2/src/new_fave/utils/textgrid.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 new_fave-0.1.2/setup.py
+-rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 new_fave-0.1.2/PKG-INFO
```

### Comparing `new_fave-0.1.1/LICENSE` & `new_fave-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/README.md` & `new_fave-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/pyproject.toml` & `new_fave-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [tool.poetry]
 name = "new-fave"
-version = "0.1.1"
+version = "0.1.2"
 description = "New Vowel Extraction Suite"
 authors = ["JoFrhwld <jofrhwld@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "new_fave", from="src"}]
+homepage = "https://forced-alignment-and-vowel-extraction.github.io/new-fave/"
+repository = "https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave"
+
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 aligned-textgrid = "^0.6.6"
 fasttrackpy = "^0.4.5"
 numpy = "^1.26.4"
 tqdm = "^4.66.2"
```

### Comparing `new_fave-0.1.1/src/new_fave/__init__.py` & `new_fave-0.1.2/src/new_fave/__init__.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/extract.py` & `new_fave-0.1.2/src/new_fave/extract.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/measurements/vowel_measurement.py` & `new_fave-0.1.2/src/new_fave/measurements/vowel_measurement.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
     def winner(self):
         return self._winner
     
     @winner.setter
     def winner(self, idx):
         self._winner = self.candidates[idx]
         self.vowel_class.vowel_system._reset_winners()
+        self.vowel_class._reset_winners()
         self._expanded_formants = None
         self._optimized += 1
 
     @property
     def optimized(self):
         return self._optimized
     
@@ -260,14 +261,38 @@
             self.cand_mahals,
             df = df
         )
         if np.isfinite(log_prob).mean() < 0.5:
             log_prob = np.zeros(shape = log_prob.shape)
         return log_prob
     
+    @property
+    def cand_vclass_mahals(self):
+        N = len(self.candidates)
+        square_params = self.cand_params.reshape(-1, N)
+        inv_covmat = self.vowel_class.params_icov
+        param_means = self.vowel_class.params_means
+        x_mu = square_params - param_means
+        left = np.dot(x_mu.T, inv_covmat)
+        mahal = np.dot(left, x_mu)
+        return mahal.diagonal()
+    
+    @property
+    def cand_vclass_mahal_log_prob(self):
+        df = self.cand_params.size
+        log_prob = stats.chi2.logsf(
+            self.cand_vclass_mahals,
+            df = df
+        )
+        if np.isfinite(log_prob).mean() < 0.5:
+            log_prob = np.zeros(shape = log_prob.shape)
+        if len(self.vowel_class) < 10:
+            log_prob = np.zeros(shape = log_prob.shape)
+        return log_prob    
+    
     @property 
     def max_formant_mahal(self):
         inv_covmat = self.vowel_class.vowel_system.max_formant_icov
         maximum_formant_means = self.vowel_class.vowel_system.maximum_formant_means
         x_mu = self.cand_max_formants - maximum_formant_means
         left = np.dot(x_mu.T, inv_covmat)
         mahal = np.dot(left, x_mu)
@@ -461,14 +486,18 @@
             from the vowel class.
     """
     label: str
     tracks: list[VowelMeasurement]
     def __post_init__(self):
         super().__init__()
         self._winners = [x.winner for x in self.tracks]
+        self._winner_params = None
+        self._params_means = None
+        self._params_cov = None
+        self._params_icov = None
         for t in self.tracks:
             t.vowel_class = self
 
     def __getitem__(self, i):
         return self.tracks[i]
     
     def __len__(self):
@@ -479,14 +508,20 @@
             "VowelClass: {"
             f"label: {self.label}, "
             f"len: {len(self)}"
             "}"
         )
         return out
     
+    def _reset_winners(self):
+        self._winner_params = None
+        self._params_means = None
+        self._params_cov = None
+        self._params_icov = None
+    
     @property
     def vowel_system(self):
         return self._vowel_system
     
     @vowel_system.setter
     def vowel_system(self, vowel_system):
         self._vowel_system = vowel_system
@@ -494,22 +529,66 @@
     @property
     def winners(self):
         self._winners = [x.winner for x in self.tracks]
         return self._winners
     
     @property
     def winner_params(self):
+        if not self._winner_params is None:
+            return self._winner_params
+
         params = np.array(
             [
                 x.parameters
                 for x in self.winners
             ]
         ).T
 
         return params
+
+    @property
+    def params_means(self):
+        if self._params_means is not None:
+            return self._params_means
+        N = len(self.winners)
+        winner_mean =  self.winner_params.reshape(-1, N).mean(axis = 1)
+        winner_mean = winner_mean[:, np.newaxis]
+        self._params_means = winner_mean
+        return winner_mean
+    
+    @property
+    def params_covs(self):
+        if self._params_cov is not None:
+            return self._params_cov
+        N = len(self.winners)
+        square_param = self.winner_params.reshape(-1, N)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            param_cov = np.cov(square_param)
+        return param_cov
+    
+    @property
+    def params_icov(self):
+        if self._params_icov is not None:
+            return self._params_icov
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            try:
+                params_icov = np.linalg.inv(self.params_covs)
+                self._params_icov = params_icov
+                return params_icov
+            except:
+                params_icov = np.array([
+                    [np.nan] * self.params_covs.size
+                ]).reshape(
+                    self.params_covs.shape[0],
+                    self.params_covs.shape[1]
+                )
+                self._params_icov = params_icov
+                return params_icov    
     
     def to_param_df(
             self, 
             output:Literal["param", "log_param"] = "log_param"
         ) -> pl.DataFrame:
         """Return DataFrame of formant DCT parameters.
```

### Comparing `new_fave-0.1.1/src/new_fave/optimize/optimize.py` & `new_fave-0.1.2/src/new_fave/optimize/optimize.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from fasttrackpy.utils.safely import safely
 import numpy as np
 from tqdm import tqdm
 from typing import Literal
 
 def run_optimize(
         vowel_system: VowelClassCollection,
-        optim_params = ["cand_mahal", "max_formant"],
+        optim_params = ["cand_mahal", "vclass_mahal", "max_formant"],
         max_iter = 10
     ):
     """
     Repeatedly run optimization until either `max_iter` is reached,
     or the difference between two iterations becomes small.
 
     Args:
@@ -46,15 +46,17 @@
     
     return
 
 
 
 def optimize_vowel_measures(
         vowel_measurements: list[VowelMeasurement],
-        optim_params: list[Literal["cand_mahal", "max_formant"]] = ["cand_mahal", "max_formant"]
+        optim_params: list[
+            Literal["cand_mahal", "vclass_mahal", "max_formant"]
+            ] = ["cand_mahal", "vclass_mahal", "max_formant"]
     ):
     """
     Optimize a list of VowelMeasurements.
 
     Args:
         vowel_measurements (list[VowelMeasurement]): 
             The list of vowel measurements to optimize
@@ -73,15 +75,17 @@
     
     for vm, idx in zip(vowel_measurements, new_winners):
         vm.winner = idx
 
 @safely(message="There was a problem optimizing a vowel.")
 def optimize_one_measure(
         vowel_measurement: VowelMeasurement,
-         optim_params: list[Literal["cand_mahal", "max_formant"]] = ["cand_mahal", "max_formant"]
+         optim_params: list[
+             Literal["cand_mahal", "vclass_mahal", "max_formant"]
+             ] = ["cand_mahal", "vclass_mahal", "max_formant"]
     )->int:
     """
     This function optimizes a given vowel measurement based on the 
     specified optimization parameters. The optimization parameters 
     can include 'cand_mahal' and 'max_formant'.
 
     Args:
@@ -94,14 +98,17 @@
         (int): The index of the winning candidate.
     """
     prob_dict = dict()
 
     if "cand_mahal" in optim_params:
         prob_dict["cand_mahal"] = vowel_measurement.cand_mahal_log_prob
 
+    if "vclass_mahal" in optim_params:
+        prob_dict["vclass_mahal"] = vowel_measurement.cand_vclass_mahal_log_prob
+
     if "max_formant" in optim_params:
         prob_dict["max_formant"] = vowel_measurement.max_formant_log_prob
         
     joint_prob = vowel_measurement.error_log_prob 
     for dim in optim_params:
         joint_prob += prob_dict[dim]
```

### Comparing `new_fave-0.1.1/src/new_fave/patterns/common_processing.py` & `new_fave-0.1.2/src/new_fave/patterns/common_processing.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/patterns/fave_audio_textgrid.py` & `new_fave-0.1.2/src/new_fave/patterns/fave_audio_textgrid.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/patterns/fave_corpus.py` & `new_fave-0.1.2/src/new_fave/patterns/fave_corpus.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/patterns/fave_subcorpora.py` & `new_fave-0.1.2/src/new_fave/patterns/fave_subcorpora.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/patterns/writers.py` & `new_fave-0.1.2/src/new_fave/patterns/writers.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/resources/cmu2labov.yml` & `new_fave-0.1.2/src/new_fave/resources/cmu2labov.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/resources/cmu2phila.yml` & `new_fave-0.1.2/src/new_fave/resources/cmu2phila.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/resources/cmu_parser.yml` & `new_fave-0.1.2/src/new_fave/resources/cmu_parser.yml`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/speaker/speaker.py` & `new_fave-0.1.2/src/new_fave/speaker/speaker.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/utils/local_resources.py` & `new_fave-0.1.2/src/new_fave/utils/local_resources.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/src/new_fave/utils/textgrid.py` & `new_fave-0.1.2/src/new_fave/utils/textgrid.py`

 * *Files identical despite different names*

### Comparing `new_fave-0.1.1/setup.py` & `new_fave-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
  ':sys_platform == "win32"': ['python-magic-bin>=0.4.14,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['fave-extract = new_fave.extract:fave_extract']}
 
 setup_kwargs = {
     'name': 'new-fave',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'New Vowel Extraction Suite',
     'long_description': '# new-fave\n\n![PyPI](https://img.shields.io/pypi/v/new-fave.png) [![Python CI](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave/graph/badge.svg?token=8JRGOB9NMN)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave) [![Maintainability](https://api.codeclimate.com/v1/badges/2f00920067765c0ad77f/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/new-fave/maintainability) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n## What is `new-fave`?\n\n`new-fave` is a tool for automating and optimizing vowel formant extraction. It is philosophically similar (and named after) [the FAVE-suite](https://github.com/JoFrhwld/FAVE). However, `new-fave` has been completely written from scratch, and has some key differences from the FAVE-suite.\n\n1. **`new-fave` does not include a forced-aligner.**\n    It can process alignments produced by fave-align, \n    but we would recommend using the Monteal Forced Aligner instead\n2. **`new-fave` does not require speaker demographics.**\n    You can optionally pass `fave-extract` a speaker\n    demographics file to be merged into your formant data,\n    but this does *not* influence how the data is processed\n    in any way. Besides including file name and speaker\n    number data, you can pass *any* demographic information\n    you would like.\n3. **`new-fave` does not assume North American English vowels**.\n    Your alignments can contain any set of vowels, in\n    any transcription system, as long as you can provide \n    a regular expression to identify them.\n4. **`new-fave` is customizable.**\n    With config files, you can customize vowel recoding,\n    labelset parsing, and point measurement heuristics.\n5. **`new-fave` is focused on formant tracks.**\n    You can still produce single point measurements \n    for vowels, but `new-fave` is built upon \n    the [FastTrack](https://fasttrackiverse.github.io/fasttrackpy/) method. By default, it will write \n    output files including point measurements, full\n    formant tracks, and Discrete Cosine Transform \n    coefficients.\n6. **`new-fave` is maintainable**. As time goes on, and the \n    code base needs updating, the organization and \n    infrastructure of `new-fave` should allow it to be\n    readilly updateable.\n\nYou can read more at [the `new-fave` documentation](https://forced-alignment-and-vowel-extraction.github.io/new-fave/).\n\n## Installation\n\nYou can install `new-fave` with `pip`.\n\n```bash\n# bash\npip install new-fave\n```\n\n## Usage\n\nTo use the default settings (which assume CMU \ndictionary transcriptions), you can use one of these \npatterns.\n\n### A single audio + textgrid pair\n\n```bash\n# bash\nfave-extract audio-textgrid speaker1.wav speaker1.TextGrid\n```\n\n### A directory of audio + textgrid pairs\n\n```bash\n# bash\nfave-extract corpus speakers/\n```\n\n### Multiple subdirectories of audio + textgrid pairs\n\n```bash\n# bash\nfave-extract subcorpora data/*\n```',
     'author': 'JoFrhwld',
     'author_email': 'jofrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://forced-alignment-and-vowel-extraction.github.io/new-fave/',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.11,<3.12',
```

### Comparing `new_fave-0.1.1/PKG-INFO` & `new_fave-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: new-fave
-Version: 0.1.1
+Version: 0.1.2
 Summary: New Vowel Extraction Suite
+Home-page: https://forced-alignment-and-vowel-extraction.github.io/new-fave/
 License: GPLv3
 Author: JoFrhwld
 Author-email: jofrhwld@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -17,14 +18,15 @@
 Requires-Dist: fave-recode (>=0.3.0,<0.4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0) ; sys_platform != "win32"
 Requires-Dist: python-magic-bin (>=0.4.14,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xlsx2csv (>=0.8.2,<0.9.0)
+Project-URL: Repository, https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave
 Description-Content-Type: text/markdown
 
 # new-fave
 
 ![PyPI](https://img.shields.io/pypi/v/new-fave.png) [![Python CI](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml/badge.svg)](https://github.com/Forced-Alignment-and-Vowel-Extraction/new-fave/actions/workflows/test-and-run.yml) [![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave/graph/badge.svg?token=8JRGOB9NMN)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/new-fave) [![Maintainability](https://api.codeclimate.com/v1/badges/2f00920067765c0ad77f/maintainability)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/new-fave/maintainability) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 ## What is `new-fave`?
```

