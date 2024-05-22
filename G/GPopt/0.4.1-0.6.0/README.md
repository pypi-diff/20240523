# Comparing `tmp/GPopt-0.4.1.tar.gz` & `tmp/gpopt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPopt-0.4.1.tar", last modified: Mon Feb  5 23:39:52 2024, max compression
+gzip compressed data, was "gpopt-0.6.0.tar", last modified: Wed May 22 21:12:35 2024, max compression
```

## Comparing `GPopt-0.4.1.tar` & `gpopt-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.127454 GPopt-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.123454 GPopt-0.4.1/GPopt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.123454 GPopt-0.4.1/GPopt/GPOpt/
--rw-r--r--   0 runner    (1001) docker     (127)    21990 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/GPOpt/GPOpt.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/GPOpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.123454 GPopt-0.4.1/GPopt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/utils/nodesimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/utils/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)   346940 2024-02-05 23:39:20.000000 GPopt-0.4.1/GPopt/utils/sobol_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.127454 GPopt-0.4.1/GPopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-05 23:39:52.000000 GPopt-0.4.1/GPopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-05 23:39:52.000000 GPopt-0.4.1/GPopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 23:39:52.000000 GPopt-0.4.1/GPopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 23:39:52.000000 GPopt-0.4.1/GPopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 23:39:52.000000 GPopt-0.4.1/GPopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-05 23:39:20.000000 GPopt-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 23:39:20.000000 GPopt-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-05 23:39:52.127454 GPopt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-05 23:39:20.000000 GPopt-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 23:39:20.000000 GPopt-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-05 23:39:52.127454 GPopt-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-05 23:39:20.000000 GPopt-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:39:52.127454 GPopt-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-05 23:39:20.000000 GPopt-0.4.1/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:35.055205 gpopt-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:35.051205 gpopt-0.6.0/GPopt/
+-rw-r--r--   0 runner    (1001) docker     (127)    40305 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/GPOpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:35.051205 gpopt-0.6.0/GPopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/utils/nodesimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/utils/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   346938 2024-05-22 21:12:01.000000 gpopt-0.6.0/GPopt/utils/sobol_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:35.055205 gpopt-0.6.0/GPopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 21:12:35.000000 gpopt-0.6.0/GPopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 21:12:35.000000 gpopt-0.6.0/GPopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:12:35.000000 gpopt-0.6.0/GPopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 21:12:35.000000 gpopt-0.6.0/GPopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 21:12:35.000000 gpopt-0.6.0/GPopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-22 21:12:01.000000 gpopt-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 21:12:01.000000 gpopt-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 21:12:35.055205 gpopt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-22 21:12:01.000000 gpopt-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 21:12:01.000000 gpopt-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 21:12:35.055205 gpopt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-22 21:12:01.000000 gpopt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:12:35.055205 gpopt-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 21:12:01.000000 gpopt-0.6.0/tests/test_sample.py
```

### Comparing `GPopt-0.4.1/GPopt/GPOpt/GPOpt.py` & `gpopt-0.6.0/GPopt/GPOpt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """GPOpt class."""
 
 # Authors: T. Moudiki
 #
 # License: BSD 3 Clause Clear
 
+import copy
+import nnetsauce as ns
 import numpy as np
 import pickle
 import shelve
 from collections import namedtuple
+from functools import partial
+from sklearn.utils.discovery import all_estimators
+from sklearn.base import RegressorMixin
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.gaussian_process.kernels import Matern
 import scipy.stats as st
 from joblib import Parallel, delayed
 from time import time
-from ..utils import generate_sobol2
-from ..utils import Progbar
+from tqdm import tqdm
+from .config import REGRESSORS, REMOVED_REGRESSORS
+from .utils import generate_sobol2
+from .utils import Progbar
 
 
 class GPOpt:
     """Class GPOpt.
 
     # Arguments:
 
@@ -27,20 +34,20 @@
             lower bound for researched minimum
 
         upper_bound: a numpy array;
             upper bound for researched minimum
 
         objective_func: a function;
             the objective function to be minimized
-        
+
         params_names: a list;
             names of the parameters of the objective function (optional)
 
-        gp_obj: a GaussianProcessRegressor object;
-            An ML model for estimating the uncertainty around the objective function        
+        surrogate_obj: a GaussianProcessRegressor object;
+            An ML model for estimating the uncertainty around the objective function
 
         x_init:
             initial setting of points where `objective_func` is evaluated (optional)
 
         y_init:
             initial setting values at points where `objective_func` is evaluated (optional)
 
@@ -62,44 +69,53 @@
         seed: an integer;
             reproducibility seed
 
         save: a string;
             Specifies where to save the optimizer in its current state
 
         n_jobs: an integer;
-            number of jobs for parallel computing on initial setting (can be -1)
+            number of jobs for parallel computing on initial setting or method `lazyoptimize` (can be -1)
+
+        acquisition: a string;
+            acquisition function: "ei" (expected improvement) or "ucb" (upper confidence bound)
+
+        min_value: a float;
+            minimum value of the objective function (default is None). For example,
+            if objective function is accuracy, will be 1, and the algorithm will stop
 
         per_second: a boolean;
             __experimental__, default is False (leave to default for now)
 
         log_scale: a boolean;
             __experimental__, default is False (leave to default for now)
 
     see also [Bayesian Optimization with GPopt](https://thierrymoudiki.github.io/blog/2021/04/16/python/misc/gpopt)
         and [Hyperparameters tuning with GPopt](https://thierrymoudiki.github.io/blog/2021/06/11/python/misc/hyperparam-tuning-gpopt)
 
     """
 
     def __init__(
-        self,        
+        self,
         lower_bound,
         upper_bound,
         objective_func=None,
         params_names=None,
-        gp_obj=None,
+        surrogate_obj=None,
         x_init=None,
         y_init=None,
         n_init=10,
         n_choices=25000,
         n_iter=190,
         alpha=1e-6,
         n_restarts_optimizer=25,
         seed=123,
         save=None,
-        n_jobs=1,
+        n_jobs=None,
+        acquisition="ei",
+        min_value=None,
         per_second=False,  # /!\ very experimental
         log_scale=False,  # /!\ experimental
     ):
 
         n_dims = len(lower_bound)
 
         assert n_dims == len(
@@ -116,31 +132,37 @@
         self.n_init = n_init
         self.n_choices = n_choices
         self.n_iter = n_iter
         self.alpha = alpha
         self.n_restarts_optimizer = n_restarts_optimizer
         self.seed = seed
         self.save = save
+        self.n_jobs = n_jobs  # for parallel case on initial design
         self.per_second = per_second
         self.x_min = None
         self.y_min = None
         self.y_mean = None
         self.y_std = None
-        self.ei = np.array([])
-        self.max_ei = []
-        if gp_obj is None:
-            self.gp_obj = GaussianProcessRegressor(
+        self.best_surrogate = None
+        self.acquisition = acquisition
+        self.min_value = min_value
+        self.acq = np.array([])
+        self.max_acq = []
+        if surrogate_obj is None:
+            self.surrogate_obj = GaussianProcessRegressor(
                 kernel=Matern(nu=2.5),
                 alpha=self.alpha,
                 normalize_y=True,
                 n_restarts_optimizer=self.n_restarts_optimizer,
                 random_state=self.seed,
             )
         else:
-            self.gp_obj = gp_obj
+            self.surrogate_obj = surrogate_obj
+        self.method = None
+        self.posterior_ = None
 
         # Sobol seqs for initial design and choices
         sobol_seq_init = np.transpose(
             generate_sobol2(
                 n_dims=self.n_dims,
                 n_points=self.n_init,
                 skip=2,
@@ -258,66 +280,94 @@
 
         See also: [Bayesian Optimization with GPopt Part 2 (save and resume)](https://thierrymoudiki.github.io/blog/2021/04/30/python/misc/gpopt)
         """
 
         self.sh.close()
 
     # fit predict
-    def gp_fit_predict(self, X_train, y_train, X_test):
+    def surrogate_fit_predict(
+        self, X_train, y_train, X_test, return_std=False, return_pi=False
+    ):
 
         if len(X_train.shape) == 1:
             X_train = X_train.reshape((-1, 1))
             X_test = X_test.reshape((-1, 1))
 
-        # Get mean and standard deviation
-        return self.gp_obj.fit(X_train, y_train).predict(
-            X_test, return_std=True
-        )
+        # Get mean and standard deviation (+ lower and upper for not GPs)
+        assert (
+            return_std == True and return_pi == True
+        ) == False, "must have either return_std == True or return_pi == True"
+        if return_std == True:
+            self.posterior_ = "gaussian"
+            return self.surrogate_obj.fit(X_train, y_train).predict(
+                X_test, return_std=True
+            )
+        elif return_pi == True:
+            self.posterior_ = "mc"
+            res = self.surrogate_obj.fit(X_train, y_train).predict(
+                X_test, return_pi=True, method="splitconformal"
+            )
+            self.y_sims = res.sims
+            self.y_mean, self.y_std = (
+                np.mean(self.y_sims, axis=1),
+                np.std(self.y_sims, axis=1),
+            )
+            return self.y_mean, self.y_std, self.y_sims
+        else:
+            raise NotImplementedError
 
     # fit predict timings
     def timings_fit_predict(self, X_train, y_train, X_test):
 
         if len(X_train.shape) == 1:
             X_train = X_train.reshape((-1, 1))
             X_test = X_test.reshape((-1, 1))
 
         # Get mean preds for timings
         return self.rf_obj.fit(X_train, y_train).predict(X_test)
 
     # find next parameter by using expected improvement (ei)
-    def next_parameter_by_ei(self, seed, i):
+    def next_parameter_by_acq(self, i, acq="ei"):
 
-        gamma_hat = (self.y_min - self.y_mean) / self.y_std
+        if acq == "ei":
+            if self.posterior_ == "gaussian":
+                gamma_hat = (self.y_min - self.y_mean) / self.y_std
+                self.acq = -self.y_std * (
+                    gamma_hat * st.norm.cdf(gamma_hat) + st.norm.pdf(gamma_hat)
+                )
+            elif self.posterior_ == "mc":
+                self.acq = -np.mean(
+                    np.maximum(self.y_min - self.y_sims, 0), axis=1
+                )
 
-        self.ei = -self.y_std * (
-            gamma_hat * st.norm.cdf(gamma_hat) + st.norm.pdf(gamma_hat)
-        )
+        if acq == "ucb":
+            self.acq = -(self.y_mean - 1.96 * self.y_std)
 
         # find max index -----
 
         if self.per_second is False:
 
             # find index for max. ei
-            max_index = self.ei.argmin()
+            max_index = self.acq.argmin()
 
         else:  # self.per_second is True
 
             # predict timings on self.x_choices
             # train on X = self.parameters and y = self.timings
             # (must have same shape[0])
             timing_preds = self.timings_fit_predict(
                 X_train=np.asarray(self.parameters),
                 y_train=np.asarray(self.timings),
                 X_test=self.x_choices,
             )
 
             # find index for max. ei (and min. timings)
-            max_index = (-self.ei / timing_preds).argmax()
+            max_index = (-self.acq / timing_preds).argmax()
 
-        self.max_ei.append(np.abs(self.ei[max_index]))
+        self.max_acq.append(np.abs(self.acq[max_index]))
 
         # Select next choice
         next_param = self.x_choices[max_index, :]
 
         if next_param in np.asarray(self.parameters):
 
             if self.log_scale == False:
@@ -348,14 +398,15 @@
     def optimize(
         self,
         verbose=1,
         n_more_iter=None,
         abs_tol=None,  # suggested 1e-4, for n_iter = 200
         min_budget=50,  # minimum budget for early stopping
         func_args=None,
+        method="bayesian",
     ):
         """Launch optimization loop.
 
         # Arguments:
 
             verbose: an integer;
                 verbose = 0: nothing is printed,
@@ -370,19 +421,28 @@
 
             min_budget: an integer (default is 50);
                 minimum number of iterations before early stopping controlled by `abs_tol`
 
             func_args: a list;
                 additional parameters for the objective function (if necessary)
 
+            method: an str;
+                "bayesian" (default) for Gaussian posteriors or "mc" for Monte Carlo posteriors
+
         see also [Bayesian Optimization with GPopt](https://thierrymoudiki.github.io/blog/2021/04/16/python/misc/gpopt)
         and [Hyperparameters tuning with GPopt](https://thierrymoudiki.github.io/blog/2021/06/11/python/misc/hyperparam-tuning-gpopt)
 
         """
 
+        assert method in (
+            "bayesian",
+            "mc",
+        ), "method must be in ('bayesian', 'mc')"
+        self.method = method
+
         # verbose = 0: nothing is printed
         # verbose = 1: a progress bar is printed (longer than 0)
         # verbose = 2: information about each iteration is printed (longer than 1)
         if func_args is None:
             func_args = []
 
         if (
@@ -470,15 +530,15 @@
                     )
 
                     self.scores = scores
 
                     if self.save is not None:
                         self.update_shelve()
 
-            else:  # if self.y_init is None:
+            else:  # if self.y_init is not None:
 
                 assert self.x_init.shape[0] == len(
                     self.y_init
                 ), "must have: self.x_init.shape[0] == len(self.y_init)"
 
                 self.scores = pickle.loads(
                     pickle.dumps(self.y_init.tolist(), -1)
@@ -486,31 +546,64 @@
 
             # current best score on initial design
             min_index = (np.asarray(self.scores)).argmin()
             self.y_min = self.scores[min_index]
             self.x_min = self.x_init[min_index, :]
 
             # current gp mean and std on initial design
-            y_mean, y_std = self.gp_fit_predict(
-                np.asarray(self.parameters),
-                np.asarray(self.scores),
-                self.x_choices,
-            )
+            # /!\ if GP
+            if self.method == "bayesian":
+                self.posterior_ = "gaussian"
+                try:
+                    y_mean, y_std = self.surrogate_fit_predict(
+                        np.asarray(self.parameters),
+                        np.asarray(self.scores),
+                        self.x_choices,
+                        return_std=True,
+                        return_pi=False,
+                    )
+                except ValueError:  # do not remove this
+                    preds_with_std = self.surrogate_fit_predict(
+                        np.asarray(self.parameters),
+                        np.asarray(self.scores),
+                        self.x_choices,
+                        return_std=True,
+                        return_pi=False,
+                    )
+                    y_mean, y_std = preds_with_std[0], preds_with_std[1]
+
+            elif self.method == "mc":
+                self.posterior_ = "mc"
+                assert self.surrogate_obj.__class__.__name__.startswith(
+                    "CustomRegressor"
+                ), "for `method = 'mc'`, the surrogate must be a nnetsauce.CustomRegressor()"
+                assert (
+                    self.surrogate_obj.replications is not None
+                ), "for `method = 'mc'`, the surrogate must be a nnetsauce.CustomRegressor() with a number of 'replications' provided"
+                preds_with_std = self.surrogate_fit_predict(
+                    np.asarray(self.parameters),
+                    np.asarray(self.scores),
+                    self.x_choices,
+                    return_std=False,
+                    return_pi=True,
+                )
+                y_mean, y_std = preds_with_std[0], preds_with_std[1]
+
             self.y_mean = y_mean
             self.y_std = np.maximum(2.220446049250313e-16, y_std)
 
             # saving after initial design computation
             if self.save is not None:
                 self.update_shelve()
 
         else:  # if n_more_iter is not None
 
             assert self.n_iter > 5, "you must have n_iter > 5"
             n_iter = n_more_iter
-            iter_stop = len(self.max_ei) + n_more_iter  # potentially
+            iter_stop = len(self.max_acq) + n_more_iter  # potentially
 
         if (verbose == 1) | (verbose == 2):
             print(f"\n ...Done. \n")
             try:
                 print(np.hstack((self.x_init, self.y_init.reshape(-1, 1))))
             except:
                 pass
@@ -532,15 +625,15 @@
             progbar = Progbar(target=n_iter)
 
         # main loop ----------
 
         for i in range(n_iter):
 
             # find next set of parameters (vector), maximizing ei
-            next_param = self.next_parameter_by_ei(seed=len(self.max_ei), i=i)
+            next_param = self.next_parameter_by_acq(i=i, acq="ei")
 
             try:
 
                 if self.per_second is True:
 
                     start = time()
 
@@ -621,57 +714,427 @@
                 print(f"score for next parameter: {score_next_param} \n")
 
             if score_next_param < self.y_min:
                 self.x_min = next_param
                 self.y_min = score_next_param
                 if self.save is not None:
                     self.update_shelve()
+                if self.y_min == self.min_value:
+                    break
 
-            self.y_mean, self.y_std = self.gp_fit_predict(
-                np.asarray(self.parameters),
-                np.asarray(self.scores),
-                self.x_choices,
-            )
+            if self.posterior_ == "gaussian" and self.method == "bayesian":
+                try:
+                    self.y_mean, self.y_std = self.surrogate_fit_predict(
+                        np.asarray(self.parameters),
+                        np.asarray(self.scores),
+                        self.x_choices,
+                        return_std=True,
+                        return_pi=False,
+                    )
+                except:
+                    self.y_mean, self.y_std, lower, upper = (
+                        self.surrogate_fit_predict(
+                            np.asarray(self.parameters),
+                            np.asarray(self.scores),
+                            self.x_choices,
+                            return_std=True,
+                            return_pi=False,
+                        )
+                    )
+
+            elif self.posterior_ == "mc" and self.method == "mc":
+                self.y_mean, self.y_std, self.y_sims = (
+                    self.surrogate_fit_predict(
+                        np.asarray(self.parameters),
+                        np.asarray(self.scores),
+                        self.x_choices,
+                        return_std=False,
+                        return_pi=True,
+                    )
+                )
+            else:
+                return NotImplementedError
 
             if self.save is not None:
                 self.update_shelve()
 
             if verbose == 1:
                 progbar.update(i + 1)  # update progress bar
 
             # early stopping
 
             if abs_tol is not None:
 
-                # if self.max_ei.size > (self.n_init + self.n_iter * min_budget_pct):
-                if len(self.max_ei) > min_budget:
+                # if self.max_acq.size > (self.n_init + self.n_iter * min_budget_pct):
+                if len(self.max_acq) > min_budget:
 
-                    diff_max_ei = np.abs(np.diff(np.asarray(self.max_ei)))
+                    diff_max_ei = np.abs(np.diff(np.asarray(self.max_acq)))
 
                     if diff_max_ei[-1] <= abs_tol:
 
-                        iter_stop = len(self.max_ei)  # index i starts at 0
+                        iter_stop = len(self.max_acq)  # index i starts at 0
 
                         break
 
         # end main loop ----------
 
         if (verbose == 1) & (i < (n_iter - 1)):
             progbar.update(n_iter)
 
         self.n_iter = iter_stop
         if self.save is not None:
             self.update_shelve()
-        
+
         DescribeResult = namedtuple(
-                "DescribeResult", ("best_params", "best_score")
-            )
+            "DescribeResult", ("best_params", "best_score")
+        )
 
         if self.params_names is None:
 
             return DescribeResult(self.x_min, self.y_min)
 
         else:
 
             return DescribeResult(
                 dict(zip(self.params_names, self.x_min)), self.y_min
             )
+
+    # optimize the objective
+    def lazyoptimize(
+        self,
+        verbose=1,
+        abs_tol=None,  # suggested 1e-4, for n_iter = 200
+        min_budget=50,  # minimum budget for early stopping
+        func_args=None,
+        method="bayesian",  # "bayesian" or "mc
+        estimators="all",
+        type_pi="kde", # for now, 'kde' or 'bootstrap'
+        type_exec="independent",  # "queue" or "independent" (default)
+    ):
+        """Launch optimization loop.
+
+        # Arguments:
+
+            verbose: an integer;
+                verbose = 0: nothing is printed,
+                verbose = 1: a progress bar is printed (longer than 0),
+                verbose = 2: information about each iteration is printed (longer than 1)
+
+            n_more_iter: an integer;
+                additional number of iterations for the optimizer (which has been run once)
+
+            abs_tol: a float;
+                tolerance for convergence of the optimizer (early stopping based on expected improvement)
+
+            min_budget: an integer (default is 50);
+                minimum number of iterations before early stopping controlled by `abs_tol`
+
+            func_args: a list;
+                additional parameters for the objective function (if necessary)
+
+            method: an str;
+                "bayesian" (default) for Gaussian posteriors or "mc" for Monte Carlo posteriors
+
+            estimators: an str or a list of strs (estimators names)
+                if "all", then 30 models are fitted. Otherwise, only those provided in the list
+                are adjusted; for example ["RandomForestRegressor", "Ridge"]
+            
+            type_pi: an str;
+                "kde" (default) or "bootstrap"; type of prediction intervals for the surrogate 
+                model 
+
+            type_exec: an str;
+                "independent" (default) is when surrogate models are adjusted independently on
+                the same design set and the best model is chosen eventually; "queue" is when
+                surrogate models are adjusted one after the other, on a design set with
+                increasing size;
+
+        """
+
+        if estimators == "all":
+
+            self.regressors = REGRESSORS
+
+        else:
+
+            self.regressors = [
+                (
+                    "CustomRegressor(" + est[0] + ")",
+                    ns.CustomRegressor(
+                        est[1](), replications=150, type_pi=type_pi
+                    ),
+                )
+                for est in all_estimators()
+                if (
+                    issubclass(est[1], RegressorMixin)
+                    and (est[0] not in REMOVED_REGRESSORS)
+                    and (est[0] in estimators)
+                )
+            ]
+
+        self.surrogate_fit_predict = partial(
+            self.surrogate_fit_predict, return_pi=True
+        )
+
+        if (
+            type_exec == "queue"
+        ):  # when models are adjusted one after the other on a design set with increasing size
+
+            self.x_min = None
+
+            self.y_min = np.inf
+
+            score_next_param = np.inf
+
+            DescribeResult = namedtuple(
+                "DescribeResult", ("best_params", "best_score")
+            )
+
+            if verbose == 2:
+                print(
+                    f"\n adjusting surrogate model # {1} ({self.regressors[0][0]})... \n"
+                )
+
+            gp_opt_obj_prev = GPOpt(
+                objective_func=self.objective_func,
+                lower_bound=self.lower_bound,
+                upper_bound=self.upper_bound,
+                n_init=self.n_init,
+                n_iter=self.n_iter,
+                alpha=self.alpha,
+                n_restarts_optimizer=self.n_restarts_optimizer,
+                seed=self.seed,
+                n_jobs=self.n_jobs,
+                acquisition=self.acquisition,
+                min_value=self.min_value,
+                surrogate_obj=copy.deepcopy(self.regressors[0][1]),
+            )
+
+            gp_opt_obj_prev.optimize(
+                verbose=verbose,
+                abs_tol=abs_tol,  # suggested 1e-4, for n_iter = 200
+                min_budget=min_budget,  # minimum budget for early stopping
+                func_args=func_args,
+                method=method,
+            )
+
+            score_next_param = gp_opt_obj_prev.y_min
+
+            if self.n_jobs is None:  # sequential optimization
+
+                for i in range(len(self.regressors)):
+
+                    try:
+
+                        if verbose == 2:
+                            print(
+                                f"\n adjusting surrogate model # {i + 2} ({self.regressors[i][0]})... \n"
+                            )
+
+                        gp_opt_obj = GPOpt(
+                            objective_func=self.objective_func,
+                            lower_bound=self.lower_bound,
+                            upper_bound=self.upper_bound,
+                            n_init=self.n_init,
+                            n_iter=self.n_iter,
+                            alpha=self.alpha,
+                            n_restarts_optimizer=self.n_restarts_optimizer,
+                            seed=self.seed,
+                            n_jobs=self.n_jobs,
+                            acquisition=self.acquisition,
+                            min_value=self.min_value,
+                            surrogate_obj=copy.deepcopy(self.regressors[i][1]),
+                            x_init=np.asarray(gp_opt_obj_prev.parameters),
+                            y_init=np.asarray(gp_opt_obj_prev.scores),
+                        )
+
+                        gp_opt_obj.optimize(
+                            verbose=verbose,
+                            abs_tol=abs_tol,  # suggested 1e-4, for n_iter = 200
+                            min_budget=min_budget,  # minimum budget for early stopping
+                            func_args=func_args,
+                            method=method,
+                        )
+
+                        score_next_param = gp_opt_obj.y_min
+
+                        if score_next_param < self.y_min:
+                            self.x_min = gp_opt_obj.x_min
+                            self.y_min = score_next_param
+                            if self.y_min == self.min_value:
+                                break
+
+                        if verbose == 2:
+                            print(f"Global iteration #{i + 1} -----")
+                            print(f"current minimum:  {self.x_min}")
+                            print(f"current minimum score:  {self.y_min}")
+                            print(
+                                f"score for next parameter: {score_next_param} \n"
+                            )
+
+                        gp_opt_obj_prev = copy.deepcopy(gp_opt_obj)
+
+                    except ValueError:
+
+                        continue
+
+            elif self.n_jobs >= 2 or self.n_jobs == -1:  # parallel optimization
+                pass
+            else:
+                raise ValueError(
+                    "n_jobs must be either None or >= 2 or equal to -1"
+                )
+            return DescribeResult(self.x_min, self.y_min)
+
+        elif (
+            type_exec == "independent"
+        ):  # when models are adjusted independently on the same design set and the best model is chosen eventually
+
+            self.x_min = None
+
+            self.y_min = np.inf
+
+            score_next_param = np.inf
+
+            DescribeResult = namedtuple(
+                "DescribeResult",
+                ("best_params", "best_score", "best_surrogate"),
+            )
+
+            if verbose == 2:
+                print(
+                    f"\n adjusting surrogate model # {1} ({self.regressors[0][0]})... \n"
+                )
+
+            if self.n_jobs is None:  # sequential optimization
+
+                for i in range(len(self.regressors)):
+
+                    try:
+
+                        if verbose == 2:
+                            print(
+                                f"\n adjusting surrogate model # {i + 1} ({self.regressors[i][0]})... \n"
+                            )
+
+                        gp_opt_obj = GPOpt(
+                            objective_func=self.objective_func,
+                            lower_bound=self.lower_bound,
+                            upper_bound=self.upper_bound,
+                            n_init=self.n_init,
+                            n_iter=self.n_iter,
+                            alpha=self.alpha,
+                            n_restarts_optimizer=self.n_restarts_optimizer,
+                            seed=self.seed,
+                            n_jobs=self.n_jobs,
+                            acquisition=self.acquisition,
+                            min_value=self.min_value,
+                            surrogate_obj=copy.deepcopy(self.regressors[i][1]),
+                        )
+
+                        gp_opt_obj.optimize(
+                            verbose=verbose,
+                            abs_tol=abs_tol,  # suggested 1e-4, for n_iter = 200
+                            min_budget=min_budget,  # minimum budget for early stopping
+                            func_args=func_args,
+                            method=method,
+                        )
+
+                        score_next_param = gp_opt_obj.y_min
+
+                        if score_next_param < self.y_min:
+                            self.x_min = gp_opt_obj.x_min
+                            self.y_min = score_next_param
+                            self.best_surrogate = copy.deepcopy(
+                                gp_opt_obj.surrogate_obj
+                            )
+                            if self.y_min == self.min_value:
+                                break
+
+                        if verbose == 2:
+                            print(f"Global iteration #{i + 1} -----")
+                            print(f"current minimum:  {self.x_min}")
+                            print(f"current minimum score:  {self.y_min}")
+                            print(
+                                f"score for next parameter: {score_next_param} \n"
+                            )
+
+                    except ValueError:
+
+                        continue
+
+            elif self.n_jobs >= 2 or self.n_jobs == -1:  # parallel optimization
+
+                def foo(i):
+
+                    gp_opt_obj = GPOpt(
+                        objective_func=self.objective_func,
+                        lower_bound=self.lower_bound,
+                        upper_bound=self.upper_bound,
+                        n_init=self.n_init,
+                        n_iter=self.n_iter,
+                        alpha=self.alpha,
+                        n_restarts_optimizer=self.n_restarts_optimizer,
+                        seed=self.seed,
+                        n_jobs=self.n_jobs,
+                        acquisition=self.acquisition,
+                        min_value=self.min_value,
+                        surrogate_obj=copy.deepcopy(self.regressors[i][1]),
+                    )
+
+                    try:
+                        gp_opt_obj.optimize(
+                            verbose=0,  # important
+                            abs_tol=abs_tol,  # suggested 1e-4, for n_iter = 200
+                            min_budget=min_budget,  # minimum budget for early stopping
+                            func_args=func_args,
+                            method=method,
+                        )
+
+                        return gp_opt_obj
+                    except ValueError:
+                        return None
+
+                tmp_results = Parallel(n_jobs=self.n_jobs)(
+                    delayed(foo)(i) for i in tqdm(range(len(self.regressors)))
+                )
+
+                for i in tqdm(range(len(tmp_results))):
+
+                    if tmp_results[i] is not None:
+
+                        gp_opt_obj = copy.deepcopy(tmp_results[i])
+
+                        score_next_param = gp_opt_obj.y_min
+
+                        if score_next_param < self.y_min:
+                            self.x_min = gp_opt_obj.x_min
+                            self.y_min = score_next_param
+                            self.best_surrogate = copy.deepcopy(
+                                gp_opt_obj.surrogate_obj
+                            )
+                            if self.y_min == self.min_value:
+                                break
+
+                        if verbose == 2:
+                            print(f"Global iteration #{i + 1} -----")
+                            print(f"current minimum:  {self.x_min}")
+                            print(f"current minimum score:  {self.y_min}")
+                            print(
+                                f"score for next parameter: {score_next_param} \n"
+                            )
+
+                    else:
+
+                        continue
+
+            else:
+                raise ValueError(
+                    "n_jobs must be either None or >= 2 or equal to -1"
+                )
+            return DescribeResult(self.x_min, self.y_min, self.best_surrogate)
+
+        else:
+
+            NotImplementedError(
+                "type_exec must be either 'queue' or 'independent'"
+            )
```

### Comparing `GPopt-0.4.1/GPopt/utils/nodesimulation.py` & `gpopt-0.6.0/GPopt/utils/nodesimulation.py`

 * *Files identical despite different names*

### Comparing `GPopt-0.4.1/GPopt/utils/progress_bar.py` & `gpopt-0.6.0/GPopt/utils/progress_bar.py`

 * *Files identical despite different names*

### Comparing `GPopt-0.4.1/GPopt/utils/sobol_lib.py` & `gpopt-0.6.0/GPopt/utils/sobol_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -14694,15 +14694,15 @@
             16273,
             16299,
             16309,
             16355,
             16375,
             16381,
         ]
-        atmost = 2 ** log_max - 1
+        atmost = 2**log_max - 1
         #
         # 	Find the number of bits in ATMOST.
         #
         maxcol = i4_bit_hi1(atmost)
         #
         # 	Initialize row 1 of V.
         #
```

### Comparing `GPopt-0.4.1/GPopt.egg-info/PKG-INFO` & `gpopt-0.6.0/GPopt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: GPopt
-Version: 0.4.1
+Version: 0.6.0
 Summary: Bayesian Optimization using Gaussian Process Regression
 Home-page: https://github.com/thierrymoudiki/GPopt
-Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.4.1
+Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.6.0
 Author: Thierry Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: matplotlib
+Requires-Dist: nnetsauce
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: threadpoolctl
+Requires-Dist: tqdm
 
 Bayesian Optimization using Gaussian Process Regression
```

### Comparing `GPopt-0.4.1/LICENSE` & `gpopt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GPopt-0.4.1/PKG-INFO` & `gpopt-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: GPopt
-Version: 0.4.1
+Version: 0.6.0
 Summary: Bayesian Optimization using Gaussian Process Regression
 Home-page: https://github.com/thierrymoudiki/GPopt
-Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.4.1
+Download-URL: https://github.com/thierrymoudiki/GPopt/tarball/0.6.0
 Author: Thierry Moudiki
 Author-email: thierry.moudiki@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 Requires-Dist: joblib
 Requires-Dist: matplotlib
+Requires-Dist: nnetsauce
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: threadpoolctl
+Requires-Dist: tqdm
 
 Bayesian Optimization using Gaussian Process Regression
```

### Comparing `GPopt-0.4.1/README.md` & `gpopt-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 GPopt
 ===============================
 
 Bayesian Optimization using Gaussian Process Regression
 
 
 
-![PyPI](https://img.shields.io/pypi/v/gpopt) [![PyPI - License](https://img.shields.io/pypi/l/gpopt)](./LICENSE) [![Downloads](https://pepy.tech/badge/gpopt)](https://pepy.tech/project/gpopt) [![HitCount](https://hits.dwyl.com/Techtonique/GPopt.svg?style=flat-square)](http://hits.dwyl.com/Techtonique/GPopt) [![CodeFactor](https://www.codefactor.io/repository/github/techtonique/gpopt/badge/main)](https://www.codefactor.io/repository/github/techtonique/gpopt/overview/main) [![Documentation](https://img.shields.io/badge/documentation-is_here-green)](https://techtonique.github.io/GPopt/)
+![PyPI](https://img.shields.io/pypi/v/gpopt) [![PyPI - License](https://img.shields.io/pypi/l/gpopt)](./LICENSE) [![Downloads](https://pepy.tech/badge/gpopt)](https://pepy.tech/project/gpopt) [![HitCount](https://hits.dwyl.com/Techtonique/GPopt.svg?style=flat-square)](http://hits.dwyl.com/Techtonique/GPopt)
+[![CodeFactor](https://www.codefactor.io/repository/github/techtonique/gpopt/badge)](https://www.codefactor.io/repository/github/techtonique/gpopt)
+[![Documentation](https://img.shields.io/badge/documentation-is_here-green)](https://techtonique.github.io/GPopt/)
 
 Installation / Usage
 --------------------
 
 To install use pip:
 
     $ pip install GPopt
```

### Comparing `GPopt-0.4.1/setup.py` & `gpopt-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import subprocess
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "0.4.1"
+__version__ = "0.6.0"
 
 subprocess.call("pip install -r requirements.txt", shell=True)
 
 here = path.abspath(path.dirname(__file__))
 
 # get the dependencies and installs
 with open(
```

