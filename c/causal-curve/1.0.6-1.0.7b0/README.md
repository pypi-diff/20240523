# Comparing `tmp/causal-curve-1.0.6.tar.gz` & `tmp/causal_curve-1.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal-curve-1.0.6.tar", last modified: Mon Apr 26 00:05:35 2021, max compression
+gzip compressed data, was "causal_curve-1.0.7b0.tar", last modified: Thu May 23 19:18:18 2024, max compression
```

## Comparing `causal-curve-1.0.6.tar` & `causal_curve-1.0.7b0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 roni_kobrosly   (501) staff       (20)        0 2021-04-26 00:05:35.750985 causal-curve-1.0.6/
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     1070 2021-04-25 23:38:35.000000 causal-curve-1.0.6/LICENSE
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     5068 2021-04-26 00:05:35.750729 causal-curve-1.0.6/PKG-INFO
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     3750 2021-04-25 23:38:35.000000 causal-curve-1.0.6/README.md
-drwxr-xr-x   0 roni_kobrosly   (501) staff       (20)        0 2021-04-26 00:05:35.748757 causal-curve-1.0.6/causal_curve/
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)      491 2021-04-25 23:38:35.000000 causal-curve-1.0.6/causal_curve/__init__.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     2044 2021-04-26 00:04:57.000000 causal-curve-1.0.6/causal_curve/core.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     4357 2021-04-25 23:38:35.000000 causal-curve-1.0.6/causal_curve/gps_classifier.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)    28024 2021-04-26 00:04:57.000000 causal-curve-1.0.6/causal_curve/gps_core.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     6082 2021-04-25 23:38:35.000000 causal-curve-1.0.6/causal_curve/gps_regressor.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)    23898 2021-04-25 23:38:35.000000 causal-curve-1.0.6/causal_curve/mediation.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)    23023 2021-04-26 00:04:57.000000 causal-curve-1.0.6/causal_curve/tmle_core.py
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     5296 2021-04-25 23:38:35.000000 causal-curve-1.0.6/causal_curve/tmle_regressor.py
-drwxr-xr-x   0 roni_kobrosly   (501) staff       (20)        0 2021-04-26 00:05:35.749740 causal-curve-1.0.6/causal_curve.egg-info/
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     5068 2021-04-26 00:05:35.000000 causal-curve-1.0.6/causal_curve.egg-info/PKG-INFO
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)      420 2021-04-26 00:05:35.000000 causal-curve-1.0.6/causal_curve.egg-info/SOURCES.txt
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)        1 2021-04-26 00:05:35.000000 causal-curve-1.0.6/causal_curve.egg-info/dependency_links.txt
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)      169 2021-04-26 00:05:35.000000 causal-curve-1.0.6/causal_curve.egg-info/requires.txt
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)       13 2021-04-26 00:05:35.000000 causal-curve-1.0.6/causal_curve.egg-info/top_level.txt
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)       38 2021-04-26 00:05:35.751299 causal-curve-1.0.6/setup.cfg
--rw-r--r--   0 roni_kobrosly   (501) staff       (20)     1196 2021-04-26 00:04:57.000000 causal-curve-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:18:18.886640 causal_curve-1.0.7b0/
+-rw-rw-rw-   0        0        0     1091 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/LICENSE
+-rw-rw-rw-   0        0        0     4931 2024-05-23 19:18:18.883639 causal_curve-1.0.7b0/PKG-INFO
+-rw-rw-rw-   0        0        0     3869 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:18:18.858260 causal_curve-1.0.7b0/causal_curve/
+-rw-rw-rw-   0        0        0      507 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/__init__.py
+-rw-rw-rw-   0        0        0     2139 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/core.py
+-rw-rw-rw-   0        0        0     4486 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/gps_classifier.py
+-rw-rw-rw-   0        0        0    28755 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/gps_core.py
+-rw-rw-rw-   0        0        0     6246 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/gps_regressor.py
+-rw-rw-rw-   0        0        0    24565 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/mediation.py
+-rw-rw-rw-   0        0        0    23632 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/tmle_core.py
+-rw-rw-rw-   0        0        0     5435 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/causal_curve/tmle_regressor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:18:18.882647 causal_curve-1.0.7b0/causal_curve.egg-info/
+-rw-rw-rw-   0        0        0     4931 2024-05-23 19:18:18.000000 causal_curve-1.0.7b0/causal_curve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2024-05-23 19:18:18.000000 causal_curve-1.0.7b0/causal_curve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:18:18.000000 causal_curve-1.0.7b0/causal_curve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      169 2024-05-23 19:18:18.000000 causal_curve-1.0.7b0/causal_curve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 19:18:18.000000 causal_curve-1.0.7b0/causal_curve.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:18:18.887640 causal_curve-1.0.7b0/setup.cfg
+-rw-rw-rw-   0        0        0     1241 2024-05-23 19:17:51.000000 causal_curve-1.0.7b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:18:18.880535 causal_curve-1.0.7b0/tests/
+-rw-rw-rw-   0        0        0      447 2024-05-23 17:07:23.000000 causal_curve-1.0.7b0/tests/test_helpers.py
```

### Comparing `causal-curve-1.0.6/LICENSE` & `causal_curve-1.0.7b0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Roni Kobrosly
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Roni Kobrosly
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `causal-curve-1.0.6/README.md` & `causal_curve-1.0.7b0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-# causal-curve
-
-[![build status](http://img.shields.io/travis/ronikobrosly/causal-curve/main.svg?style=flat)](https://travis-ci.org/ronikobrosly/causal-curve)
-[![codecov](https://codecov.io/gh/ronikobrosly/causal-curve/branch/main/graph/badge.svg)](https://codecov.io/gh/ronikobrosly/causal-curve)
-[![DOI](https://zenodo.org/badge/256017107.svg)](https://zenodo.org/badge/latestdoi/256017107)
-
-Python tools to perform causal inference when the treatment of interest is continuous.
-
-
-<p align="center">
-<img src="/imgs/curves.png" align="middle"/>
-</p>
-
-
-
-## Table of Contents
-
-- [Overview](#overview)
-- [Installation](#installation)
-- [Documentation](#documentation)
-- [Contributing](#contributing)
-- [Citation](#citation)
-- [References](#references)
-
-## Overview
-
-(**Version 1.0.0 released in January 2021!**)
-
-There are many implemented methods to perform causal inference when your intervention of interest is binary,
-but few methods exist to handle continuous treatments.
-
-This is unfortunate because there are many scenarios (in industry and research) where these methods would be useful.
-For example, when you would like to:
-
-* Estimate the causal response to increasing or decreasing the price of a product across a wide range.
-* Understand how the number of minutes per week of aerobic exercise causes positive health outcomes.
-* Estimate how decreasing order wait time will impact customer satisfaction, after controlling for confounding effects.
-* Estimate how changing neighborhood income inequality (Gini index) could be causally related to neighborhood crime rate.
-
-This library attempts to address this gap, providing tools to estimate causal curves (AKA causal dose-response curves).
-Both continuous and binary outcomes can be modeled against a continuous treatment.
-
-## Installation
-
-Available via PyPI:
-
-`pip install causal-curve`
-
-You can also get the latest version of causal-curve by cloning the repository::
-
-```
-git clone -b main https://github.com/ronikobrosly/causal-curve.git
-cd causal-curve
-pip install .
-```
-
-## Documentation
-
-[Documentation is available at readthedocs.org](https://causal-curve.readthedocs.io/en/latest/)
-
-
-## Contributing
-
-Your help is absolutely welcome! Please do reach out or create a feature branch!
-
-## Citation
-
-Kobrosly, R. W., (2020). causal-curve: A Python Causal Inference Package to Estimate Causal Dose-Response Curves. Journal of Open Source Software, 5(52), 2523, [https://doi.org/10.21105/joss.02523](https://doi.org/10.21105/joss.02523)
-
-## References
-
-Galagate, D. Causal Inference with a Continuous Treatment and Outcome: Alternative
-Estimators for Parametric Dose-Response function with Applications. PhD thesis, 2016.
-
-Hirano K and Imbens GW. The propensity score with continuous treatments.
-In: Gelman A and Meng XL (eds) Applied bayesian modeling and causal inference
-from incomplete-data perspectives. Oxford, UK: Wiley, 2004, pp.73–84.
-
-Imai K, Keele L, Tingley D. A General Approach to Causal Mediation Analysis. Psychological
-Methods. 15(4), 2010, pp.309–334.
-
-Kennedy EH, Ma Z, McHugh MD, Small DS. Nonparametric methods for doubly robust estimation
-of continuous treatment effects. Journal of the Royal Statistical Society, Series B. 79(4), 2017, pp.1229-1245.
-
-Moodie E and Stephens DA. Estimation of dose–response functions for
-longitudinal data using the generalised propensity score. In: Statistical Methods in
-Medical Research 21(2), 2010, pp.149–166.
-
-van der Laan MJ and Gruber S. Collaborative double robust penalized targeted
-maximum likelihood estimation. In: The International Journal of Biostatistics 6(1), 2010.
-
-van der Laan MJ and Rubin D. Targeted maximum likelihood learning. In: ​U.C. Berkeley Division of
-Biostatistics Working Paper Series, 2006.
+# causal-curve
+
+[![build status](http://img.shields.io/travis/ronikobrosly/causal-curve/main.svg?style=flat)](https://travis-ci.org/ronikobrosly/causal-curve)
+[![codecov](https://codecov.io/gh/ronikobrosly/causal-curve/branch/main/graph/badge.svg)](https://codecov.io/gh/ronikobrosly/causal-curve)
+[![DOI](https://zenodo.org/badge/256017107.svg)](https://zenodo.org/badge/latestdoi/256017107)
+
+Python tools to perform causal inference when the treatment of interest is continuous.
+
+
+<p align="center">
+<img src="/imgs/curves.png" align="middle"/>
+</p>
+
+
+
+## Table of Contents
+
+- [Overview](#overview)
+- [Installation](#installation)
+- [Documentation](#documentation)
+- [Contributing](#contributing)
+- [Citation](#citation)
+- [References](#references)
+
+## Overview
+
+(**Version 1.0.0 released in January 2021!**)
+
+There are many implemented methods to perform causal inference when your intervention of interest is binary,
+but few methods exist to handle continuous treatments.
+
+This is unfortunate because there are many scenarios (in industry and research) where these methods would be useful.
+For example, when you would like to:
+
+* Estimate the causal response to increasing or decreasing the price of a product across a wide range.
+* Understand how the number of minutes per week of aerobic exercise causes positive health outcomes.
+* Estimate how decreasing order wait time will impact customer satisfaction, after controlling for confounding effects.
+* Estimate how changing neighborhood income inequality (Gini index) could be causally related to neighborhood crime rate.
+
+This library attempts to address this gap, providing tools to estimate causal curves (AKA causal dose-response curves).
+Both continuous and binary outcomes can be modeled against a continuous treatment.
+
+## Installation
+
+Available via PyPI:
+
+`pip install causal-curve`
+
+You can also get the latest version of causal-curve by cloning the repository::
+
+```
+git clone -b main https://github.com/ronikobrosly/causal-curve.git
+cd causal-curve
+pip install .
+```
+
+## Documentation
+
+[Documentation, tutorials, and examples are available at readthedocs.org](https://causal-curve.readthedocs.io/en/latest/)
+
+
+## Contributing
+
+Your help is absolutely welcome! Please do reach out or create a feature branch!
+
+## Citation
+
+Kobrosly, R. W., (2020). causal-curve: A Python Causal Inference Package to Estimate Causal Dose-Response Curves. Journal of Open Source Software, 5(52), 2523, [https://doi.org/10.21105/joss.02523](https://doi.org/10.21105/joss.02523)
+
+## References
+
+Galagate, D. Causal Inference with a Continuous Treatment and Outcome: Alternative
+Estimators for Parametric Dose-Response function with Applications. PhD thesis, 2016.
+
+Hirano K and Imbens GW. The propensity score with continuous treatments.
+In: Gelman A and Meng XL (eds) Applied bayesian modeling and causal inference
+from incomplete-data perspectives. Oxford, UK: Wiley, 2004, pp.73–84.
+
+Imai K, Keele L, Tingley D. A General Approach to Causal Mediation Analysis. Psychological
+Methods. 15(4), 2010, pp.309–334.
+
+Kennedy EH, Ma Z, McHugh MD, Small DS. Nonparametric methods for doubly robust estimation
+of continuous treatment effects. Journal of the Royal Statistical Society, Series B. 79(4), 2017, pp.1229-1245.
+
+Moodie E and Stephens DA. Estimation of dose–response functions for
+longitudinal data using the generalised propensity score. In: Statistical Methods in
+Medical Research 21(2), 2010, pp.149–166.
+
+van der Laan MJ and Gruber S. Collaborative double robust penalized targeted
+maximum likelihood estimation. In: The International Journal of Biostatistics 6(1), 2010.
+
+van der Laan MJ and Rubin D. Targeted maximum likelihood learning. In: ​U.C. Berkeley Division of
+Biostatistics Working Paper Series, 2006.
```

### Comparing `causal-curve-1.0.6/causal_curve/core.py` & `causal_curve-1.0.7b0/causal_curve/core.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-"""
-Core classes (with basic methods) that will be invoked when other, model classes are defined
-"""
-
-import numpy as np
-from scipy.stats import norm
-
-
-class Core:
-    """Base class for causal_curve module"""
-
-    def __init__(self):
-        pass
-
-    __version__ = "1.0.6"
-
-    def get_params(self):
-        """Returns a dict of all of the object's user-facing parameters
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        self: object
-        """
-        attrs = self.__dict__
-        return dict(
-            [(k, v) for k, v in list(attrs.items()) if (k[0] != "_") and (k[-1] != "_")]
-        )
-
-    def if_verbose_print(self, string):
-        """Prints the input statement if verbose is set to True
-
-        Parameters
-        ----------
-        string: str, some string to be printed
-
-        Returns
-        ----------
-        None
-
-        """
-        if self.verbose:
-            print(string)
-
-    @staticmethod
-    def rand_seed_wrapper(random_seed=None):
-        """Sets the random seed using numpy
-
-        Parameters
-        ----------
-        random_seed: int, random seed number
-
-        Returns
-        ----------
-        None
-        """
-        if random_seed is None:
-            pass
-        else:
-            np.random.seed(random_seed)
-
-    @staticmethod
-    def calculate_z_score(ci):
-        """Calculates the critical z-score for a desired two-sided,
-        confidence interval width.
-
-        Parameters
-        ----------
-        ci: float, the confidence interval width (e.g. 0.95)
-
-        Returns
-        -------
-        Float, critical z-score value
-        """
-        return norm.ppf((1 + ci) / 2)
-
-    @staticmethod
-    def clip_negatives(number):
-        """Helper function to clip negative numbers to zero
-
-        Parameters
-        ----------
-        number: int or float, any number that needs a floor at zero
-
-        Returns
-        -------
-        Int or float of modified value
-
-        """
-        if number < 0:
-            return 0
-        return number
+"""
+Core classes (with basic methods) that will be invoked when other, model classes are defined
+"""
+
+import numpy as np
+from scipy.stats import norm
+
+
+class Core:
+    """Base class for causal_curve module"""
+
+    def __init__(self):
+        pass
+
+    __version__ = "1.0.6"
+
+    def get_params(self):
+        """Returns a dict of all of the object's user-facing parameters
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self: object
+        """
+        attrs = self.__dict__
+        return dict(
+            [(k, v) for k, v in list(attrs.items()) if (k[0] != "_") and (k[-1] != "_")]
+        )
+
+    def if_verbose_print(self, string):
+        """Prints the input statement if verbose is set to True
+
+        Parameters
+        ----------
+        string: str, some string to be printed
+
+        Returns
+        ----------
+        None
+
+        """
+        if self.verbose:
+            print(string)
+
+    @staticmethod
+    def rand_seed_wrapper(random_seed=None):
+        """Sets the random seed using numpy
+
+        Parameters
+        ----------
+        random_seed: int, random seed number
+
+        Returns
+        ----------
+        None
+        """
+        if random_seed is None:
+            pass
+        else:
+            np.random.seed(random_seed)
+
+    @staticmethod
+    def calculate_z_score(ci):
+        """Calculates the critical z-score for a desired two-sided,
+        confidence interval width.
+
+        Parameters
+        ----------
+        ci: float, the confidence interval width (e.g. 0.95)
+
+        Returns
+        -------
+        Float, critical z-score value
+        """
+        return norm.ppf((1 + ci) / 2)
+
+    @staticmethod
+    def clip_negatives(number):
+        """Helper function to clip negative numbers to zero
+
+        Parameters
+        ----------
+        number: int or float, any number that needs a floor at zero
+
+        Returns
+        -------
+        Int or float of modified value
+
+        """
+        if number < 0:
+            return 0
+        return number
```

### Comparing `causal-curve-1.0.6/causal_curve/gps_classifier.py` & `causal_curve-1.0.7b0/causal_curve/gps_classifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-"""
-Defines the Generalized Prospensity Score (GPS) classifier model class
-"""
-from pprint import pprint
-
-import numpy as np
-from scipy.special import logit
-
-from causal_curve.gps_core import GPS_Core
-
-
-class GPS_Classifier(GPS_Core):
-    """
-    A GPS tool that handles binary outcomes. Inherits the GPS_core
-    base class. See that base class code its docstring for more details.
-
-
-    Methods
-    ----------
-
-    estimate_log_odds: (self, T)
-        Calculates the predicted log odds of the highest integer class. Can
-        only be used when the outcome is binary.
-
-    """
-
-    def __init__(
-        self,
-        gps_family=None,
-        treatment_grid_num=100,
-        lower_grid_constraint=0.01,
-        upper_grid_constraint=0.99,
-        spline_order=3,
-        n_splines=30,
-        lambda_=0.5,
-        max_iter=100,
-        random_seed=None,
-        verbose=False,
-    ):
-
-        self.gps_family = gps_family
-        self.treatment_grid_num = treatment_grid_num
-        self.lower_grid_constraint = lower_grid_constraint
-        self.upper_grid_constraint = upper_grid_constraint
-        self.spline_order = spline_order
-        self.n_splines = n_splines
-        self.lambda_ = lambda_
-        self.max_iter = max_iter
-        self.random_seed = random_seed
-        self.verbose = verbose
-
-        # Validate the params
-        self._validate_init_params()
-        self.rand_seed_wrapper()
-
-        self.if_verbose_print("Using the following params for GPS model:")
-        if self.verbose:
-            pprint(self.get_params(), indent=4)
-
-    def _cdrc_predictions_binary(self, ci):
-        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
-        we're making predictions using the original treatment and gps_at_grid.
-        To be used when the outcome of interest is binary.
-        """
-        # To keep track of cdrc predictions, we create an empty 2d array of shape
-        # (n_samples, treatment_grid_num, 2). The last dimension is of length 2 because
-        # we are going to keep track of the point estimate (log-odds) of the prediction, as well as
-        # the standard error of the prediction interval (again, this is for the log odds)
-        cdrc_preds = np.zeros((len(self.T), self.treatment_grid_num, 2), dtype=float)
-
-        # Loop through each of the grid values, predict point estimate and get prediction interval
-        for i in range(0, self.treatment_grid_num):
-
-            temp_T = np.repeat(self.grid_values[i], repeats=len(self.T))
-            temp_gps = self.gps_at_grid[:, i]
-
-            temp_cdrc_preds = logit(
-                self.gam_results.predict_proba(np.column_stack((temp_T, temp_gps)))
-            )
-
-            temp_cdrc_interval = logit(
-                self.gam_results.confidence_intervals(
-                    np.column_stack((temp_T, temp_gps)), width=ci
-                )
-            )
-
-            standard_error = (
-                temp_cdrc_interval[:, 1] - temp_cdrc_preds
-            ) / self.calculate_z_score(ci)
-
-            cdrc_preds[:, i, 0] = temp_cdrc_preds
-            cdrc_preds[:, i, 1] = standard_error
-
-        return np.round(cdrc_preds, 3)
-
-    def estimate_log_odds(self, T):
-        """Calculates the estimated log odds of the highest integer class. Can
-        only be used when the outcome is binary. Can be estimate for a single
-        data point or can be run in batch for many observations. Extrapolation will produce
-        untrustworthy results; the provided treatment should be within
-        the range of the training data.
-
-        Parameters
-        ----------
-        T: Numpy array, shape (n_samples,)
-            A continuous treatment variable.
-
-        Returns
-        ----------
-        array: Numpy array
-            Contains a set of log odds
-        """
-        if self.outcome_type != "binary":
-            raise TypeError("Your outcome must be binary to use this function!")
-
-        return np.apply_along_axis(self._create_log_odds, 0, T.reshape(1, -1))
-
-    def _create_log_odds(self, T):
-        """Take a single treatment value and produces the log odds of the higher
-        integer class, in the case of a binary outcome.
-        """
-        return logit(
-            self.gam_results.predict_proba(
-                np.array([T, self.gps_function(T).mean()]).reshape(1, -1)
-            )
-        )
+"""
+Defines the Generalized Prospensity Score (GPS) classifier model class
+"""
+from pprint import pprint
+
+import numpy as np
+from scipy.special import logit
+
+from causal_curve.gps_core import GPS_Core
+
+
+class GPS_Classifier(GPS_Core):
+    """
+    A GPS tool that handles binary outcomes. Inherits the GPS_core
+    base class. See that base class code its docstring for more details.
+
+
+    Methods
+    ----------
+
+    estimate_log_odds: (self, T)
+        Calculates the predicted log odds of the highest integer class. Can
+        only be used when the outcome is binary.
+
+    """
+
+    def __init__(
+        self,
+        gps_family=None,
+        treatment_grid_num=100,
+        lower_grid_constraint=0.01,
+        upper_grid_constraint=0.99,
+        spline_order=3,
+        n_splines=30,
+        lambda_=0.5,
+        max_iter=100,
+        random_seed=None,
+        verbose=False,
+    ):
+
+        self.gps_family = gps_family
+        self.treatment_grid_num = treatment_grid_num
+        self.lower_grid_constraint = lower_grid_constraint
+        self.upper_grid_constraint = upper_grid_constraint
+        self.spline_order = spline_order
+        self.n_splines = n_splines
+        self.lambda_ = lambda_
+        self.max_iter = max_iter
+        self.random_seed = random_seed
+        self.verbose = verbose
+
+        # Validate the params
+        self._validate_init_params()
+        self.rand_seed_wrapper()
+
+        self.if_verbose_print("Using the following params for GPS model:")
+        if self.verbose:
+            pprint(self.get_params(), indent=4)
+
+    def _cdrc_predictions_binary(self, ci):
+        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
+        we're making predictions using the original treatment and gps_at_grid.
+        To be used when the outcome of interest is binary.
+        """
+        # To keep track of cdrc predictions, we create an empty 2d array of shape
+        # (n_samples, treatment_grid_num, 2). The last dimension is of length 2 because
+        # we are going to keep track of the point estimate (log-odds) of the prediction, as well as
+        # the standard error of the prediction interval (again, this is for the log odds)
+        cdrc_preds = np.zeros((len(self.T), self.treatment_grid_num, 2), dtype=float)
+
+        # Loop through each of the grid values, predict point estimate and get prediction interval
+        for i in range(0, self.treatment_grid_num):
+
+            temp_T = np.repeat(self.grid_values[i], repeats=len(self.T))
+            temp_gps = self.gps_at_grid[:, i]
+
+            temp_cdrc_preds = logit(
+                self.gam_results.predict_proba(np.column_stack((temp_T, temp_gps)))
+            )
+
+            temp_cdrc_interval = logit(
+                self.gam_results.confidence_intervals(
+                    np.column_stack((temp_T, temp_gps)), width=ci
+                )
+            )
+
+            standard_error = (
+                temp_cdrc_interval[:, 1] - temp_cdrc_preds
+            ) / self.calculate_z_score(ci)
+
+            cdrc_preds[:, i, 0] = temp_cdrc_preds
+            cdrc_preds[:, i, 1] = standard_error
+
+        return np.round(cdrc_preds, 3)
+
+    def estimate_log_odds(self, T):
+        """Calculates the estimated log odds of the highest integer class. Can
+        only be used when the outcome is binary. Can be estimate for a single
+        data point or can be run in batch for many observations. Extrapolation will produce
+        untrustworthy results; the provided treatment should be within
+        the range of the training data.
+
+        Parameters
+        ----------
+        T: Numpy array, shape (n_samples,)
+            A continuous treatment variable.
+
+        Returns
+        ----------
+        array: Numpy array
+            Contains a set of log odds
+        """
+        if self.outcome_type != "binary":
+            raise TypeError("Your outcome must be binary to use this function!")
+
+        return np.apply_along_axis(self._create_log_odds, 0, T.reshape(1, -1))
+
+    def _create_log_odds(self, T):
+        """Take a single treatment value and produces the log odds of the higher
+        integer class, in the case of a binary outcome.
+        """
+        return logit(
+            self.gam_results.predict_proba(
+                np.array([T[0], self.gps_function(T).mean()]).reshape(1, -1)
+            )
+        )
```

### Comparing `causal-curve-1.0.6/causal_curve/gps_core.py` & `causal_curve-1.0.7b0/causal_curve/gps_core.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,731 +1,731 @@
-"""
-Defines the Generalized Prospensity Score (GPS) Core model class
-"""
-
-import contextlib
-import io
-
-import numpy as np
-import pandas as pd
-from pandas.api.types import is_float_dtype, is_integer_dtype, is_numeric_dtype
-from pygam import LinearGAM, LogisticGAM, s
-from scipy.stats import gamma, norm
-import statsmodels.api as sm
-from statsmodels.genmod.families.links import inverse_power as Inverse_Power
-from statsmodels.tools.tools import add_constant
-
-from causal_curve.core import Core
-
-
-class GPS_Core(Core):
-    """
-    In a multi-stage approach, this computes the generalized propensity score (GPS) function,
-    and uses this in a generalized additive model (GAM) to correct treatment prediction of
-    the outcome variable. Assumes continuous treatment, but the outcome variable may be
-    continuous or binary.
-
-    WARNING:
-
-    -This algorithm assumes you've already performed the necessary transformations to
-    categorical covariates (i.e. these variables are already one-hot encoded and
-    one of the categories is excluded for each set of dummy variables).
-
-    -Please take care to ensure that the "ignorability" assumption is met (i.e.
-    all strong confounders are captured in your covariates and there is no
-    informative censoring), otherwise your results will be biased, sometimes strongly so.
-
-    Parameters
-    ----------
-
-    gps_family: str, optional (default = None)
-        Is used to determine the family of the glm used to model the GPS function.
-        Look at the distribution of your treatment variable to determine which
-        family is more appropriate.
-        Possible values:
-
-        - 'normal'
-        - 'lognormal'
-        - 'gamma'
-        - None : (best-fitting family automatically chosen)
-
-    treatment_grid_num: int, optional (default = 100)
-        Takes the treatment, and creates a quantile-based grid across its values.
-        For instance, if the number 6 is selected, this means the algorithm will only take
-        the 6 treatment variable values at approximately the 0, 20, 40, 60, 80, and 100th
-        percentiles to estimate the causal dose response curve.
-        Higher value here means the final curve will be more finely estimated,
-        but also increases computation time. Default is usually a reasonable number.
-
-    lower_grid_constraint:  float, optional(default = 0.01)
-        This adds an optional constraint of the lower side of the treatment grid.
-        Sometimes data near the minimum values of the treatment are few in number
-        and thus generate unstable estimates. By default, this clips the bottom 1 percentile
-        or lower of treatment values. This can be as low as 0, indicating there is no
-        lower limit to how much treatment data is considered.
-
-    upper_grid_constraint: float, optional (default = 0.99)
-        See above parameter. Just like above, but this is an upper constraint.
-        By default, this clips the top 99th percentile or higher of treatment values.
-        This can be as high as 1.0, indicating there is no upper limit to how much
-        treatment data is considered.
-
-    spline_order: int, optional (default = 3)
-        Order of the splines to use fitting the final GAM.
-        Must be integer >= 1. Default value creates cubic splines.
-
-    n_splines: int, optional (default = 30)
-        Number of splines to use for the treatment and GPS in the final GAM.
-        Must be integer >= 2. Must be non-negative.
-
-    lambda_: int or float, optional (default = 0.5)
-        Strength of smoothing penalty. Must be a positive float.
-        Larger values enforce stronger smoothing.
-
-    max_iter: int, optional (default = 100)
-        Maximum number of iterations allowed for the maximum likelihood algo to converge.
-
-    random_seed: int, optional (default = None)
-        Sets the random seed.
-
-    verbose: bool, optional (default = False)
-        Determines whether the user will get verbose status updates.
-
-
-    Attributes
-    ----------
-
-    grid_values: array of shape (treatment_grid_num, )
-        The gridded values of the treatment variable. Equally spaced.
-
-    best_gps_family: str
-        If no gps_family is specified and the algorithm chooses the best glm family, this is
-        the name of the family that was chosen.
-
-    gps_deviance: float
-        The GPS model deviance
-
-    gps: array of shape (number of observations, )
-        The calculated GPS for each observation
-
-    gam_results: `pygam.LinearGAM` class
-        trained model of `LinearGAM` class, from pyGAM library
-
-
-    Methods
-    ----------
-    fit: (self, T, X, y)
-        Fits the causal dose-response model.
-
-    calculate_CDRC: (self, ci)
-        Calculates the CDRC (and confidence interval) from trained model.
-
-    print_gam_summary: (self)
-        Prints pyGAM text summary of GAM predicting outcome from the treatment and the GPS.
-
-
-    Examples
-    --------
-
-    >>> # With continuous outcome
-    >>> from causal_curve import GPS_Regressor
-    >>> gps = GPS_Regressor(treatment_grid_num = 200, random_seed = 512)
-    >>> gps.fit(T = df['Treatment'], X = df[['X_1', 'X_2']], y = df['Outcome'])
-    >>> gps_results = gps.calculate_CDRC(0.95)
-    >>> point_estimate = gps.point_estimate(np.array([5.0]))
-    >>> point_estimate_interval = gps.point_estimate_interval(np.array([5.0]), 0.95)
-
-
-    >>> # With binary outcome
-    >>> from causal_curve import GPS_Classifier
-    >>> gps = GPS_Classifier()
-    >>> gps.fit(T = df['Treatment'], X = df[['X_1', 'X_2']], y = df['Binary_Outcome'])
-    >>> gps_results = gps.calculate_CDRC(0.95)
-    >>> log_odds = gps.estimate_log_odds(np.array([5.0]))
-
-
-    References
-    ----------
-
-    Galagate, D. Causal Inference with a Continuous Treatment and Outcome: Alternative
-    Estimators for Parametric Dose-Response function with Applications. PhD thesis, 2016.
-
-    Moodie E and Stephens DA. Estimation of dose–response functions for
-    longitudinal data using the generalised propensity score. In: Statistical Methods in
-    Medical Research 21(2), 2010, pp.149–166.
-
-    Hirano K and Imbens GW. The propensity score with continuous treatments.
-    In: Gelman A and Meng XL (eds) Applied bayesian modeling and causal inference
-    from incomplete-data perspectives. Oxford, UK: Wiley, 2004, pp.73–84.
-    """
-
-    def __init__(
-        self,
-        gps_family=None,
-        treatment_grid_num=100,
-        lower_grid_constraint=0.01,
-        upper_grid_constraint=0.99,
-        spline_order=3,
-        n_splines=30,
-        lambda_=0.5,
-        max_iter=100,
-        random_seed=None,
-        verbose=False,
-    ):
-
-        self.gps_family = gps_family
-        self.treatment_grid_num = treatment_grid_num
-        self.lower_grid_constraint = lower_grid_constraint
-        self.upper_grid_constraint = upper_grid_constraint
-        self.spline_order = spline_order
-        self.n_splines = n_splines
-        self.lambda_ = lambda_
-        self.max_iter = max_iter
-        self.random_seed = random_seed
-        self.verbose = verbose
-
-    def _validate_init_params(self):
-        """
-        Checks that the params used when instantiating GPS model are formatted correctly
-        """
-        # Checks for gps_family param
-        if not isinstance(self.gps_family, (str, type(None))):
-            raise TypeError(
-                f"gps_family parameter must be a string or None "
-                f"but found type {type(self.gps_family)}"
-            )
-
-        if (isinstance(self.gps_family, str)) and (
-            self.gps_family not in ["normal", "lognormal", "gamma"]
-        ):
-            raise ValueError(
-                f"gps_family parameter must take on values of "
-                f"'normal', 'lognormal', or 'gamma', but found {self.gps_family}"
-            )
-
-        # Checks for treatment_grid_num
-        if not isinstance(self.treatment_grid_num, int):
-            raise TypeError(
-                f"treatment_grid_num parameter must be an integer, "
-                f"but found type {type(self.treatment_grid_num)}"
-            )
-
-        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num < 10:
-            raise ValueError(
-                f"treatment_grid_num parameter should be >= 10 so your final curve "
-                f"has enough resolution, but found value {self.treatment_grid_num}"
-            )
-
-        if (
-            isinstance(self.treatment_grid_num, int)
-        ) and self.treatment_grid_num >= 1000:
-            raise ValueError("treatment_grid_num parameter is too high!")
-
-        # Checks for lower_grid_constraint
-        if not isinstance(self.lower_grid_constraint, float):
-            raise TypeError(
-                f"lower_grid_constraint parameter must be a float, "
-                f"but found type {type(self.lower_grid_constraint)}"
-            )
-
-        if (
-            isinstance(self.lower_grid_constraint, float)
-        ) and self.lower_grid_constraint < 0:
-            raise ValueError(
-                f"lower_grid_constraint parameter cannot be < 0, "
-                f"but found value {self.lower_grid_constraint}"
-            )
-
-        if (
-            isinstance(self.lower_grid_constraint, float)
-        ) and self.lower_grid_constraint >= 1.0:
-            raise ValueError(
-                f"lower_grid_constraint parameter cannot >= 1.0, "
-                f"but found value {self.lower_grid_constraint}"
-            )
-
-        # Checks for upper_grid_constraint
-        if not isinstance(self.upper_grid_constraint, float):
-            raise TypeError(
-                f"upper_grid_constraint parameter must be a float, "
-                f"but found type {type(self.upper_grid_constraint)}"
-            )
-
-        if (
-            isinstance(self.upper_grid_constraint, float)
-        ) and self.upper_grid_constraint <= 0:
-            raise ValueError(
-                f"upper_grid_constraint parameter cannot be <= 0, "
-                f"but found value {self.upper_grid_constraint}"
-            )
-
-        if (
-            isinstance(self.upper_grid_constraint, float)
-        ) and self.upper_grid_constraint > 1.0:
-            raise ValueError(
-                f"upper_grid_constraint parameter cannot > 1.0, "
-                f"but found value {self.upper_grid_constraint}"
-            )
-
-        # Checks for lower_grid_constraint isn't higher than upper_grid_constraint
-        if self.lower_grid_constraint >= self.upper_grid_constraint:
-            raise ValueError(
-                "lower_grid_constraint should be lower than upper_grid_constraint!"
-            )
-
-        # Checks for spline_order
-        if not isinstance(self.spline_order, int):
-            raise TypeError(
-                f"spline_order parameter must be an integer, "
-                f"but found type {type(self.spline_order)}"
-            )
-
-        if (isinstance(self.spline_order, int)) and self.spline_order < 1:
-            raise ValueError(
-                f"spline_order parameter should be >= 1, but found {self.spline_order}"
-            )
-
-        if (isinstance(self.spline_order, int)) and self.spline_order >= 30:
-            raise ValueError("spline_order parameter is too high!")
-
-        # Checks for n_splines
-        if not isinstance(self.n_splines, int):
-            raise TypeError(
-                f"n_splines parameter must be an integer, but found type {type(self.n_splines)}"
-            )
-
-        if (isinstance(self.n_splines, int)) and self.n_splines < 2:
-            raise ValueError(
-                f"n_splines parameter should be >= 2, but found {self.n_splines}"
-            )
-
-        if (isinstance(self.n_splines, int)) and self.n_splines >= 100:
-            raise ValueError("n_splines parameter is too high!")
-
-        # Checks for lambda_
-        if not isinstance(self.lambda_, (int, float)):
-            raise TypeError(
-                f"lambda_ parameter must be an int or float, but found type {type(self.lambda_)}"
-            )
-
-        if (isinstance(self.lambda_, (int, float))) and self.lambda_ <= 0:
-            raise ValueError(
-                f"lambda_ parameter should be > 0, but found {self.lambda_}"
-            )
-
-        if (isinstance(self.lambda_, (int, float))) and self.lambda_ >= 1000:
-            raise ValueError("lambda_ parameter is too high!")
-
-        # Checks for max_iter
-        if not isinstance(self.max_iter, int):
-            raise TypeError(
-                f"max_iter parameter must be an int, but found type {type(self.max_iter)}"
-            )
-
-        if (isinstance(self.max_iter, int)) and self.max_iter <= 10:
-            raise ValueError(
-                "max_iter parameter is too low! Results won't be reliable!"
-            )
-
-        if (isinstance(self.max_iter, int)) and self.max_iter >= 1e6:
-            raise ValueError("max_iter parameter is unnecessarily high!")
-
-        # Checks for random_seed
-        if not isinstance(self.random_seed, (int, type(None))):
-            raise TypeError(
-                f"random_seed parameter must be an int, but found type {type(self.random_seed)}"
-            )
-
-        if (isinstance(self.random_seed, int)) and self.random_seed < 0:
-            raise ValueError("random_seed parameter must be > 0")
-
-        # Checks for verbose
-        if not isinstance(self.verbose, bool):
-            raise TypeError(
-                f"verbose parameter must be a boolean type, but found type {type(self.verbose)}"
-            )
-
-    def _validate_fit_data(self):
-        """Verifies that T, X, and y are formatted the right way"""
-        # Checks for T column
-        if not is_float_dtype(self.T):
-            raise TypeError("Treatment data must be of type float")
-
-        # Make sure all X columns are float or int
-        if isinstance(self.X, pd.Series):
-            if not is_numeric_dtype(self.X):
-                raise TypeError(
-                    "All covariate (X) columns must be int or float type (i.e. must be numeric)"
-                )
-
-        elif isinstance(self.X, pd.DataFrame):
-            for column in self.X:
-                if not is_numeric_dtype(self.X[column]):
-                    raise TypeError(
-                        "All covariate (X) columns must be int or float type "
-                        "(i.e. must be numeric)"
-                    )
-
-        # Checks for Y column
-        if not (is_float_dtype(self.y) or is_integer_dtype(self.y)):
-            raise TypeError("Outcome data must be of type float or integer")
-
-        if is_integer_dtype(self.y) and (
-            not np.array_equal(np.sort(self.y.unique()), np.array([0, 1]))
-        ):
-            raise TypeError(
-                "If your outcome data is of type integer (binary outcome),"
-                "it should only contain 1's and 0's."
-            )
-
-    def _grid_values(self):
-        """Produces initial grid values for the treatment variable"""
-        return np.quantile(
-            self.T,
-            q=np.linspace(
-                start=self.lower_grid_constraint,
-                stop=self.upper_grid_constraint,
-                num=self.treatment_grid_num,
-            ),
-        )
-
-    def fit(self, T, X, y):
-        """Fits the GPS causal dose-response model. For now, this only accepts pandas columns.
-        While the treatment variable must be continuous (or ordinal with many levels), the
-        outcome variable may be continuous or binary. You *must* provide
-        at least one covariate column.
-
-        Parameters
-        ----------
-        T: array-like, shape (n_samples,)
-            A continuous treatment variable.
-        X: array-like, shape (n_samples, m_features)
-            Covariates, where n_samples is the number of samples
-            and m_features is the number of features. Features can be a mix of continuous
-            and nominal/categorical variables.
-        y: array-like, shape (n_samples,)
-            Outcome variable. May be continuous or binary. If continuous, this must
-            be a series of type `float`, if binary must be a series of type `integer`.
-
-        Returns
-        ----------
-        self : object
-
-        """
-        self.rand_seed_wrapper(self.random_seed)
-
-        self.T = T.reset_index(drop=True, inplace=False)
-        self.X = X.reset_index(drop=True, inplace=False)
-        self.y = y.reset_index(drop=True, inplace=False)
-
-        # Determine what type of outcome variable we're working with
-        if is_float_dtype(self.y):
-            self.outcome_type = "continuous"
-        elif is_integer_dtype(self.y):
-            self.outcome_type = "binary"
-
-        self.if_verbose_print(
-            f"Determined the outcome variable is of type {self.outcome_type}..."
-        )
-
-        # Validate this input data
-        self._validate_fit_data()
-
-        # Create grid_values
-        self.grid_values = self._grid_values()
-
-        # Determine which GPS family to use
-        self._determine_gps_function()
-
-        # Estimate the GPS
-        self.if_verbose_print("Saving GPS values...")
-
-        self.gps = self.gps_function(self.T)
-
-        # Create GAM that predicts outcome from the treatment and GPS
-        self.if_verbose_print("Fitting GAM using treatment and GPS...")
-
-        # Save model results
-        self.gam_results = self._fit_gam()
-
-        f = io.StringIO()
-        with contextlib.redirect_stdout(f):
-            self.gam_results.summary()
-
-        self._gam_summary_str = f.getvalue()
-
-        self.if_verbose_print(
-            "Calculating many CDRC estimates for each treatment grid value..."
-        )
-
-        # Loop over all grid values (`treatment_grid_num` in total)
-        # and give GPS loading for each observation in the dataset
-        self.gps_at_grid = self._gps_values_at_grid()
-
-    def calculate_CDRC(self, ci=0.95):
-        """Using the results of the fitted model, this generates a dataframe of
-        point estimates for the CDRC at each of the values of the
-        treatment grid. Connecting these estimates will produce the overall
-        estimated CDRC. Confidence interval is returned as well.
-
-        Parameters
-        ----------
-        ci: float (default = 0.95)
-            The desired confidence interval to produce. Default value is 0.95, corresponding
-            to 95% confidence intervals. bounded (0, 1.0).
-
-        Returns
-        ----------
-        dataframe: Pandas dataframe
-            Contains treatment grid values, the CDRC point estimate at that value,
-            and the associated lower and upper confidence interval bounds at that point.
-
-        self: object
-
-        """
-        self.rand_seed_wrapper(self.random_seed)
-        self._validate_calculate_CDRC_params(ci)
-
-        self.if_verbose_print(
-            """
-            Generating predictions for each value of treatment grid,
-            and averaging to get the CDRC..."""
-        )
-
-        # Create CDRC predictions from trained GAM
-        # If working with a continuous outcome variable, use this path
-        if self.outcome_type == "continuous":
-            self._cdrc_preds = self._cdrc_predictions_continuous(ci)
-
-            results = []
-
-            for i in range(0, self.treatment_grid_num):
-                temp_grid_value = self.grid_values[i]
-                temp_point_estimate = self._cdrc_preds[:, i, 0].mean()
-                mean_ci_width = (
-                    self._cdrc_preds[:, i, 2].mean() - self._cdrc_preds[:, i, 1].mean()
-                ) / 2
-                temp_lower_bound = temp_point_estimate - mean_ci_width
-                temp_upper_bound = temp_point_estimate + mean_ci_width
-                results.append(
-                    [
-                        temp_grid_value,
-                        temp_point_estimate,
-                        temp_lower_bound,
-                        temp_upper_bound,
-                    ]
-                )
-
-            outcome_name = "Causal_Dose_Response"
-
-        # If working with a binary outcome variable, use this path
-        else:
-            self._cdrc_preds = self._cdrc_predictions_binary(ci)
-
-            # Capture the first prediction's mean log odds.
-            # This will serve as a reference for calculating the odds ratios
-            log_odds_reference = self._cdrc_preds[:, 0, 0].mean()
-
-            results = []
-
-            for i in range(0, self.treatment_grid_num):
-                temp_grid_value = self.grid_values[i]
-
-                temp_log_odds_estimate = (
-                    self._cdrc_preds[:, i, 0].mean() - log_odds_reference
-                )
-                temp_OR_estimate = np.exp(temp_log_odds_estimate)
-
-                temp_lower_bound = np.exp(
-                    temp_log_odds_estimate
-                    - (self.calculate_z_score(ci) * self._cdrc_preds[:, i, 1].mean())
-                )
-                temp_upper_bound = np.exp(
-                    temp_log_odds_estimate
-                    + (self.calculate_z_score(ci) * self._cdrc_preds[:, i, 1].mean())
-                )
-                results.append(
-                    [
-                        temp_grid_value,
-                        temp_OR_estimate,
-                        temp_lower_bound,
-                        temp_upper_bound,
-                    ]
-                )
-
-            outcome_name = "Causal_Odds_Ratio"
-
-        return pd.DataFrame(
-            results, columns=["Treatment", outcome_name, "Lower_CI", "Upper_CI"]
-        ).round(3)
-
-    @staticmethod
-    def _validate_calculate_CDRC_params(ci):
-        """Validates the parameters given to `calculate_CDRC`"""
-
-        if not isinstance(ci, float):
-            raise TypeError(
-                f"`ci` parameter must be an float, but found type {type(ci)}"
-            )
-
-        if isinstance(ci, float) and ((ci <= 0) or (ci >= 1.0)):
-            raise ValueError("`ci` parameter should be between (0, 1)")
-
-    def _gps_values_at_grid(self):
-        """Returns an array where we get the GPS-derived values for each element
-        of the treatment grid. Resulting array will be of shape (n_samples, treatment_grid_num)
-        """
-        # Creates an empty 2d array of shape (n_samples, treatment_grid_num)
-        gps_at_grid = np.zeros((len(self.T), self.treatment_grid_num), dtype=float)
-
-        # Loop over all grid values
-        for i in range(0, self.treatment_grid_num):
-            gps_at_grid[:, i] = self.gps_function(self.grid_values[i])
-
-        return gps_at_grid
-
-    def print_gam_summary(self):
-        """Prints the GAM model summary (uses pyGAM's output)
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        ----------
-        self: object
-        """
-        print(self._gam_summary_str)
-
-    def _fit_gam(self):
-        """Fits a GAM that predicts the outcome (continuous or binary) from the treatment and GPS"""
-
-        X = np.column_stack((self.T.values, self.gps))
-        y = np.asarray(self.y)
-
-        model_type_dict = {"continuous": LinearGAM, "binary": LogisticGAM}
-
-        return model_type_dict[self.outcome_type](
-            s(0, n_splines=self.n_splines, spline_order=self.spline_order)
-            + s(1, n_splines=self.n_splines, spline_order=self.spline_order),
-            max_iter=self.max_iter,
-            lam=self.lambda_,
-        ).fit(X, y)
-
-    def _determine_gps_function(self):
-        """Based on the user input, distribution of treatment values, and/or model deviances,
-        this function determines which GPS function family should be used.
-        """
-
-        # If any negative values in treatment, you must use the normal GLM family.
-        if any(self.T <= 0):
-            self.best_gps_family = "normal"
-            self.gps_function, self.gps_deviance = self._create_normal_gps_function()
-            self.if_verbose_print(
-                """Must fit `normal` GLM family to model treatment since
-                treatment takes on zero or negative values..."""
-            )
-
-        # If treatment has no negative values and user provides in put, use that.
-        elif (all(self.T > 0)) & (not isinstance(self.gps_family, type(None))):
-            self.if_verbose_print(f"Fitting GPS model of family '{self.gps_family}'...")
-
-            if self.gps_family == "normal":
-                self.best_gps_family = "normal"
-                (
-                    self.gps_function,
-                    self.gps_deviance,
-                ) = self._create_normal_gps_function()
-            elif self.gps_family == "lognormal":
-                self.best_gps_family = "lognormal"
-                (
-                    self.gps_function,
-                    self.gps_deviance,
-                ) = self._create_lognormal_gps_function()
-            elif self.gps_family == "gamma":
-                self.best_gps_family = "gamma"
-                self.gps_function, self.gps_deviance = self._create_gamma_gps_function()
-
-        # If no zero or negative treatment values and user didn't provide
-        # input, figure out best-fitting family
-        elif (all(self.T > 0)) & (isinstance(self.gps_family, type(None))):
-            self.if_verbose_print(
-                "Fitting several GPS models and" " picking the best fitting one..."
-            )
-
-            (
-                self.best_gps_family,
-                self.gps_function,
-                self.gps_deviance,
-            ) = self._find_best_gps_model()
-
-            self.if_verbose_print(
-                f"""Best fitting model was {self.best_gps_family}, which
-                    produced a deviance of {self.gps_deviance}"""
-            )
-
-    def _create_normal_gps_function(self):
-        """Models the GPS using a GLM of the Gaussian family"""
-        normal_gps_model = sm.GLM(
-            self.T, add_constant(self.X), family=sm.families.Gaussian()
-        ).fit()
-
-        pred_treat = normal_gps_model.fittedvalues
-        sigma = np.std(normal_gps_model.resid_response)
-
-        def gps_function(treatment_val, pred_treat=pred_treat, sigma=sigma):
-            return norm.pdf(treatment_val, pred_treat, sigma)
-
-        return gps_function, normal_gps_model.deviance
-
-    def _create_lognormal_gps_function(self):
-        """Models the GPS using a GLM of the Gaussian family (assumes treatment is lognormal)"""
-        lognormal_gps_model = sm.GLM(
-            np.log(self.T), add_constant(self.X), family=sm.families.Gaussian()
-        ).fit()
-
-        pred_log_treat = lognormal_gps_model.fittedvalues
-        sigma = np.std(lognormal_gps_model.resid_response)
-
-        def gps_function(treatment_val, pred_log_treat=pred_log_treat, sigma=sigma):
-            return norm.pdf(np.log(treatment_val), pred_log_treat, sigma)
-
-        return gps_function, lognormal_gps_model.deviance
-
-    def _create_gamma_gps_function(self):
-        """Models the GPS using a GLM of the Gamma family"""
-        gamma_gps_model = sm.GLM(
-            self.T, add_constant(self.X), family=sm.families.Gamma(Inverse_Power())
-        ).fit()
-
-        mu = gamma_gps_model.mu
-        scale = gamma_gps_model.scale
-        shape = mu / gamma_gps_model.scale
-
-        def gps_function(treatment_val):
-            return gamma.pdf(treatment_val, a=shape, loc=0, scale=scale)
-
-        return gps_function, gamma_gps_model.deviance
-
-    def _find_best_gps_model(self):
-        """If user doesn't provide a GLM family for modeling the GPS, this function compares
-        a few different gps models and picks the one with the lowest deviance
-        """
-        models_to_try_dict = {
-            "normal_gps_model": self._create_normal_gps_function(),
-            "lognormal_gps_model": self._create_lognormal_gps_function(),
-            "gamma_gps_model": self._create_gamma_gps_function(),
-        }
-
-        model_comparison_dict = {}
-
-        for key, value in models_to_try_dict.items():
-            model_comparison_dict[key] = value[1]
-
-        # Return model with lowest deviance
-        best_model = min(model_comparison_dict, key=model_comparison_dict.get)
-
-        return (
-            best_model,
-            models_to_try_dict[best_model][0],
-            models_to_try_dict[best_model][1],
-        )
+"""
+Defines the Generalized Prospensity Score (GPS) Core model class
+"""
+
+import contextlib
+import io
+
+import numpy as np
+import pandas as pd
+from pandas.api.types import is_float_dtype, is_integer_dtype, is_numeric_dtype
+from pygam import LinearGAM, LogisticGAM, s
+from scipy.stats import gamma, norm
+import statsmodels.api as sm
+from statsmodels.genmod.families.links import inverse_power as Inverse_Power
+from statsmodels.tools.tools import add_constant
+
+from causal_curve.core import Core
+
+
+class GPS_Core(Core):
+    """
+    In a multi-stage approach, this computes the generalized propensity score (GPS) function,
+    and uses this in a generalized additive model (GAM) to correct treatment prediction of
+    the outcome variable. Assumes continuous treatment, but the outcome variable may be
+    continuous or binary.
+
+    WARNING:
+
+    -This algorithm assumes you've already performed the necessary transformations to
+    categorical covariates (i.e. these variables are already one-hot encoded and
+    one of the categories is excluded for each set of dummy variables).
+
+    -Please take care to ensure that the "ignorability" assumption is met (i.e.
+    all strong confounders are captured in your covariates and there is no
+    informative censoring), otherwise your results will be biased, sometimes strongly so.
+
+    Parameters
+    ----------
+
+    gps_family: str, optional (default = None)
+        Is used to determine the family of the glm used to model the GPS function.
+        Look at the distribution of your treatment variable to determine which
+        family is more appropriate.
+        Possible values:
+
+        - 'normal'
+        - 'lognormal'
+        - 'gamma'
+        - None : (best-fitting family automatically chosen)
+
+    treatment_grid_num: int, optional (default = 100)
+        Takes the treatment, and creates a quantile-based grid across its values.
+        For instance, if the number 6 is selected, this means the algorithm will only take
+        the 6 treatment variable values at approximately the 0, 20, 40, 60, 80, and 100th
+        percentiles to estimate the causal dose response curve.
+        Higher value here means the final curve will be more finely estimated,
+        but also increases computation time. Default is usually a reasonable number.
+
+    lower_grid_constraint:  float, optional(default = 0.01)
+        This adds an optional constraint of the lower side of the treatment grid.
+        Sometimes data near the minimum values of the treatment are few in number
+        and thus generate unstable estimates. By default, this clips the bottom 1 percentile
+        or lower of treatment values. This can be as low as 0, indicating there is no
+        lower limit to how much treatment data is considered.
+
+    upper_grid_constraint: float, optional (default = 0.99)
+        See above parameter. Just like above, but this is an upper constraint.
+        By default, this clips the top 99th percentile or higher of treatment values.
+        This can be as high as 1.0, indicating there is no upper limit to how much
+        treatment data is considered.
+
+    spline_order: int, optional (default = 3)
+        Order of the splines to use fitting the final GAM.
+        Must be integer >= 1. Default value creates cubic splines.
+
+    n_splines: int, optional (default = 30)
+        Number of splines to use for the treatment and GPS in the final GAM.
+        Must be integer >= 2. Must be non-negative.
+
+    lambda_: int or float, optional (default = 0.5)
+        Strength of smoothing penalty. Must be a positive float.
+        Larger values enforce stronger smoothing.
+
+    max_iter: int, optional (default = 100)
+        Maximum number of iterations allowed for the maximum likelihood algo to converge.
+
+    random_seed: int, optional (default = None)
+        Sets the random seed.
+
+    verbose: bool, optional (default = False)
+        Determines whether the user will get verbose status updates.
+
+
+    Attributes
+    ----------
+
+    grid_values: array of shape (treatment_grid_num, )
+        The gridded values of the treatment variable. Equally spaced.
+
+    best_gps_family: str
+        If no gps_family is specified and the algorithm chooses the best glm family, this is
+        the name of the family that was chosen.
+
+    gps_deviance: float
+        The GPS model deviance
+
+    gps: array of shape (number of observations, )
+        The calculated GPS for each observation
+
+    gam_results: `pygam.LinearGAM` class
+        trained model of `LinearGAM` class, from pyGAM library
+
+
+    Methods
+    ----------
+    fit: (self, T, X, y)
+        Fits the causal dose-response model.
+
+    calculate_CDRC: (self, ci)
+        Calculates the CDRC (and confidence interval) from trained model.
+
+    print_gam_summary: (self)
+        Prints pyGAM text summary of GAM predicting outcome from the treatment and the GPS.
+
+
+    Examples
+    --------
+
+    >>> # With continuous outcome
+    >>> from causal_curve import GPS_Regressor
+    >>> gps = GPS_Regressor(treatment_grid_num = 200, random_seed = 512)
+    >>> gps.fit(T = df['Treatment'], X = df[['X_1', 'X_2']], y = df['Outcome'])
+    >>> gps_results = gps.calculate_CDRC(0.95)
+    >>> point_estimate = gps.point_estimate(np.array([5.0]))
+    >>> point_estimate_interval = gps.point_estimate_interval(np.array([5.0]), 0.95)
+
+
+    >>> # With binary outcome
+    >>> from causal_curve import GPS_Classifier
+    >>> gps = GPS_Classifier()
+    >>> gps.fit(T = df['Treatment'], X = df[['X_1', 'X_2']], y = df['Binary_Outcome'])
+    >>> gps_results = gps.calculate_CDRC(0.95)
+    >>> log_odds = gps.estimate_log_odds(np.array([5.0]))
+
+
+    References
+    ----------
+
+    Galagate, D. Causal Inference with a Continuous Treatment and Outcome: Alternative
+    Estimators for Parametric Dose-Response function with Applications. PhD thesis, 2016.
+
+    Moodie E and Stephens DA. Estimation of dose–response functions for
+    longitudinal data using the generalised propensity score. In: Statistical Methods in
+    Medical Research 21(2), 2010, pp.149–166.
+
+    Hirano K and Imbens GW. The propensity score with continuous treatments.
+    In: Gelman A and Meng XL (eds) Applied bayesian modeling and causal inference
+    from incomplete-data perspectives. Oxford, UK: Wiley, 2004, pp.73–84.
+    """
+
+    def __init__(
+        self,
+        gps_family=None,
+        treatment_grid_num=100,
+        lower_grid_constraint=0.01,
+        upper_grid_constraint=0.99,
+        spline_order=3,
+        n_splines=30,
+        lambda_=0.5,
+        max_iter=100,
+        random_seed=None,
+        verbose=False,
+    ):
+
+        self.gps_family = gps_family
+        self.treatment_grid_num = treatment_grid_num
+        self.lower_grid_constraint = lower_grid_constraint
+        self.upper_grid_constraint = upper_grid_constraint
+        self.spline_order = spline_order
+        self.n_splines = n_splines
+        self.lambda_ = lambda_
+        self.max_iter = max_iter
+        self.random_seed = random_seed
+        self.verbose = verbose
+
+    def _validate_init_params(self):
+        """
+        Checks that the params used when instantiating GPS model are formatted correctly
+        """
+        # Checks for gps_family param
+        if not isinstance(self.gps_family, (str, type(None))):
+            raise TypeError(
+                f"gps_family parameter must be a string or None "
+                f"but found type {type(self.gps_family)}"
+            )
+
+        if (isinstance(self.gps_family, str)) and (
+            self.gps_family not in ["normal", "lognormal", "gamma"]
+        ):
+            raise ValueError(
+                f"gps_family parameter must take on values of "
+                f"'normal', 'lognormal', or 'gamma', but found {self.gps_family}"
+            )
+
+        # Checks for treatment_grid_num
+        if not isinstance(self.treatment_grid_num, int):
+            raise TypeError(
+                f"treatment_grid_num parameter must be an integer, "
+                f"but found type {type(self.treatment_grid_num)}"
+            )
+
+        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num < 10:
+            raise ValueError(
+                f"treatment_grid_num parameter should be >= 10 so your final curve "
+                f"has enough resolution, but found value {self.treatment_grid_num}"
+            )
+
+        if (
+            isinstance(self.treatment_grid_num, int)
+        ) and self.treatment_grid_num >= 1000:
+            raise ValueError("treatment_grid_num parameter is too high!")
+
+        # Checks for lower_grid_constraint
+        if not isinstance(self.lower_grid_constraint, float):
+            raise TypeError(
+                f"lower_grid_constraint parameter must be a float, "
+                f"but found type {type(self.lower_grid_constraint)}"
+            )
+
+        if (
+            isinstance(self.lower_grid_constraint, float)
+        ) and self.lower_grid_constraint < 0:
+            raise ValueError(
+                f"lower_grid_constraint parameter cannot be < 0, "
+                f"but found value {self.lower_grid_constraint}"
+            )
+
+        if (
+            isinstance(self.lower_grid_constraint, float)
+        ) and self.lower_grid_constraint >= 1.0:
+            raise ValueError(
+                f"lower_grid_constraint parameter cannot >= 1.0, "
+                f"but found value {self.lower_grid_constraint}"
+            )
+
+        # Checks for upper_grid_constraint
+        if not isinstance(self.upper_grid_constraint, float):
+            raise TypeError(
+                f"upper_grid_constraint parameter must be a float, "
+                f"but found type {type(self.upper_grid_constraint)}"
+            )
+
+        if (
+            isinstance(self.upper_grid_constraint, float)
+        ) and self.upper_grid_constraint <= 0:
+            raise ValueError(
+                f"upper_grid_constraint parameter cannot be <= 0, "
+                f"but found value {self.upper_grid_constraint}"
+            )
+
+        if (
+            isinstance(self.upper_grid_constraint, float)
+        ) and self.upper_grid_constraint > 1.0:
+            raise ValueError(
+                f"upper_grid_constraint parameter cannot > 1.0, "
+                f"but found value {self.upper_grid_constraint}"
+            )
+
+        # Checks for lower_grid_constraint isn't higher than upper_grid_constraint
+        if self.lower_grid_constraint >= self.upper_grid_constraint:
+            raise ValueError(
+                "lower_grid_constraint should be lower than upper_grid_constraint!"
+            )
+
+        # Checks for spline_order
+        if not isinstance(self.spline_order, int):
+            raise TypeError(
+                f"spline_order parameter must be an integer, "
+                f"but found type {type(self.spline_order)}"
+            )
+
+        if (isinstance(self.spline_order, int)) and self.spline_order < 1:
+            raise ValueError(
+                f"spline_order parameter should be >= 1, but found {self.spline_order}"
+            )
+
+        if (isinstance(self.spline_order, int)) and self.spline_order >= 30:
+            raise ValueError("spline_order parameter is too high!")
+
+        # Checks for n_splines
+        if not isinstance(self.n_splines, int):
+            raise TypeError(
+                f"n_splines parameter must be an integer, but found type {type(self.n_splines)}"
+            )
+
+        if (isinstance(self.n_splines, int)) and self.n_splines < 2:
+            raise ValueError(
+                f"n_splines parameter should be >= 2, but found {self.n_splines}"
+            )
+
+        if (isinstance(self.n_splines, int)) and self.n_splines >= 100:
+            raise ValueError("n_splines parameter is too high!")
+
+        # Checks for lambda_
+        if not isinstance(self.lambda_, (int, float)):
+            raise TypeError(
+                f"lambda_ parameter must be an int or float, but found type {type(self.lambda_)}"
+            )
+
+        if (isinstance(self.lambda_, (int, float))) and self.lambda_ <= 0:
+            raise ValueError(
+                f"lambda_ parameter should be > 0, but found {self.lambda_}"
+            )
+
+        if (isinstance(self.lambda_, (int, float))) and self.lambda_ >= 1000:
+            raise ValueError("lambda_ parameter is too high!")
+
+        # Checks for max_iter
+        if not isinstance(self.max_iter, int):
+            raise TypeError(
+                f"max_iter parameter must be an int, but found type {type(self.max_iter)}"
+            )
+
+        if (isinstance(self.max_iter, int)) and self.max_iter <= 10:
+            raise ValueError(
+                "max_iter parameter is too low! Results won't be reliable!"
+            )
+
+        if (isinstance(self.max_iter, int)) and self.max_iter >= 1e6:
+            raise ValueError("max_iter parameter is unnecessarily high!")
+
+        # Checks for random_seed
+        if not isinstance(self.random_seed, (int, type(None))):
+            raise TypeError(
+                f"random_seed parameter must be an int, but found type {type(self.random_seed)}"
+            )
+
+        if (isinstance(self.random_seed, int)) and self.random_seed < 0:
+            raise ValueError("random_seed parameter must be > 0")
+
+        # Checks for verbose
+        if not isinstance(self.verbose, bool):
+            raise TypeError(
+                f"verbose parameter must be a boolean type, but found type {type(self.verbose)}"
+            )
+
+    def _validate_fit_data(self):
+        """Verifies that T, X, and y are formatted the right way"""
+        # Checks for T column
+        if not is_float_dtype(self.T):
+            raise TypeError("Treatment data must be of type float")
+
+        # Make sure all X columns are float or int
+        if isinstance(self.X, pd.Series):
+            if not is_numeric_dtype(self.X):
+                raise TypeError(
+                    "All covariate (X) columns must be int or float type (i.e. must be numeric)"
+                )
+
+        elif isinstance(self.X, pd.DataFrame):
+            for column in self.X:
+                if not is_numeric_dtype(self.X[column]):
+                    raise TypeError(
+                        "All covariate (X) columns must be int or float type "
+                        "(i.e. must be numeric)"
+                    )
+
+        # Checks for Y column
+        if not (is_float_dtype(self.y) or is_integer_dtype(self.y)):
+            raise TypeError("Outcome data must be of type float or integer")
+
+        if is_integer_dtype(self.y) and (
+            not np.array_equal(np.sort(self.y.unique()), np.array([0, 1]))
+        ):
+            raise TypeError(
+                "If your outcome data is of type integer (binary outcome),"
+                "it should only contain 1's and 0's."
+            )
+
+    def _grid_values(self):
+        """Produces initial grid values for the treatment variable"""
+        return np.quantile(
+            self.T,
+            q=np.linspace(
+                start=self.lower_grid_constraint,
+                stop=self.upper_grid_constraint,
+                num=self.treatment_grid_num,
+            ),
+        )
+
+    def fit(self, T, X, y):
+        """Fits the GPS causal dose-response model. For now, this only accepts pandas columns.
+        While the treatment variable must be continuous (or ordinal with many levels), the
+        outcome variable may be continuous or binary. You *must* provide
+        at least one covariate column.
+
+        Parameters
+        ----------
+        T: array-like, shape (n_samples,)
+            A continuous treatment variable.
+        X: array-like, shape (n_samples, m_features)
+            Covariates, where n_samples is the number of samples
+            and m_features is the number of features. Features can be a mix of continuous
+            and nominal/categorical variables.
+        y: array-like, shape (n_samples,)
+            Outcome variable. May be continuous or binary. If continuous, this must
+            be a series of type `float`, if binary must be a series of type `integer`.
+
+        Returns
+        ----------
+        self : object
+
+        """
+        self.rand_seed_wrapper(self.random_seed)
+
+        self.T = T.reset_index(drop=True, inplace=False)
+        self.X = X.reset_index(drop=True, inplace=False)
+        self.y = y.reset_index(drop=True, inplace=False)
+
+        # Determine what type of outcome variable we're working with
+        if is_float_dtype(self.y):
+            self.outcome_type = "continuous"
+        elif is_integer_dtype(self.y):
+            self.outcome_type = "binary"
+
+        self.if_verbose_print(
+            f"Determined the outcome variable is of type {self.outcome_type}..."
+        )
+
+        # Validate this input data
+        self._validate_fit_data()
+
+        # Create grid_values
+        self.grid_values = self._grid_values()
+
+        # Determine which GPS family to use
+        self._determine_gps_function()
+
+        # Estimate the GPS
+        self.if_verbose_print("Saving GPS values...")
+
+        self.gps = self.gps_function(self.T)
+
+        # Create GAM that predicts outcome from the treatment and GPS
+        self.if_verbose_print("Fitting GAM using treatment and GPS...")
+
+        # Save model results
+        self.gam_results = self._fit_gam()
+
+        f = io.StringIO()
+        with contextlib.redirect_stdout(f):
+            self.gam_results.summary()
+
+        self._gam_summary_str = f.getvalue()
+
+        self.if_verbose_print(
+            "Calculating many CDRC estimates for each treatment grid value..."
+        )
+
+        # Loop over all grid values (`treatment_grid_num` in total)
+        # and give GPS loading for each observation in the dataset
+        self.gps_at_grid = self._gps_values_at_grid()
+
+    def calculate_CDRC(self, ci=0.95):
+        """Using the results of the fitted model, this generates a dataframe of
+        point estimates for the CDRC at each of the values of the
+        treatment grid. Connecting these estimates will produce the overall
+        estimated CDRC. Confidence interval is returned as well.
+
+        Parameters
+        ----------
+        ci: float (default = 0.95)
+            The desired confidence interval to produce. Default value is 0.95, corresponding
+            to 95% confidence intervals. bounded (0, 1.0).
+
+        Returns
+        ----------
+        dataframe: Pandas dataframe
+            Contains treatment grid values, the CDRC point estimate at that value,
+            and the associated lower and upper confidence interval bounds at that point.
+
+        self: object
+
+        """
+        self.rand_seed_wrapper(self.random_seed)
+        self._validate_calculate_CDRC_params(ci)
+
+        self.if_verbose_print(
+            """
+            Generating predictions for each value of treatment grid,
+            and averaging to get the CDRC..."""
+        )
+
+        # Create CDRC predictions from trained GAM
+        # If working with a continuous outcome variable, use this path
+        if self.outcome_type == "continuous":
+            self._cdrc_preds = self._cdrc_predictions_continuous(ci)
+
+            results = []
+
+            for i in range(0, self.treatment_grid_num):
+                temp_grid_value = self.grid_values[i]
+                temp_point_estimate = self._cdrc_preds[:, i, 0].mean()
+                mean_ci_width = (
+                    self._cdrc_preds[:, i, 2].mean() - self._cdrc_preds[:, i, 1].mean()
+                ) / 2
+                temp_lower_bound = temp_point_estimate - mean_ci_width
+                temp_upper_bound = temp_point_estimate + mean_ci_width
+                results.append(
+                    [
+                        temp_grid_value,
+                        temp_point_estimate,
+                        temp_lower_bound,
+                        temp_upper_bound,
+                    ]
+                )
+
+            outcome_name = "Causal_Dose_Response"
+
+        # If working with a binary outcome variable, use this path
+        else:
+            self._cdrc_preds = self._cdrc_predictions_binary(ci)
+
+            # Capture the first prediction's mean log odds.
+            # This will serve as a reference for calculating the odds ratios
+            log_odds_reference = self._cdrc_preds[:, 0, 0].mean()
+
+            results = []
+
+            for i in range(0, self.treatment_grid_num):
+                temp_grid_value = self.grid_values[i]
+
+                temp_log_odds_estimate = (
+                    self._cdrc_preds[:, i, 0].mean() - log_odds_reference
+                )
+                temp_OR_estimate = np.exp(temp_log_odds_estimate)
+
+                temp_lower_bound = np.exp(
+                    temp_log_odds_estimate
+                    - (self.calculate_z_score(ci) * self._cdrc_preds[:, i, 1].mean())
+                )
+                temp_upper_bound = np.exp(
+                    temp_log_odds_estimate
+                    + (self.calculate_z_score(ci) * self._cdrc_preds[:, i, 1].mean())
+                )
+                results.append(
+                    [
+                        temp_grid_value,
+                        temp_OR_estimate,
+                        temp_lower_bound,
+                        temp_upper_bound,
+                    ]
+                )
+
+            outcome_name = "Causal_Odds_Ratio"
+
+        return pd.DataFrame(
+            results, columns=["Treatment", outcome_name, "Lower_CI", "Upper_CI"]
+        ).round(3)
+
+    @staticmethod
+    def _validate_calculate_CDRC_params(ci):
+        """Validates the parameters given to `calculate_CDRC`"""
+
+        if not isinstance(ci, float):
+            raise TypeError(
+                f"`ci` parameter must be an float, but found type {type(ci)}"
+            )
+
+        if isinstance(ci, float) and ((ci <= 0) or (ci >= 1.0)):
+            raise ValueError("`ci` parameter should be between (0, 1)")
+
+    def _gps_values_at_grid(self):
+        """Returns an array where we get the GPS-derived values for each element
+        of the treatment grid. Resulting array will be of shape (n_samples, treatment_grid_num)
+        """
+        # Creates an empty 2d array of shape (n_samples, treatment_grid_num)
+        gps_at_grid = np.zeros((len(self.T), self.treatment_grid_num), dtype=float)
+
+        # Loop over all grid values
+        for i in range(0, self.treatment_grid_num):
+            gps_at_grid[:, i] = self.gps_function(self.grid_values[i])
+
+        return gps_at_grid
+
+    def print_gam_summary(self):
+        """Prints the GAM model summary (uses pyGAM's output)
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        ----------
+        self: object
+        """
+        print(self._gam_summary_str)
+
+    def _fit_gam(self):
+        """Fits a GAM that predicts the outcome (continuous or binary) from the treatment and GPS"""
+
+        X = np.column_stack((self.T.values, self.gps))
+        y = np.asarray(self.y)
+
+        model_type_dict = {"continuous": LinearGAM, "binary": LogisticGAM}
+
+        return model_type_dict[self.outcome_type](
+            s(0, n_splines=self.n_splines, spline_order=self.spline_order)
+            + s(1, n_splines=self.n_splines, spline_order=self.spline_order),
+            max_iter=self.max_iter,
+            lam=self.lambda_,
+        ).fit(X, y)
+
+    def _determine_gps_function(self):
+        """Based on the user input, distribution of treatment values, and/or model deviances,
+        this function determines which GPS function family should be used.
+        """
+
+        # If any negative values in treatment, you must use the normal GLM family.
+        if any(self.T <= 0):
+            self.best_gps_family = "normal"
+            self.gps_function, self.gps_deviance = self._create_normal_gps_function()
+            self.if_verbose_print(
+                """Must fit `normal` GLM family to model treatment since
+                treatment takes on zero or negative values..."""
+            )
+
+        # If treatment has no negative values and user provides in put, use that.
+        elif (all(self.T > 0)) & (not isinstance(self.gps_family, type(None))):
+            self.if_verbose_print(f"Fitting GPS model of family '{self.gps_family}'...")
+
+            if self.gps_family == "normal":
+                self.best_gps_family = "normal"
+                (
+                    self.gps_function,
+                    self.gps_deviance,
+                ) = self._create_normal_gps_function()
+            elif self.gps_family == "lognormal":
+                self.best_gps_family = "lognormal"
+                (
+                    self.gps_function,
+                    self.gps_deviance,
+                ) = self._create_lognormal_gps_function()
+            elif self.gps_family == "gamma":
+                self.best_gps_family = "gamma"
+                self.gps_function, self.gps_deviance = self._create_gamma_gps_function()
+
+        # If no zero or negative treatment values and user didn't provide
+        # input, figure out best-fitting family
+        elif (all(self.T > 0)) & (isinstance(self.gps_family, type(None))):
+            self.if_verbose_print(
+                "Fitting several GPS models and" " picking the best fitting one..."
+            )
+
+            (
+                self.best_gps_family,
+                self.gps_function,
+                self.gps_deviance,
+            ) = self._find_best_gps_model()
+
+            self.if_verbose_print(
+                f"""Best fitting model was {self.best_gps_family}, which
+                    produced a deviance of {self.gps_deviance}"""
+            )
+
+    def _create_normal_gps_function(self):
+        """Models the GPS using a GLM of the Gaussian family"""
+        normal_gps_model = sm.GLM(
+            self.T, add_constant(self.X), family=sm.families.Gaussian()
+        ).fit()
+
+        pred_treat = normal_gps_model.fittedvalues
+        sigma = np.std(normal_gps_model.resid_response)
+
+        def gps_function(treatment_val, pred_treat=pred_treat, sigma=sigma):
+            return norm.pdf(treatment_val, pred_treat, sigma)
+
+        return gps_function, normal_gps_model.deviance
+
+    def _create_lognormal_gps_function(self):
+        """Models the GPS using a GLM of the Gaussian family (assumes treatment is lognormal)"""
+        lognormal_gps_model = sm.GLM(
+            np.log(self.T), add_constant(self.X), family=sm.families.Gaussian()
+        ).fit()
+
+        pred_log_treat = lognormal_gps_model.fittedvalues
+        sigma = np.std(lognormal_gps_model.resid_response)
+
+        def gps_function(treatment_val, pred_log_treat=pred_log_treat, sigma=sigma):
+            return norm.pdf(np.log(treatment_val), pred_log_treat, sigma)
+
+        return gps_function, lognormal_gps_model.deviance
+
+    def _create_gamma_gps_function(self):
+        """Models the GPS using a GLM of the Gamma family"""
+        gamma_gps_model = sm.GLM(
+            self.T, add_constant(self.X), family=sm.families.Gamma(Inverse_Power())
+        ).fit()
+
+        mu = gamma_gps_model.mu
+        scale = gamma_gps_model.scale
+        shape = mu / gamma_gps_model.scale
+
+        def gps_function(treatment_val):
+            return gamma.pdf(treatment_val, a=shape, loc=0, scale=scale)
+
+        return gps_function, gamma_gps_model.deviance
+
+    def _find_best_gps_model(self):
+        """If user doesn't provide a GLM family for modeling the GPS, this function compares
+        a few different gps models and picks the one with the lowest deviance
+        """
+        models_to_try_dict = {
+            "normal_gps_model": self._create_normal_gps_function(),
+            "lognormal_gps_model": self._create_lognormal_gps_function(),
+            "gamma_gps_model": self._create_gamma_gps_function(),
+        }
+
+        model_comparison_dict = {}
+
+        for key, value in models_to_try_dict.items():
+            model_comparison_dict[key] = value[1]
+
+        # Return model with lowest deviance
+        best_model = min(model_comparison_dict, key=model_comparison_dict.get)
+
+        return (
+            best_model,
+            models_to_try_dict[best_model][0],
+            models_to_try_dict[best_model][1],
+        )
```

### Comparing `causal-curve-1.0.6/causal_curve/gps_regressor.py` & `causal_curve-1.0.7b0/causal_curve/gps_regressor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-"""
-Defines the Generalized Prospensity Score (GPS) regressor model class
-"""
-from pprint import pprint
-
-import numpy as np
-
-from causal_curve.gps_core import GPS_Core
-
-
-class GPS_Regressor(GPS_Core):
-    """
-    A GPS tool that handles continuous outcomes. Inherits the GPS_core
-    base class. See that base class code its docstring for more details.
-
-    Methods
-    ----------
-
-    point_estimate: (self, T)
-        Calculates point estimate within the CDRC given treatment values.
-        Can only be used when outcome is continuous.
-
-    point_estimate_interval: (self, T, ci)
-        Calculates the prediction confidence interval associated with a point estimate
-        within the CDRC given treatment values. Can only be used when outcome is continuous.
-
-    """
-
-    def __init__(
-        self,
-        gps_family=None,
-        treatment_grid_num=100,
-        lower_grid_constraint=0.01,
-        upper_grid_constraint=0.99,
-        spline_order=3,
-        n_splines=30,
-        lambda_=0.5,
-        max_iter=100,
-        random_seed=None,
-        verbose=False,
-    ):
-
-        self.gps_family = gps_family
-        self.treatment_grid_num = treatment_grid_num
-        self.lower_grid_constraint = lower_grid_constraint
-        self.upper_grid_constraint = upper_grid_constraint
-        self.spline_order = spline_order
-        self.n_splines = n_splines
-        self.lambda_ = lambda_
-        self.max_iter = max_iter
-        self.random_seed = random_seed
-        self.verbose = verbose
-
-        # Validate the params
-        self._validate_init_params()
-        self.rand_seed_wrapper()
-
-        self.if_verbose_print("Using the following params for GPS model:")
-        if self.verbose:
-            pprint(self.get_params(), indent=4)
-
-    def _cdrc_predictions_continuous(self, ci):
-        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
-        we're making predictions using the original treatment and gps_at_grid.
-        To be used when the outcome of interest is continuous.
-        """
-
-        # To keep track of cdrc predictions, we create an empty 3d array of shape
-        # (n_samples, treatment_grid_num, 3). The last dimension is of length 3 because
-        # we are going to keep track of the point estimate of the prediction, as well as
-        # the lower and upper bounds of the prediction interval
-        cdrc_preds = np.zeros((len(self.T), self.treatment_grid_num, 3), dtype=float)
-
-        # Loop through each of the grid values, predict point estimate and get prediction interval
-        for i in range(0, self.treatment_grid_num):
-            temp_T = np.repeat(self.grid_values[i], repeats=len(self.T))
-            temp_gps = self.gps_at_grid[:, i]
-            temp_cdrc_preds = self.gam_results.predict(
-                np.column_stack((temp_T, temp_gps))
-            )
-            temp_cdrc_interval = self.gam_results.confidence_intervals(
-                np.column_stack((temp_T, temp_gps)), width=ci
-            )
-            temp_cdrc_lower_bound = temp_cdrc_interval[:, 0]
-            temp_cdrc_upper_bound = temp_cdrc_interval[:, 1]
-            cdrc_preds[:, i, 0] = temp_cdrc_preds
-            cdrc_preds[:, i, 1] = temp_cdrc_lower_bound
-            cdrc_preds[:, i, 2] = temp_cdrc_upper_bound
-
-        return np.round(cdrc_preds, 3)
-
-    def point_estimate(self, T):
-        """Calculates point estimate within the CDRC given treatment values.
-        Can only be used when outcome is continuous. Can be estimate for a single
-        data point or can be run in batch for many observations. Extrapolation will produce
-        untrustworthy results; the provided treatment should be within
-        the range of the training data.
-
-        Parameters
-        ----------
-        T: Numpy array, shape (n_samples,)
-            A continuous treatment variable.
-
-        Returns
-        ----------
-        array: Numpy array
-            Contains a set of CDRC point estimates
-
-        """
-        if self.outcome_type != "continuous":
-            raise TypeError("Your outcome must be continuous to use this function!")
-
-        return np.apply_along_axis(self._create_point_estimate, 0, T.reshape(1, -1))
-
-    def _create_point_estimate(self, T):
-        """Takes a single treatment value and produces a single point estimate
-        in the case of a continuous outcome.
-        """
-        return self.gam_results.predict(
-            np.array([T, self.gps_function(T).mean()]).reshape(1, -1)
-        )
-
-    def point_estimate_interval(self, T, ci=0.95):
-        """Calculates the prediction confidence interval associated with a point estimate
-        within the CDRC given treatment values. Can only be used
-        when outcome is continuous. Can be estimate for a single data point
-        or can be run in batch for many observations. Extrapolation will produce
-        untrustworthy results; the provided treatment should be within
-        the range of the training data.
-
-        Parameters
-        ----------
-        T: Numpy array, shape (n_samples,)
-            A continuous treatment variable.
-        ci: float (default = 0.95)
-            The desired confidence interval to produce. Default value is 0.95, corresponding
-            to 95% confidence intervals. bounded (0, 1.0).
-
-        Returns
-        ----------
-        array: Numpy array
-            Contains a set of CDRC prediction intervals ([lower bound, higher bound])
-
-        """
-        if self.outcome_type != "continuous":
-            raise TypeError("Your outcome must be continuous to use this function!")
-
-        return np.apply_along_axis(
-            self._create_point_estimate_interval, 0, T.reshape(1, -1), width=ci
-        ).T.reshape(-1, 2)
-
-    def _create_point_estimate_interval(self, T, width):
-        """Takes a single treatment value and produces confidence interval
-        associated with a point estimate in the case of a continuous outcome.
-        """
-        return self.gam_results.prediction_intervals(
-            np.array([T, self.gps_function(T).mean()]).reshape(1, -1), width=width
-        )
+"""
+Defines the Generalized Prospensity Score (GPS) regressor model class
+"""
+from pprint import pprint
+
+import numpy as np
+
+from causal_curve.gps_core import GPS_Core
+
+
+class GPS_Regressor(GPS_Core):
+    """
+    A GPS tool that handles continuous outcomes. Inherits the GPS_core
+    base class. See that base class code its docstring for more details.
+
+    Methods
+    ----------
+
+    point_estimate: (self, T)
+        Calculates point estimate within the CDRC given treatment values.
+        Can only be used when outcome is continuous.
+
+    point_estimate_interval: (self, T, ci)
+        Calculates the prediction confidence interval associated with a point estimate
+        within the CDRC given treatment values. Can only be used when outcome is continuous.
+
+    """
+
+    def __init__(
+        self,
+        gps_family=None,
+        treatment_grid_num=100,
+        lower_grid_constraint=0.01,
+        upper_grid_constraint=0.99,
+        spline_order=3,
+        n_splines=30,
+        lambda_=0.5,
+        max_iter=100,
+        random_seed=None,
+        verbose=False,
+    ):
+
+        self.gps_family = gps_family
+        self.treatment_grid_num = treatment_grid_num
+        self.lower_grid_constraint = lower_grid_constraint
+        self.upper_grid_constraint = upper_grid_constraint
+        self.spline_order = spline_order
+        self.n_splines = n_splines
+        self.lambda_ = lambda_
+        self.max_iter = max_iter
+        self.random_seed = random_seed
+        self.verbose = verbose
+
+        # Validate the params
+        self._validate_init_params()
+        self.rand_seed_wrapper()
+
+        self.if_verbose_print("Using the following params for GPS model:")
+        if self.verbose:
+            pprint(self.get_params(), indent=4)
+
+    def _cdrc_predictions_continuous(self, ci):
+        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
+        we're making predictions using the original treatment and gps_at_grid.
+        To be used when the outcome of interest is continuous.
+        """
+
+        # To keep track of cdrc predictions, we create an empty 3d array of shape
+        # (n_samples, treatment_grid_num, 3). The last dimension is of length 3 because
+        # we are going to keep track of the point estimate of the prediction, as well as
+        # the lower and upper bounds of the prediction interval
+        cdrc_preds = np.zeros((len(self.T), self.treatment_grid_num, 3), dtype=float)
+
+        # Loop through each of the grid values, predict point estimate and get prediction interval
+        for i in range(0, self.treatment_grid_num):
+            temp_T = np.repeat(self.grid_values[i], repeats=len(self.T))
+            temp_gps = self.gps_at_grid[:, i]
+            temp_cdrc_preds = self.gam_results.predict(
+                np.column_stack((temp_T, temp_gps))
+            )
+            temp_cdrc_interval = self.gam_results.confidence_intervals(
+                np.column_stack((temp_T, temp_gps)), width=ci
+            )
+            temp_cdrc_lower_bound = temp_cdrc_interval[:, 0]
+            temp_cdrc_upper_bound = temp_cdrc_interval[:, 1]
+            cdrc_preds[:, i, 0] = temp_cdrc_preds
+            cdrc_preds[:, i, 1] = temp_cdrc_lower_bound
+            cdrc_preds[:, i, 2] = temp_cdrc_upper_bound
+
+        return np.round(cdrc_preds, 3)
+
+    def point_estimate(self, T):
+        """Calculates point estimate within the CDRC given treatment values.
+        Can only be used when outcome is continuous. Can be estimate for a single
+        data point or can be run in batch for many observations. Extrapolation will produce
+        untrustworthy results; the provided treatment should be within
+        the range of the training data.
+
+        Parameters
+        ----------
+        T: Numpy array, shape (n_samples,)
+            A continuous treatment variable.
+
+        Returns
+        ----------
+        array: Numpy array
+            Contains a set of CDRC point estimates
+
+        """
+        if self.outcome_type != "continuous":
+            raise TypeError("Your outcome must be continuous to use this function!")
+
+        return np.apply_along_axis(self._create_point_estimate, 0, T.reshape(1, -1))
+
+    def _create_point_estimate(self, T):
+        """Takes a single treatment value and produces a single point estimate
+        in the case of a continuous outcome.
+        """
+        return self.gam_results.predict(
+            np.array([T[0], self.gps_function(T).mean()]).reshape(1, -1)
+        )
+
+    def point_estimate_interval(self, T, ci=0.95):
+        """Calculates the prediction confidence interval associated with a point estimate
+        within the CDRC given treatment values. Can only be used
+        when outcome is continuous. Can be estimate for a single data point
+        or can be run in batch for many observations. Extrapolation will produce
+        untrustworthy results; the provided treatment should be within
+        the range of the training data.
+
+        Parameters
+        ----------
+        T: Numpy array, shape (n_samples,)
+            A continuous treatment variable.
+        ci: float (default = 0.95)
+            The desired confidence interval to produce. Default value is 0.95, corresponding
+            to 95% confidence intervals. bounded (0, 1.0).
+
+        Returns
+        ----------
+        array: Numpy array
+            Contains a set of CDRC prediction intervals ([lower bound, higher bound])
+
+        """
+        if self.outcome_type != "continuous":
+            raise TypeError("Your outcome must be continuous to use this function!")
+
+        return np.apply_along_axis(
+            self._create_point_estimate_interval, 0, T.reshape(1, -1), width=ci
+        ).T.reshape(-1, 2)
+
+    def _create_point_estimate_interval(self, T, width):
+        """Takes a single treatment value and produces confidence interval
+        associated with a point estimate in the case of a continuous outcome.
+        """
+        return self.gam_results.prediction_intervals(
+            np.array([T[0], self.gps_function(T).mean()]).reshape(1, -1), width=width
+        )
```

### Comparing `causal-curve-1.0.6/causal_curve/mediation.py` & `causal_curve-1.0.7b0/causal_curve/mediation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,667 +1,667 @@
-"""
-Defines the Mediation test class
-"""
-
-from pprint import pprint
-
-import numpy as np
-import pandas as pd
-from pandas.api.types import is_float_dtype
-from pygam import LinearGAM, s
-
-from causal_curve.core import Core
-
-
-class Mediation(Core):
-    """
-    Given three continuous variables (a treatment or independent variable of interest,
-    a potential mediator, and an outcome variable of interest), Mediation provides a method
-    to determine the average direct and indirect effect.
-
-    Parameters
-    ----------
-
-    treatment_grid_num: int, optional (default = 10)
-        Takes the treatment, and creates a quantile-based grid across its values.
-        For instance, if the number 6 is selected, this means the algorithm will only take
-        the 6 treatment variable values at approximately the 0, 20, 40, 60, 80, and 100th
-        percentiles to estimate the causal dose response curve.
-        Higher value here means the final curve will be more finely estimated,
-        but also increases computation time. Default is usually a reasonable number.
-
-    lower_grid_constraint:  float, optional(default = 0.01)
-        This adds an optional constraint of the lower side of the treatment grid.
-        Sometimes data near the minimum values of the treatment are few in number
-        and thus generate unstable estimates. By default, this clips the bottom 1 percentile
-        or lower of treatment values. This can be as low as 0, indicating there is no
-        lower limit to how much treatment data is considered.
-
-    upper_grid_constraint: float, optional (default = 0.99)
-        See above parameter. Just like above, but this is an upper constraint.
-        By default, this clips the top 99th percentile or higher of treatment values.
-        This can be as high as 1.0, indicating there is no upper limit to how much
-        treatment data is considered.
-
-    bootstrap_draws: int, optional (default = 500)
-        Bootstrapping is used as part of the mediation test. The parameter determines
-        the number of draws from the original data to create a single bootstrap replicate.
-
-    bootstrap_replicates: int, optional (default = 100)
-        Bootstrapping is used as part of the mediation test. The parameter determines
-        the number of bootstrapping runs to perform / number of new datasets to create.
-
-    spline_order: int, optional (default = 3)
-        Order of the splines to use fitting the final GAM.
-        Must be integer >= 1. Default value creates cubic splines.
-
-    n_splines: int, optional (default = 5)
-        Number of splines to use for the mediation and outcome GAMs.
-        Must be integer >= 2. Must be non-negative.
-
-    lambda_: int or float, optional (default = 0.5)
-        Strength of smoothing penalty. Must be a positive float.
-        Larger values enforce stronger smoothing.
-
-    max_iter: int, optional (default = 100)
-        Maximum number of iterations allowed for the maximum likelihood algo to converge.
-
-    random_seed: int, optional (default = None)
-        Sets the random seed.
-
-    verbose: bool, optional (default = False)
-        Determines whether the user will get verbose status updates.
-
-
-    Attributes
-    ----------
-
-    grid_values: array of shape (treatment_grid_num, )
-        The gridded values of the treatment variable. Equally spaced.
-
-
-    Methods
-    ----------
-    fit: (self, T, M, y)
-        Fits the trio of relevant variables using generalized additive models.
-
-    calculate_effects: (self, ci)
-        Calculates the average direct and indirect effects.
-
-
-    Examples
-    --------
-    >>> from causal_curve import Mediation
-    >>> med = Mediation(treatment_grid_num = 200, random_seed = 512)
-    >>> med.fit(T = df['Treatment'], M = df['Mediator'], y = df['Outcome'])
-    >>> med_results = med.calculate_effects(0.95)
-
-
-    References
-    ----------
-
-    Imai K., Keele L., Tingley D. A General Approach to Causal Mediation Analysis. Psychological
-    Methods. 15(4), 2010, pp.309–334.
-
-    """
-
-    def __init__(
-        self,
-        treatment_grid_num=10,
-        lower_grid_constraint=0.01,
-        upper_grid_constraint=0.99,
-        bootstrap_draws=500,
-        bootstrap_replicates=100,
-        spline_order=3,
-        n_splines=5,
-        lambda_=0.5,
-        max_iter=100,
-        random_seed=None,
-        verbose=False,
-    ):
-
-        self.treatment_grid_num = treatment_grid_num
-        self.lower_grid_constraint = lower_grid_constraint
-        self.upper_grid_constraint = upper_grid_constraint
-        self.bootstrap_draws = bootstrap_draws
-        self.bootstrap_replicates = bootstrap_replicates
-        self.spline_order = spline_order
-        self.n_splines = n_splines
-        self.lambda_ = lambda_
-        self.max_iter = max_iter
-        self.random_seed = random_seed
-        self.verbose = verbose
-
-        # Validate the params
-        self._validate_init_params()
-        self.rand_seed_wrapper()
-
-        if self.verbose:
-            print("Using the following params for the mediation analysis:")
-            pprint(self.get_params(), indent=4)
-
-    def _validate_init_params(self):
-        """
-        Checks that the params used when instantiating mediation tool are formatted correctly
-        """
-
-        # Checks for treatment_grid_num
-        if not isinstance(self.treatment_grid_num, int):
-            raise TypeError(
-                f"treatment_grid_num parameter must be an integer, "
-                f"but found type {type(self.treatment_grid_num)}"
-            )
-
-        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num < 4:
-            raise ValueError(
-                f"treatment_grid_num parameter should be >= 4 so the internal models "
-                f"have enough resolution, but found value {self.treatment_grid_num}"
-            )
-
-        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num > 100:
-            raise ValueError("treatment_grid_num parameter is too high!")
-
-        # Checks for lower_grid_constraint
-        if not isinstance(self.lower_grid_constraint, float):
-            raise TypeError(
-                f"lower_grid_constraint parameter must be a float, "
-                f"but found type {type(self.lower_grid_constraint)}"
-            )
-
-        if (
-            isinstance(self.lower_grid_constraint, float)
-        ) and self.lower_grid_constraint < 0:
-            raise ValueError(
-                f"lower_grid_constraint parameter cannot be < 0, "
-                f"but found value {self.lower_grid_constraint}"
-            )
-
-        if (
-            isinstance(self.lower_grid_constraint, float)
-        ) and self.lower_grid_constraint >= 1.0:
-            raise ValueError(
-                f"lower_grid_constraint parameter cannot >= 1.0, "
-                f"but found value {self.lower_grid_constraint}"
-            )
-
-        # Checks for upper_grid_constraint
-        if not isinstance(self.upper_grid_constraint, float):
-            raise TypeError(
-                f"upper_grid_constraint parameter must be a float, "
-                f"but found type {type(self.upper_grid_constraint)}"
-            )
-
-        if (
-            isinstance(self.upper_grid_constraint, float)
-        ) and self.upper_grid_constraint <= 0:
-            raise ValueError(
-                f"upper_grid_constraint parameter cannot be <= 0, "
-                f"but found value {self.upper_grid_constraint}"
-            )
-
-        if (
-            isinstance(self.upper_grid_constraint, float)
-        ) and self.upper_grid_constraint > 1.0:
-            raise ValueError(
-                f"upper_grid_constraint parameter cannot > 1.0, "
-                f"but found value {self.upper_grid_constraint}"
-            )
-
-        # Checks for bootstrap_draws
-        if not isinstance(self.bootstrap_draws, int):
-            raise TypeError(
-                f"bootstrap_draws parameter must be a int, "
-                f"but found type {type(self.bootstrap_draws)}"
-            )
-
-        if (isinstance(self.bootstrap_draws, int)) and self.bootstrap_draws < 100:
-            raise ValueError(
-                f"bootstrap_draws parameter cannot be < 100, "
-                f"but found value {self.bootstrap_draws}"
-            )
-
-        if (isinstance(self.bootstrap_draws, int)) and self.bootstrap_draws > 500000:
-            raise ValueError(
-                f"bootstrap_draws parameter cannot > 500000, "
-                f"but found value {self.bootstrap_draws}"
-            )
-
-        # Checks for bootstrap_replicates
-        if not isinstance(self.bootstrap_replicates, int):
-            raise TypeError(
-                f"bootstrap_replicates parameter must be a int, "
-                f"but found type {type(self.bootstrap_replicates)}"
-            )
-
-        if (
-            isinstance(self.bootstrap_replicates, int)
-        ) and self.bootstrap_replicates < 50:
-            raise ValueError(
-                f"bootstrap_replicates parameter cannot be < 50, "
-                f"but found value {self.bootstrap_replicates}"
-            )
-
-        if (
-            isinstance(self.bootstrap_replicates, int)
-        ) and self.bootstrap_replicates > 100000:
-            raise ValueError(
-                f"bootstrap_replicates parameter cannot > 100000, "
-                f"but found value {self.bootstrap_replicates}"
-            )
-
-        # Checks for lower_grid_constraint isn't higher than upper_grid_constraint
-        if self.lower_grid_constraint >= self.upper_grid_constraint:
-            raise ValueError(
-                "lower_grid_constraint should be lower than upper_grid_constraint!"
-            )
-
-        # Checks for spline_order
-        if not isinstance(self.spline_order, int):
-            raise TypeError(
-                f"spline_order parameter must be an integer, "
-                f"but found type {type(self.spline_order)}"
-            )
-
-        if (isinstance(self.spline_order, int)) and self.spline_order < 3:
-            raise ValueError(
-                f"spline_order parameter should be >= 1, but found {self.spline_order}"
-            )
-
-        if (isinstance(self.spline_order, int)) and self.spline_order >= 30:
-            raise ValueError("spline_order parameter is too high!")
-
-        # Checks for n_splines
-        if not isinstance(self.n_splines, int):
-            raise TypeError(
-                f"n_splines parameter must be an integer, but found type {type(self.n_splines)}"
-            )
-
-        if (isinstance(self.n_splines, int)) and self.n_splines < 2:
-            raise ValueError(
-                f"n_splines parameter should be >= 2, but found {self.n_splines}"
-            )
-
-        if (isinstance(self.n_splines, int)) and self.n_splines >= 100:
-            raise ValueError("n_splines parameter is too high!")
-
-        # Checks for lambda_
-        if not isinstance(self.lambda_, (int, float)):
-            raise TypeError(
-                f"lambda_ parameter must be an int or float, but found type {type(self.lambda_)}"
-            )
-
-        if (isinstance(self.lambda_, (int, float))) and self.lambda_ <= 0:
-            raise ValueError(
-                f"lambda_ parameter should be >= 2, but found {self.lambda_}"
-            )
-
-        if (isinstance(self.lambda_, (int, float))) and self.lambda_ >= 1000:
-            raise ValueError("lambda_ parameter is too high!")
-
-        # Checks for max_iter
-        if not isinstance(self.max_iter, int):
-            raise TypeError(
-                f"max_iter parameter must be an int, but found type {type(self.max_iter)}"
-            )
-
-        if (isinstance(self.max_iter, int)) and self.max_iter <= 10:
-            raise ValueError(
-                "max_iter parameter is too low! Results won't be reliable!"
-            )
-
-        if (isinstance(self.max_iter, int)) and self.max_iter >= 1e6:
-            raise ValueError("max_iter parameter is unnecessarily high!")
-
-        # Checks for random_seed
-        if not isinstance(self.random_seed, (int, type(None))):
-            raise TypeError(
-                f"random_seed parameter must be an int, but found type {type(self.random_seed)}"
-            )
-
-        if (isinstance(self.random_seed, int)) and self.random_seed < 0:
-            raise ValueError("random_seed parameter must be > 0")
-
-        # Checks for verbose
-        if not isinstance(self.verbose, bool):
-            raise TypeError(
-                f"verbose parameter must be a boolean type, but found type {type(self.verbose)}"
-            )
-
-    def _validate_fit_data(self):
-        """Verifies that T, M, and y are formatted the right way"""
-        # Checks for T column
-        if not is_float_dtype(self.T):
-            raise TypeError("Treatment data must be of type float")
-
-        # Checks for M column
-        if not is_float_dtype(self.M):
-            raise TypeError("Mediation data must be of type float")
-
-        # Checks for Y column
-        if not is_float_dtype(self.y):
-            raise TypeError("Outcome data must be of type float")
-
-    def _grid_values(self):
-        """Produces initial grid values for the treatment variable"""
-        return np.quantile(
-            self.T,
-            q=np.linspace(
-                start=self.lower_grid_constraint,
-                stop=self.upper_grid_constraint,
-                num=self.treatment_grid_num,
-            ),
-        )
-
-    def _collect_mean_t_levels(self):
-        """Collects the mean treatment value within each treatment bucket in the grid_values"""
-
-        t_bin_means = []
-
-        for index, _ in enumerate(self.grid_values):
-            if index == (len(self.grid_values) - 1):
-                continue
-
-            t_bin_means.append(
-                self.T[
-                    (
-                        (self.T >= self.grid_values[index])
-                        & (self.T <= self.grid_values[index + 1])
-                    )
-                ].mean()
-            )
-
-        return t_bin_means
-
-    def fit(self, T, M, y):
-        """Fits models so that mediation analysis can be run.
-        For now, this only accepts pandas columns.
-
-        Parameters
-        ----------
-        T: array-like, shape (n_samples,)
-            A continuous treatment variable
-        M: array-like, shape (n_samples,)
-            A continuous mediation variable
-        y: array-like, shape (n_samples,)
-            A continuous outcome variable
-
-        Returns
-        ----------
-        self : object
-
-        """
-        self.rand_seed_wrapper(self.random_seed)
-
-        self.T = T.reset_index(drop=True, inplace=False)
-        self.M = M.reset_index(drop=True, inplace=False)
-        self.y = y.reset_index(drop=True, inplace=False)
-
-        # Validate this input data
-        self._validate_fit_data()
-
-        self.n = len(y)
-
-        # Create grid_values
-        self.grid_values = self._grid_values()
-
-        # Loop through the comparisons in the grid_values
-        if self.verbose:
-            print("Beginning main loop through treatment bins...")
-
-        # Collect loop results in this list
-        self.final_bootstrap_results = []
-
-        # Begin main loop
-        for index, _ in enumerate(self.grid_values):
-            if index == 0:
-                continue
-            if self.verbose:
-                print(
-                    f"***** Starting iteration {index} of {len(self.grid_values) - 1} *****"
-                )
-
-            temp_low_treatment = self.grid_values[index - 1]
-            temp_high_treatment = self.grid_values[index]
-
-            bootstrap_results = self._bootstrap_analysis(
-                temp_low_treatment, temp_high_treatment
-            )
-
-            self.final_bootstrap_results.append(bootstrap_results)
-
-    def calculate_mediation(self, ci=0.95):
-        """Conducts mediation analysis on the fit data
-
-        Parameters
-        ----------
-        ci: float (default = 0.95)
-            The desired bootstrap confidence interval to produce. Default value is 0.95,
-            corresponding to 95% confidence intervals. bounded (0, 1.0).
-
-        Returns
-        ----------
-        dataframe: Pandas dataframe
-            Contains the estimate of the direct and indirect effects
-            and the proportion of indirect effects across the treatment grid values.
-            The bootstrap confidence interval that is returned might not be symmetric.
-
-        self : object
-
-        """
-        self.rand_seed_wrapper(self.random_seed)
-
-        # Collect effect results in these lists
-        self.t_bin_means = self._collect_mean_t_levels()
-        self.prop_direct_list = []
-        self.prop_indirect_list = []
-        general_indirect = []
-
-        lower = (1 - ci) / 2
-        upper = ci + lower
-
-        # Calculate results for each treatment bin
-        for index, _ in enumerate(self.grid_values):
-
-            if index == (len(self.grid_values) - 1):
-                continue
-
-            temp_bootstrap_results = self.final_bootstrap_results[index]
-
-            mean_results = {
-                key: temp_bootstrap_results[key].mean()
-                for key in temp_bootstrap_results
-            }
-
-            tau_coef = (
-                mean_results["d1"]
-                + mean_results["d0"]
-                + mean_results["z1"]
-                + mean_results["z0"]
-            ) / 2
-            n0 = mean_results["d0"] / tau_coef
-            n1 = mean_results["d1"] / tau_coef
-            n_avg = (n0 + n1) / 2
-
-            tau_general = (
-                temp_bootstrap_results["d1"]
-                + temp_bootstrap_results["d0"]
-                + temp_bootstrap_results["z1"]
-                + temp_bootstrap_results["z0"]
-            ) / 2
-            nu_0_general = temp_bootstrap_results["d0"] / tau_general
-            nu_1_general = temp_bootstrap_results["d1"] / tau_general
-            nu_avg_general = (nu_0_general + nu_1_general) / 2
-
-            self.prop_direct_list.append(1 - n_avg)
-            self.prop_indirect_list.append(n_avg)
-            general_indirect.append(nu_avg_general)
-
-        general_indirect = pd.concat(general_indirect)
-
-        # Bootstrap these general_indirect values
-        bootstrap_overall_means = []
-        for _ in range(0, 1000):
-            bootstrap_overall_means.append(
-                general_indirect.sample(frac=0.25, replace=True).mean()
-            )
-
-        bootstrap_overall_means = np.array(bootstrap_overall_means)
-
-        final_results = pd.DataFrame(
-            {
-                "Treatment_Value": self.t_bin_means,
-                "Proportion_Direct_Effect": self.prop_direct_list,
-                "Proportion_Indirect_Effect": self.prop_indirect_list,
-            }
-        ).round(4)
-
-        # Clip Proportion_Direct_Effect and Proportion_Indirect_Effect
-        final_results["Proportion_Direct_Effect"].clip(lower=0, upper=1.0, inplace=True)
-        final_results["Proportion_Indirect_Effect"].clip(
-            lower=0, upper=1.0, inplace=True
-        )
-
-        # Calculate overall, mean, indirect effect
-        total_prop_mean = round(np.array(self.prop_indirect_list).mean(), 4)
-        total_prop_lower = self.clip_negatives(
-            round(np.percentile(bootstrap_overall_means, q=lower * 100), 4)
-        )
-        total_prop_upper = self.clip_negatives(
-            round(np.percentile(bootstrap_overall_means, q=upper * 100), 4)
-        )
-
-        print(
-            f"""\n\nMean indirect effect proportion:
-            {total_prop_mean} ({total_prop_lower} - {total_prop_upper})
-            """
-        )
-        return final_results
-
-    def _bootstrap_analysis(self, temp_low_treatment, temp_high_treatment):
-        """The top-level function used in the fitting method"""
-
-        bootstrap_collection = []
-
-        for _ in range(0, self.bootstrap_replicates):
-            # Create single bootstrap replicate
-            temp_t, temp_m, temp_y = self._create_bootstrap_replicate()
-            # Create the models from this
-            temp_mediator_model, temp_outcome_model = self._fit_gams(
-                temp_t, temp_m, temp_y
-            )
-            # Make mediator predictions
-            predict_m1, predict_m0 = self._mediator_prediction(
-                temp_mediator_model,
-                temp_t,
-                temp_m,
-                temp_low_treatment,
-                temp_high_treatment,
-            )
-            # Make outcome predictions
-            outcome_preds = self._outcome_prediction(
-                temp_low_treatment,
-                temp_high_treatment,
-                predict_m1,
-                predict_m0,
-                temp_outcome_model,
-            )
-            # Collect the replicate results here
-            bootstrap_collection.append(outcome_preds)
-
-        # Convert this into a dataframe
-        bootstrap_results = pd.DataFrame(bootstrap_collection)
-
-        return bootstrap_results
-
-    def _create_bootstrap_replicate(self):
-        """Creates a single bootstrap replicate from the data"""
-        temp_t = self.T.sample(n=self.bootstrap_draws, replace=True)
-        temp_m = self.M.iloc[temp_t.index]
-        temp_y = self.y.iloc[temp_t.index]
-
-        return temp_t, temp_m, temp_y
-
-    def _fit_gams(self, temp_t, temp_m, temp_y):
-        """Fits the mediator and outcome GAMs"""
-        temp_mediator_model = LinearGAM(
-            s(0, n_splines=self.n_splines, spline_order=self.spline_order),
-            fit_intercept=True,
-            max_iter=self.max_iter,
-            lam=self.lambda_,
-        )
-        temp_mediator_model.fit(temp_t, temp_m)
-
-        temp_outcome_model = LinearGAM(
-            s(0, n_splines=self.n_splines, spline_order=self.spline_order)
-            + s(1, n_splines=self.n_splines, spline_order=self.spline_order),
-            fit_intercept=True,
-            max_iter=self.max_iter,
-            lam=self.lambda_,
-        )
-        temp_outcome_model.fit(pd.concat([temp_t, temp_m], axis=1), temp_y)
-
-        return temp_mediator_model, temp_outcome_model
-
-    def _mediator_prediction(
-        self,
-        temp_mediator_model,
-        temp_t,
-        temp_m,
-        temp_low_treatment,
-        temp_high_treatment,
-    ):
-        """Makes predictions based on the mediator models"""
-
-        m1_mean = temp_mediator_model.predict(temp_high_treatment)[0]
-        m0_mean = temp_mediator_model.predict(temp_low_treatment)[0]
-
-        std_dev = (
-            (temp_mediator_model.deviance_residuals(temp_t, temp_m) ** 2).sum()
-        ) / (self.n - (len(temp_mediator_model.get_params()["terms"]._terms) + 1))
-
-        est_error = np.random.normal(loc=0, scale=std_dev, size=self.n)
-
-        predict_m1 = m1_mean + est_error
-        predict_m0 = m0_mean + est_error
-
-        return predict_m1, predict_m0
-
-    def _outcome_prediction(
-        self,
-        temp_low_treatment,
-        temp_high_treatment,
-        predict_m1,
-        predict_m0,
-        temp_outcome_model,
-    ):
-        """Makes predictions based on the outcome models"""
-
-        outcome_preds = {}
-
-        inputs = [
-            ["d1", temp_high_treatment, temp_high_treatment, predict_m1, predict_m0],
-            ["d0", temp_low_treatment, temp_low_treatment, predict_m1, predict_m0],
-            ["z1", temp_high_treatment, temp_low_treatment, predict_m1, predict_m1],
-            ["z0", temp_high_treatment, temp_low_treatment, predict_m0, predict_m0],
-        ]
-
-        for element in inputs:
-
-            # Set treatment values
-            t_1 = element[1]
-            t_0 = element[2]
-
-            # Set mediator values
-            m_1 = element[3]
-            m_0 = element[4]
-
-            pr_1 = temp_outcome_model.predict(
-                np.column_stack((np.repeat(t_1, self.n), m_1))
-            )
-
-            pr_0 = temp_outcome_model.predict(
-                np.column_stack((np.repeat(t_0, self.n), m_0))
-            )
-
-            outcome_preds[element[0]] = (pr_1 - pr_0).mean()
-
-        return outcome_preds
+"""
+Defines the Mediation test class
+"""
+
+from pprint import pprint
+
+import numpy as np
+import pandas as pd
+from pandas.api.types import is_float_dtype
+from pygam import LinearGAM, s
+
+from causal_curve.core import Core
+
+
+class Mediation(Core):
+    """
+    Given three continuous variables (a treatment or independent variable of interest,
+    a potential mediator, and an outcome variable of interest), Mediation provides a method
+    to determine the average direct and indirect effect.
+
+    Parameters
+    ----------
+
+    treatment_grid_num: int, optional (default = 10)
+        Takes the treatment, and creates a quantile-based grid across its values.
+        For instance, if the number 6 is selected, this means the algorithm will only take
+        the 6 treatment variable values at approximately the 0, 20, 40, 60, 80, and 100th
+        percentiles to estimate the causal dose response curve.
+        Higher value here means the final curve will be more finely estimated,
+        but also increases computation time. Default is usually a reasonable number.
+
+    lower_grid_constraint:  float, optional(default = 0.01)
+        This adds an optional constraint of the lower side of the treatment grid.
+        Sometimes data near the minimum values of the treatment are few in number
+        and thus generate unstable estimates. By default, this clips the bottom 1 percentile
+        or lower of treatment values. This can be as low as 0, indicating there is no
+        lower limit to how much treatment data is considered.
+
+    upper_grid_constraint: float, optional (default = 0.99)
+        See above parameter. Just like above, but this is an upper constraint.
+        By default, this clips the top 99th percentile or higher of treatment values.
+        This can be as high as 1.0, indicating there is no upper limit to how much
+        treatment data is considered.
+
+    bootstrap_draws: int, optional (default = 500)
+        Bootstrapping is used as part of the mediation test. The parameter determines
+        the number of draws from the original data to create a single bootstrap replicate.
+
+    bootstrap_replicates: int, optional (default = 100)
+        Bootstrapping is used as part of the mediation test. The parameter determines
+        the number of bootstrapping runs to perform / number of new datasets to create.
+
+    spline_order: int, optional (default = 3)
+        Order of the splines to use fitting the final GAM.
+        Must be integer >= 1. Default value creates cubic splines.
+
+    n_splines: int, optional (default = 5)
+        Number of splines to use for the mediation and outcome GAMs.
+        Must be integer >= 2. Must be non-negative.
+
+    lambda_: int or float, optional (default = 0.5)
+        Strength of smoothing penalty. Must be a positive float.
+        Larger values enforce stronger smoothing.
+
+    max_iter: int, optional (default = 100)
+        Maximum number of iterations allowed for the maximum likelihood algo to converge.
+
+    random_seed: int, optional (default = None)
+        Sets the random seed.
+
+    verbose: bool, optional (default = False)
+        Determines whether the user will get verbose status updates.
+
+
+    Attributes
+    ----------
+
+    grid_values: array of shape (treatment_grid_num, )
+        The gridded values of the treatment variable. Equally spaced.
+
+
+    Methods
+    ----------
+    fit: (self, T, M, y)
+        Fits the trio of relevant variables using generalized additive models.
+
+    calculate_effects: (self, ci)
+        Calculates the average direct and indirect effects.
+
+
+    Examples
+    --------
+    >>> from causal_curve import Mediation
+    >>> med = Mediation(treatment_grid_num = 200, random_seed = 512)
+    >>> med.fit(T = df['Treatment'], M = df['Mediator'], y = df['Outcome'])
+    >>> med_results = med.calculate_effects(0.95)
+
+
+    References
+    ----------
+
+    Imai K., Keele L., Tingley D. A General Approach to Causal Mediation Analysis. Psychological
+    Methods. 15(4), 2010, pp.309–334.
+
+    """
+
+    def __init__(
+        self,
+        treatment_grid_num=10,
+        lower_grid_constraint=0.01,
+        upper_grid_constraint=0.99,
+        bootstrap_draws=500,
+        bootstrap_replicates=100,
+        spline_order=3,
+        n_splines=5,
+        lambda_=0.5,
+        max_iter=100,
+        random_seed=None,
+        verbose=False,
+    ):
+
+        self.treatment_grid_num = treatment_grid_num
+        self.lower_grid_constraint = lower_grid_constraint
+        self.upper_grid_constraint = upper_grid_constraint
+        self.bootstrap_draws = bootstrap_draws
+        self.bootstrap_replicates = bootstrap_replicates
+        self.spline_order = spline_order
+        self.n_splines = n_splines
+        self.lambda_ = lambda_
+        self.max_iter = max_iter
+        self.random_seed = random_seed
+        self.verbose = verbose
+
+        # Validate the params
+        self._validate_init_params()
+        self.rand_seed_wrapper()
+
+        if self.verbose:
+            print("Using the following params for the mediation analysis:")
+            pprint(self.get_params(), indent=4)
+
+    def _validate_init_params(self):
+        """
+        Checks that the params used when instantiating mediation tool are formatted correctly
+        """
+
+        # Checks for treatment_grid_num
+        if not isinstance(self.treatment_grid_num, int):
+            raise TypeError(
+                f"treatment_grid_num parameter must be an integer, "
+                f"but found type {type(self.treatment_grid_num)}"
+            )
+
+        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num < 4:
+            raise ValueError(
+                f"treatment_grid_num parameter should be >= 4 so the internal models "
+                f"have enough resolution, but found value {self.treatment_grid_num}"
+            )
+
+        if (isinstance(self.treatment_grid_num, int)) and self.treatment_grid_num > 100:
+            raise ValueError("treatment_grid_num parameter is too high!")
+
+        # Checks for lower_grid_constraint
+        if not isinstance(self.lower_grid_constraint, float):
+            raise TypeError(
+                f"lower_grid_constraint parameter must be a float, "
+                f"but found type {type(self.lower_grid_constraint)}"
+            )
+
+        if (
+            isinstance(self.lower_grid_constraint, float)
+        ) and self.lower_grid_constraint < 0:
+            raise ValueError(
+                f"lower_grid_constraint parameter cannot be < 0, "
+                f"but found value {self.lower_grid_constraint}"
+            )
+
+        if (
+            isinstance(self.lower_grid_constraint, float)
+        ) and self.lower_grid_constraint >= 1.0:
+            raise ValueError(
+                f"lower_grid_constraint parameter cannot >= 1.0, "
+                f"but found value {self.lower_grid_constraint}"
+            )
+
+        # Checks for upper_grid_constraint
+        if not isinstance(self.upper_grid_constraint, float):
+            raise TypeError(
+                f"upper_grid_constraint parameter must be a float, "
+                f"but found type {type(self.upper_grid_constraint)}"
+            )
+
+        if (
+            isinstance(self.upper_grid_constraint, float)
+        ) and self.upper_grid_constraint <= 0:
+            raise ValueError(
+                f"upper_grid_constraint parameter cannot be <= 0, "
+                f"but found value {self.upper_grid_constraint}"
+            )
+
+        if (
+            isinstance(self.upper_grid_constraint, float)
+        ) and self.upper_grid_constraint > 1.0:
+            raise ValueError(
+                f"upper_grid_constraint parameter cannot > 1.0, "
+                f"but found value {self.upper_grid_constraint}"
+            )
+
+        # Checks for bootstrap_draws
+        if not isinstance(self.bootstrap_draws, int):
+            raise TypeError(
+                f"bootstrap_draws parameter must be a int, "
+                f"but found type {type(self.bootstrap_draws)}"
+            )
+
+        if (isinstance(self.bootstrap_draws, int)) and self.bootstrap_draws < 100:
+            raise ValueError(
+                f"bootstrap_draws parameter cannot be < 100, "
+                f"but found value {self.bootstrap_draws}"
+            )
+
+        if (isinstance(self.bootstrap_draws, int)) and self.bootstrap_draws > 500000:
+            raise ValueError(
+                f"bootstrap_draws parameter cannot > 500000, "
+                f"but found value {self.bootstrap_draws}"
+            )
+
+        # Checks for bootstrap_replicates
+        if not isinstance(self.bootstrap_replicates, int):
+            raise TypeError(
+                f"bootstrap_replicates parameter must be a int, "
+                f"but found type {type(self.bootstrap_replicates)}"
+            )
+
+        if (
+            isinstance(self.bootstrap_replicates, int)
+        ) and self.bootstrap_replicates < 50:
+            raise ValueError(
+                f"bootstrap_replicates parameter cannot be < 50, "
+                f"but found value {self.bootstrap_replicates}"
+            )
+
+        if (
+            isinstance(self.bootstrap_replicates, int)
+        ) and self.bootstrap_replicates > 100000:
+            raise ValueError(
+                f"bootstrap_replicates parameter cannot > 100000, "
+                f"but found value {self.bootstrap_replicates}"
+            )
+
+        # Checks for lower_grid_constraint isn't higher than upper_grid_constraint
+        if self.lower_grid_constraint >= self.upper_grid_constraint:
+            raise ValueError(
+                "lower_grid_constraint should be lower than upper_grid_constraint!"
+            )
+
+        # Checks for spline_order
+        if not isinstance(self.spline_order, int):
+            raise TypeError(
+                f"spline_order parameter must be an integer, "
+                f"but found type {type(self.spline_order)}"
+            )
+
+        if (isinstance(self.spline_order, int)) and self.spline_order < 3:
+            raise ValueError(
+                f"spline_order parameter should be >= 1, but found {self.spline_order}"
+            )
+
+        if (isinstance(self.spline_order, int)) and self.spline_order >= 30:
+            raise ValueError("spline_order parameter is too high!")
+
+        # Checks for n_splines
+        if not isinstance(self.n_splines, int):
+            raise TypeError(
+                f"n_splines parameter must be an integer, but found type {type(self.n_splines)}"
+            )
+
+        if (isinstance(self.n_splines, int)) and self.n_splines < 2:
+            raise ValueError(
+                f"n_splines parameter should be >= 2, but found {self.n_splines}"
+            )
+
+        if (isinstance(self.n_splines, int)) and self.n_splines >= 100:
+            raise ValueError("n_splines parameter is too high!")
+
+        # Checks for lambda_
+        if not isinstance(self.lambda_, (int, float)):
+            raise TypeError(
+                f"lambda_ parameter must be an int or float, but found type {type(self.lambda_)}"
+            )
+
+        if (isinstance(self.lambda_, (int, float))) and self.lambda_ <= 0:
+            raise ValueError(
+                f"lambda_ parameter should be >= 2, but found {self.lambda_}"
+            )
+
+        if (isinstance(self.lambda_, (int, float))) and self.lambda_ >= 1000:
+            raise ValueError("lambda_ parameter is too high!")
+
+        # Checks for max_iter
+        if not isinstance(self.max_iter, int):
+            raise TypeError(
+                f"max_iter parameter must be an int, but found type {type(self.max_iter)}"
+            )
+
+        if (isinstance(self.max_iter, int)) and self.max_iter <= 10:
+            raise ValueError(
+                "max_iter parameter is too low! Results won't be reliable!"
+            )
+
+        if (isinstance(self.max_iter, int)) and self.max_iter >= 1e6:
+            raise ValueError("max_iter parameter is unnecessarily high!")
+
+        # Checks for random_seed
+        if not isinstance(self.random_seed, (int, type(None))):
+            raise TypeError(
+                f"random_seed parameter must be an int, but found type {type(self.random_seed)}"
+            )
+
+        if (isinstance(self.random_seed, int)) and self.random_seed < 0:
+            raise ValueError("random_seed parameter must be > 0")
+
+        # Checks for verbose
+        if not isinstance(self.verbose, bool):
+            raise TypeError(
+                f"verbose parameter must be a boolean type, but found type {type(self.verbose)}"
+            )
+
+    def _validate_fit_data(self):
+        """Verifies that T, M, and y are formatted the right way"""
+        # Checks for T column
+        if not is_float_dtype(self.T):
+            raise TypeError("Treatment data must be of type float")
+
+        # Checks for M column
+        if not is_float_dtype(self.M):
+            raise TypeError("Mediation data must be of type float")
+
+        # Checks for Y column
+        if not is_float_dtype(self.y):
+            raise TypeError("Outcome data must be of type float")
+
+    def _grid_values(self):
+        """Produces initial grid values for the treatment variable"""
+        return np.quantile(
+            self.T,
+            q=np.linspace(
+                start=self.lower_grid_constraint,
+                stop=self.upper_grid_constraint,
+                num=self.treatment_grid_num,
+            ),
+        )
+
+    def _collect_mean_t_levels(self):
+        """Collects the mean treatment value within each treatment bucket in the grid_values"""
+
+        t_bin_means = []
+
+        for index, _ in enumerate(self.grid_values):
+            if index == (len(self.grid_values) - 1):
+                continue
+
+            t_bin_means.append(
+                self.T[
+                    (
+                        (self.T >= self.grid_values[index])
+                        & (self.T <= self.grid_values[index + 1])
+                    )
+                ].mean()
+            )
+
+        return t_bin_means
+
+    def fit(self, T, M, y):
+        """Fits models so that mediation analysis can be run.
+        For now, this only accepts pandas columns.
+
+        Parameters
+        ----------
+        T: array-like, shape (n_samples,)
+            A continuous treatment variable
+        M: array-like, shape (n_samples,)
+            A continuous mediation variable
+        y: array-like, shape (n_samples,)
+            A continuous outcome variable
+
+        Returns
+        ----------
+        self : object
+
+        """
+        self.rand_seed_wrapper(self.random_seed)
+
+        self.T = T.reset_index(drop=True, inplace=False)
+        self.M = M.reset_index(drop=True, inplace=False)
+        self.y = y.reset_index(drop=True, inplace=False)
+
+        # Validate this input data
+        self._validate_fit_data()
+
+        self.n = len(y)
+
+        # Create grid_values
+        self.grid_values = self._grid_values()
+
+        # Loop through the comparisons in the grid_values
+        if self.verbose:
+            print("Beginning main loop through treatment bins...")
+
+        # Collect loop results in this list
+        self.final_bootstrap_results = []
+
+        # Begin main loop
+        for index, _ in enumerate(self.grid_values):
+            if index == 0:
+                continue
+            if self.verbose:
+                print(
+                    f"***** Starting iteration {index} of {len(self.grid_values) - 1} *****"
+                )
+
+            temp_low_treatment = self.grid_values[index - 1]
+            temp_high_treatment = self.grid_values[index]
+
+            bootstrap_results = self._bootstrap_analysis(
+                temp_low_treatment, temp_high_treatment
+            )
+
+            self.final_bootstrap_results.append(bootstrap_results)
+
+    def calculate_mediation(self, ci=0.95):
+        """Conducts mediation analysis on the fit data
+
+        Parameters
+        ----------
+        ci: float (default = 0.95)
+            The desired bootstrap confidence interval to produce. Default value is 0.95,
+            corresponding to 95% confidence intervals. bounded (0, 1.0).
+
+        Returns
+        ----------
+        dataframe: Pandas dataframe
+            Contains the estimate of the direct and indirect effects
+            and the proportion of indirect effects across the treatment grid values.
+            The bootstrap confidence interval that is returned might not be symmetric.
+
+        self : object
+
+        """
+        self.rand_seed_wrapper(self.random_seed)
+
+        # Collect effect results in these lists
+        self.t_bin_means = self._collect_mean_t_levels()
+        self.prop_direct_list = []
+        self.prop_indirect_list = []
+        general_indirect = []
+
+        lower = (1 - ci) / 2
+        upper = ci + lower
+
+        # Calculate results for each treatment bin
+        for index, _ in enumerate(self.grid_values):
+
+            if index == (len(self.grid_values) - 1):
+                continue
+
+            temp_bootstrap_results = self.final_bootstrap_results[index]
+
+            mean_results = {
+                key: temp_bootstrap_results[key].mean()
+                for key in temp_bootstrap_results
+            }
+
+            tau_coef = (
+                mean_results["d1"]
+                + mean_results["d0"]
+                + mean_results["z1"]
+                + mean_results["z0"]
+            ) / 2
+            n0 = mean_results["d0"] / tau_coef
+            n1 = mean_results["d1"] / tau_coef
+            n_avg = (n0 + n1) / 2
+
+            tau_general = (
+                temp_bootstrap_results["d1"]
+                + temp_bootstrap_results["d0"]
+                + temp_bootstrap_results["z1"]
+                + temp_bootstrap_results["z0"]
+            ) / 2
+            nu_0_general = temp_bootstrap_results["d0"] / tau_general
+            nu_1_general = temp_bootstrap_results["d1"] / tau_general
+            nu_avg_general = (nu_0_general + nu_1_general) / 2
+
+            self.prop_direct_list.append(1 - n_avg)
+            self.prop_indirect_list.append(n_avg)
+            general_indirect.append(nu_avg_general)
+
+        general_indirect = pd.concat(general_indirect)
+
+        # Bootstrap these general_indirect values
+        bootstrap_overall_means = []
+        for _ in range(0, 1000):
+            bootstrap_overall_means.append(
+                general_indirect.sample(frac=0.25, replace=True).mean()
+            )
+
+        bootstrap_overall_means = np.array(bootstrap_overall_means)
+
+        final_results = pd.DataFrame(
+            {
+                "Treatment_Value": self.t_bin_means,
+                "Proportion_Direct_Effect": self.prop_direct_list,
+                "Proportion_Indirect_Effect": self.prop_indirect_list,
+            }
+        ).round(4)
+
+        # Clip Proportion_Direct_Effect and Proportion_Indirect_Effect
+        final_results["Proportion_Direct_Effect"].clip(lower=0, upper=1.0, inplace=True)
+        final_results["Proportion_Indirect_Effect"].clip(
+            lower=0, upper=1.0, inplace=True
+        )
+
+        # Calculate overall, mean, indirect effect
+        total_prop_mean = round(np.array(self.prop_indirect_list).mean(), 4)
+        total_prop_lower = self.clip_negatives(
+            round(np.percentile(bootstrap_overall_means, q=lower * 100), 4)
+        )
+        total_prop_upper = self.clip_negatives(
+            round(np.percentile(bootstrap_overall_means, q=upper * 100), 4)
+        )
+
+        print(
+            f"""\n\nMean indirect effect proportion:
+            {total_prop_mean} ({total_prop_lower} - {total_prop_upper})
+            """
+        )
+        return final_results
+
+    def _bootstrap_analysis(self, temp_low_treatment, temp_high_treatment):
+        """The top-level function used in the fitting method"""
+
+        bootstrap_collection = []
+
+        for _ in range(0, self.bootstrap_replicates):
+            # Create single bootstrap replicate
+            temp_t, temp_m, temp_y = self._create_bootstrap_replicate()
+            # Create the models from this
+            temp_mediator_model, temp_outcome_model = self._fit_gams(
+                temp_t, temp_m, temp_y
+            )
+            # Make mediator predictions
+            predict_m1, predict_m0 = self._mediator_prediction(
+                temp_mediator_model,
+                temp_t,
+                temp_m,
+                temp_low_treatment,
+                temp_high_treatment,
+            )
+            # Make outcome predictions
+            outcome_preds = self._outcome_prediction(
+                temp_low_treatment,
+                temp_high_treatment,
+                predict_m1,
+                predict_m0,
+                temp_outcome_model,
+            )
+            # Collect the replicate results here
+            bootstrap_collection.append(outcome_preds)
+
+        # Convert this into a dataframe
+        bootstrap_results = pd.DataFrame(bootstrap_collection)
+
+        return bootstrap_results
+
+    def _create_bootstrap_replicate(self):
+        """Creates a single bootstrap replicate from the data"""
+        temp_t = self.T.sample(n=self.bootstrap_draws, replace=True)
+        temp_m = self.M.iloc[temp_t.index]
+        temp_y = self.y.iloc[temp_t.index]
+
+        return temp_t, temp_m, temp_y
+
+    def _fit_gams(self, temp_t, temp_m, temp_y):
+        """Fits the mediator and outcome GAMs"""
+        temp_mediator_model = LinearGAM(
+            s(0, n_splines=self.n_splines, spline_order=self.spline_order),
+            fit_intercept=True,
+            max_iter=self.max_iter,
+            lam=self.lambda_,
+        )
+        temp_mediator_model.fit(temp_t, temp_m)
+
+        temp_outcome_model = LinearGAM(
+            s(0, n_splines=self.n_splines, spline_order=self.spline_order)
+            + s(1, n_splines=self.n_splines, spline_order=self.spline_order),
+            fit_intercept=True,
+            max_iter=self.max_iter,
+            lam=self.lambda_,
+        )
+        temp_outcome_model.fit(pd.concat([temp_t, temp_m], axis=1), temp_y)
+
+        return temp_mediator_model, temp_outcome_model
+
+    def _mediator_prediction(
+        self,
+        temp_mediator_model,
+        temp_t,
+        temp_m,
+        temp_low_treatment,
+        temp_high_treatment,
+    ):
+        """Makes predictions based on the mediator models"""
+
+        m1_mean = temp_mediator_model.predict(temp_high_treatment)[0]
+        m0_mean = temp_mediator_model.predict(temp_low_treatment)[0]
+
+        std_dev = (
+            (temp_mediator_model.deviance_residuals(temp_t, temp_m) ** 2).sum()
+        ) / (self.n - (len(temp_mediator_model.get_params()["terms"]._terms) + 1))
+
+        est_error = np.random.normal(loc=0, scale=std_dev, size=self.n)
+
+        predict_m1 = m1_mean + est_error
+        predict_m0 = m0_mean + est_error
+
+        return predict_m1, predict_m0
+
+    def _outcome_prediction(
+        self,
+        temp_low_treatment,
+        temp_high_treatment,
+        predict_m1,
+        predict_m0,
+        temp_outcome_model,
+    ):
+        """Makes predictions based on the outcome models"""
+
+        outcome_preds = {}
+
+        inputs = [
+            ["d1", temp_high_treatment, temp_high_treatment, predict_m1, predict_m0],
+            ["d0", temp_low_treatment, temp_low_treatment, predict_m1, predict_m0],
+            ["z1", temp_high_treatment, temp_low_treatment, predict_m1, predict_m1],
+            ["z0", temp_high_treatment, temp_low_treatment, predict_m0, predict_m0],
+        ]
+
+        for element in inputs:
+
+            # Set treatment values
+            t_1 = element[1]
+            t_0 = element[2]
+
+            # Set mediator values
+            m_1 = element[3]
+            m_0 = element[4]
+
+            pr_1 = temp_outcome_model.predict(
+                np.column_stack((np.repeat(t_1, self.n), m_1))
+            )
+
+            pr_0 = temp_outcome_model.predict(
+                np.column_stack((np.repeat(t_0, self.n), m_0))
+            )
+
+            outcome_preds[element[0]] = (pr_1 - pr_0).mean()
+
+        return outcome_preds
```

### Comparing `causal-curve-1.0.6/causal_curve/tmle_regressor.py` & `causal_curve-1.0.7b0/causal_curve/tmle_regressor.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-"""
-Defines the Targetted Maximum likelihood Estimation (TMLE) regressor model class
-"""
-from pprint import pprint
-
-import numpy as np
-
-from causal_curve.tmle_core import TMLE_Core
-
-
-class TMLE_Regressor(TMLE_Core):
-    """
-    A TMLE tool that handles continuous outcomes. Inherits the TMLE_core
-    base class. See that base class code its docstring for more details.
-
-    Methods
-    ----------
-
-    point_estimate: (self, T)
-        Calculates point estimate within the CDRC given treatment values.
-        Can only be used when outcome is continuous.
-    """
-
-    def __init__(
-        self,
-        treatment_grid_num=100,
-        lower_grid_constraint=0.01,
-        upper_grid_constraint=0.99,
-        n_estimators=200,
-        learning_rate=0.01,
-        max_depth=3,
-        bandwidth=0.5,
-        random_seed=None,
-        verbose=False,
-    ):
-
-        self.treatment_grid_num = treatment_grid_num
-        self.lower_grid_constraint = lower_grid_constraint
-        self.upper_grid_constraint = upper_grid_constraint
-        self.n_estimators = n_estimators
-        self.learning_rate = learning_rate
-        self.max_depth = max_depth
-        self.bandwidth = bandwidth
-        self.random_seed = random_seed
-        self.verbose = verbose
-
-        # Validate the params
-        self._validate_init_params()
-        self.rand_seed_wrapper()
-
-        self.if_verbose_print("Using the following params for TMLE model:")
-        if self.verbose:
-            pprint(self.get_params(), indent=4)
-
-    def _cdrc_predictions_continuous(self, ci):
-        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
-        we're making predictions using the original treatment against the pseudo-outcome.
-        To be used when the outcome of interest is continuous.
-        """
-
-        # To keep track of cdrc predictions, we create an empty 2d array of shape
-        # (treatment_grid_num, 4). The last dimension is of length 4 because
-        # we are going to keep track of the treatment, point estimate of the prediction, as well as
-        # the lower and upper bounds of the prediction interval
-        cdrc_preds = np.zeros((self.treatment_grid_num, 4), dtype=float)
-
-        # Loop through each of the grid values, get point estimate and get estimate interval
-        for i in range(0, self.treatment_grid_num):
-            temp_T = self.grid_values[i]
-            temp_cdrc_preds = self.final_gam.predict(temp_T)
-            temp_cdrc_interval = self.final_gam.confidence_intervals(temp_T, width=ci)
-            temp_cdrc_lower_bound = temp_cdrc_interval[:, 0]
-            temp_cdrc_upper_bound = temp_cdrc_interval[:, 1]
-            cdrc_preds[i, 0] = temp_T
-            cdrc_preds[i, 1] = temp_cdrc_preds
-            cdrc_preds[i, 2] = temp_cdrc_lower_bound
-            cdrc_preds[i, 3] = temp_cdrc_upper_bound
-
-        return cdrc_preds
-
-    def point_estimate(self, T):
-        """Calculates point estimate within the CDRC given treatment values.
-        Can only be used when outcome is continuous. Can be estimate for a single
-        data point or can be run in batch for many observations. Extrapolation will produce
-        untrustworthy results; the provided treatment should be within
-        the range of the training data.
-
-        Parameters
-        ----------
-        T: Numpy array, shape (n_samples,)
-            A continuous treatment variable.
-
-        Returns
-        ----------
-        array: Numpy array
-            Contains a set of CDRC point estimates
-
-        """
-        return np.apply_along_axis(self._create_point_estimate, 0, T.reshape(1, -1))
-
-    def _create_point_estimate(self, T):
-        """Takes a single treatment value and produces a single point estimate
-        in the case of a continuous outcome.
-        """
-        return self.final_gam.predict(np.array([T]).reshape(1, -1))
-
-    def point_estimate_interval(self, T, ci=0.95):
-        """Calculates the prediction confidence interval associated with a point estimate
-        within the CDRC given treatment values. Can only be used
-        when outcome is continuous. Can be estimate for a single data point
-        or can be run in batch for many observations. Extrapolation will produce
-        untrustworthy results; the provided treatment should be within
-        the range of the training data.
-
-        Parameters
-        ----------
-        T: Numpy array, shape (n_samples,)
-            A continuous treatment variable.
-        ci: float (default = 0.95)
-            The desired confidence interval to produce. Default value is 0.95, corresponding
-            to 95% confidence intervals. bounded (0, 1.0).
-
-        Returns
-        ----------
-        array: Numpy array
-            Contains a set of CDRC prediction intervals ([lower bound, higher bound])
-
-        """
-        return np.apply_along_axis(
-            self._create_point_estimate_interval, 0, T.reshape(1, -1), width=ci
-        ).T.reshape(-1, 2)
-
-    def _create_point_estimate_interval(self, T, width):
-        """Takes a single treatment value and produces confidence interval
-        associated with a point estimate in the case of a continuous outcome.
-        """
-        return self.final_gam.prediction_intervals(
-            np.array([T]).reshape(1, -1), width=width
-        )
+"""
+Defines the Targetted Maximum likelihood Estimation (TMLE) regressor model class
+"""
+from pprint import pprint
+
+import numpy as np
+
+from causal_curve.tmle_core import TMLE_Core
+
+
+class TMLE_Regressor(TMLE_Core):
+    """
+    A TMLE tool that handles continuous outcomes. Inherits the TMLE_core
+    base class. See that base class code its docstring for more details.
+
+    Methods
+    ----------
+
+    point_estimate: (self, T)
+        Calculates point estimate within the CDRC given treatment values.
+        Can only be used when outcome is continuous.
+    """
+
+    def __init__(
+        self,
+        treatment_grid_num=100,
+        lower_grid_constraint=0.01,
+        upper_grid_constraint=0.99,
+        n_estimators=200,
+        learning_rate=0.01,
+        max_depth=3,
+        bandwidth=0.5,
+        random_seed=None,
+        verbose=False,
+    ):
+
+        self.treatment_grid_num = treatment_grid_num
+        self.lower_grid_constraint = lower_grid_constraint
+        self.upper_grid_constraint = upper_grid_constraint
+        self.n_estimators = n_estimators
+        self.learning_rate = learning_rate
+        self.max_depth = max_depth
+        self.bandwidth = bandwidth
+        self.random_seed = random_seed
+        self.verbose = verbose
+
+        # Validate the params
+        self._validate_init_params()
+        self.rand_seed_wrapper()
+
+        self.if_verbose_print("Using the following params for TMLE model:")
+        if self.verbose:
+            pprint(self.get_params(), indent=4)
+
+    def _cdrc_predictions_continuous(self, ci):
+        """Returns the predictions of CDRC for each value of the treatment grid. Essentially,
+        we're making predictions using the original treatment against the pseudo-outcome.
+        To be used when the outcome of interest is continuous.
+        """
+
+        # To keep track of cdrc predictions, we create an empty 2d array of shape
+        # (treatment_grid_num, 4). The last dimension is of length 4 because
+        # we are going to keep track of the treatment, point estimate of the prediction, as well as
+        # the lower and upper bounds of the prediction interval
+        cdrc_preds = np.zeros((self.treatment_grid_num, 4), dtype=float)
+
+        # Loop through each of the grid values, get point estimate and get estimate interval
+        for i in range(0, self.treatment_grid_num):
+            temp_T = self.grid_values[i]
+            temp_cdrc_preds = self.final_gam.predict(temp_T)
+            temp_cdrc_interval = self.final_gam.confidence_intervals(temp_T, width=ci)
+            temp_cdrc_lower_bound = temp_cdrc_interval[:, 0]
+            temp_cdrc_upper_bound = temp_cdrc_interval[:, 1]
+            cdrc_preds[i, 0] = temp_T
+            cdrc_preds[i, 1] = temp_cdrc_preds
+            cdrc_preds[i, 2] = temp_cdrc_lower_bound
+            cdrc_preds[i, 3] = temp_cdrc_upper_bound
+
+        return cdrc_preds
+
+    def point_estimate(self, T):
+        """Calculates point estimate within the CDRC given treatment values.
+        Can only be used when outcome is continuous. Can be estimate for a single
+        data point or can be run in batch for many observations. Extrapolation will produce
+        untrustworthy results; the provided treatment should be within
+        the range of the training data.
+
+        Parameters
+        ----------
+        T: Numpy array, shape (n_samples,)
+            A continuous treatment variable.
+
+        Returns
+        ----------
+        array: Numpy array
+            Contains a set of CDRC point estimates
+
+        """
+        return np.apply_along_axis(self._create_point_estimate, 0, T.reshape(1, -1))
+
+    def _create_point_estimate(self, T):
+        """Takes a single treatment value and produces a single point estimate
+        in the case of a continuous outcome.
+        """
+        return self.final_gam.predict(np.array([T]).reshape(1, -1))
+
+    def point_estimate_interval(self, T, ci=0.95):
+        """Calculates the prediction confidence interval associated with a point estimate
+        within the CDRC given treatment values. Can only be used
+        when outcome is continuous. Can be estimate for a single data point
+        or can be run in batch for many observations. Extrapolation will produce
+        untrustworthy results; the provided treatment should be within
+        the range of the training data.
+
+        Parameters
+        ----------
+        T: Numpy array, shape (n_samples,)
+            A continuous treatment variable.
+        ci: float (default = 0.95)
+            The desired confidence interval to produce. Default value is 0.95, corresponding
+            to 95% confidence intervals. bounded (0, 1.0).
+
+        Returns
+        ----------
+        array: Numpy array
+            Contains a set of CDRC prediction intervals ([lower bound, higher bound])
+
+        """
+        return np.apply_along_axis(
+            self._create_point_estimate_interval, 0, T.reshape(1, -1), width=ci
+        ).T.reshape(-1, 2)
+
+    def _create_point_estimate_interval(self, T, width):
+        """Takes a single treatment value and produces confidence interval
+        associated with a point estimate in the case of a continuous outcome.
+        """
+        return self.final_gam.prediction_intervals(
+            np.array([T]).reshape(1, -1), width=width
+        )
```

### Comparing `causal-curve-1.0.6/setup.py` & `causal_curve-1.0.7b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="causal-curve",
-    version="1.0.6",
-    author="Roni Kobrosly",
-    author_email="roni.kobrosly@gmail.com",
-    description="A python library with tools to perform causal inference using \
-        observational data when the treatment of interest is continuous.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/ronikobrosly/causal-curve",
-    packages=setuptools.find_packages(include=['causal_curve']),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'black',
-        'coverage',
-        'future',
-        'joblib',
-        'numpy',
-        'numpydoc',
-        'pandas',
-        'patsy',
-        'progressbar2',
-        'pygam',
-        'pytest',
-        'python-dateutil',
-        'python-utils',
-        'pytz',
-        'scikit-learn',
-        'scipy',
-        'six',
-        'sphinx_rtd_theme',
-        'statsmodels'
-    ]
-)
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="causal-curve",
+    version="1.0.7b",
+    author="Roni Kobrosly",
+    author_email="roni.kobrosly@gmail.com",
+    description="A python library with tools to perform causal inference using \
+        observational data when the treatment of interest is continuous.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/ronikobrosly/causal-curve",
+    packages=setuptools.find_packages(include=['causal_curve']),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+        'black',
+        'coverage',
+        'future',
+        'joblib',
+        'numpy',
+        'numpydoc',
+        'pandas',
+        'patsy',
+        'progressbar2',
+        'pygam',
+        'pytest',
+        'python-dateutil',
+        'python-utils',
+        'pytz',
+        'scikit-learn',
+        'scipy',
+        'six',
+        'sphinx_rtd_theme',
+        'statsmodels'
+    ]
+)
```

