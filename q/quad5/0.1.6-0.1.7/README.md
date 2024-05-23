# Comparing `tmp/quad5-0.1.6.tar.gz` & `tmp/quad5-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quad5-0.1.6.tar", last modified: Wed May 22 16:02:51 2024, max compression
+gzip compressed data, was "quad5-0.1.7.tar", last modified: Thu May 23 09:35:45 2024, max compression
```

## Comparing `quad5-0.1.6.tar` & `quad5-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:02:51.009699 quad5-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 16:02:16.000000 quad5-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-22 16:02:51.009699 quad5-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-22 16:02:16.000000 quad5-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:02:51.009699 quad5-0.1.6/quad5/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 16:02:16.000000 quad5-0.1.6/quad5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-22 16:02:16.000000 quad5-0.1.6/quad5/quadratic_approximation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:02:51.009699 quad5-0.1.6/quad5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-22 16:02:51.000000 quad5-0.1.6/quad5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-22 16:02:51.000000 quad5-0.1.6/quad5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:02:51.000000 quad5-0.1.6/quad5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 16:02:51.000000 quad5-0.1.6/quad5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 16:02:51.000000 quad5-0.1.6/quad5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 16:02:51.013699 quad5-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-22 16:02:16.000000 quad5-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:35:45.195410 quad5-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 09:35:08.000000 quad5-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-23 09:35:45.195410 quad5-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-23 09:35:08.000000 quad5-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:35:45.191410 quad5-0.1.7/quad5/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 09:35:08.000000 quad5-0.1.7/quad5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 09:35:08.000000 quad5-0.1.7/quad5/quadratic_approximation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:35:45.195410 quad5-0.1.7/quad5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-23 09:35:45.000000 quad5-0.1.7/quad5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 09:35:45.000000 quad5-0.1.7/quad5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:35:45.000000 quad5-0.1.7/quad5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 09:35:45.000000 quad5-0.1.7/quad5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 09:35:45.000000 quad5-0.1.7/quad5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 09:35:45.195410 quad5-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-23 09:35:08.000000 quad5-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:35:45.195410 quad5-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 09:35:08.000000 quad5-0.1.7/tests/test.py
```

### Comparing `quad5-0.1.6/LICENSE` & `quad5-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quad5-0.1.6/PKG-INFO` & `quad5-0.1.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,36 @@
-Metadata-Version: 2.1
-Name: quad5
-Version: 0.1.6
-Summary: Quadratic Approximation custom step sampler for PYMC.
-Home-page: https://github.com/carsten-j/quad5
-Author: Carsten Jørgensen
-Author-email: carstenj@gmail.com
-License: MIT
-Keywords: Bayesian Statistics,Probabalistic Programming Language,Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: PYMC==5.15.0
-
 # Quadratic Approximation
 
 Modern Bayesian data analysis is based on efficient Markov Chain Monte Carlo (MCMC) techniques. 
 
 Learning Bayesian statistic can be hard for a Frequentist! The [Statistical Rethinking](https://xcelab.net/rm/) book by Richard McElreath tries to avoid cognitive overload for its readers by not requireing them to learn Bayesian statistics and MCMC at the same time. The posterior distribution is in most interesting cases analytically intractable and hence MCMC is used to numerically determine it.
 
 As a simpler alternative to MCMC one can you Quadratic Approximation[^1]. A lot of people has ported the R code examples from Statistical Rethinking to Python using frameworks like PYMC, Pyro, NumPyro, and TensorFlow Probability. Apparently there is no Quadratic Approximation solution available for PYMC[^2]. Numpyro has [AutoLaplaceApproximation](https://num.pyro.ai/en/latest/autoguide.html#numpyro.infer.autoguide.AutoLaplaceApproximation)[^3] but it is not clear to me that this is the same as Quadratic Approximation.
 
 quad5 leverages [PYMC](https://www.pymc.io/welcome.html) and works by adding a custom step for the sample method on PYMC models. By doing so it benefits from standard PYMC functionality that automatically adds constant, deterministic, and observed data to the 
 [inferencedata](https://python.arviz.org/en/stable/getting_started/WorkingWithInferenceData.html) output from the sample method. This allows for easy usage of the [Arviz](https://www.arviz.org/en/latest/) visualization library for posterior distributions and more general the ecosystem around PYMC.
 
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
-I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit eihter PR's or createa issue for such cases.
+I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
+``` python
+        y = np.array([2642, 3503, 4358], dtype=np.float64)
 
+        with pm.Model() as m:
+            logsigma = pm.Uniform("logsigma", 1, 100)
+            mu = pm.Uniform("mu", 0, 10000)
+            _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
+            custom_step = QuadraticApproximation([mu, logsigma], m)
+            trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+```
 
-add photo of model
-
-and summary
-
-See more examples ...
+See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
-[^1]: The Bernstein-Von Mises Theorem states that under some regularity conditions 
-the posterior distribution is asymptotically normal. Unimodal , most of the probability mass is located symmetric around the peak
+[^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
-[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC.
+[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
-[^3]:foo
+[^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
+of variational inference of the posterior distribution.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `quad5-0.1.6/README.md` & `quad5-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,52 @@
+Metadata-Version: 2.1
+Name: quad5
+Version: 0.1.7
+Summary: Quadratic Approximation custom step sampler for PYMC.
+Home-page: https://github.com/carsten-j/quad5
+Author: Carsten Jørgensen
+Author-email: carstenj@gmail.com
+License: MIT
+Keywords: Bayesian Statistics,Probabalistic Programming Language,Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: PYMC==5.15.0
+
 # Quadratic Approximation
 
 Modern Bayesian data analysis is based on efficient Markov Chain Monte Carlo (MCMC) techniques. 
 
 Learning Bayesian statistic can be hard for a Frequentist! The [Statistical Rethinking](https://xcelab.net/rm/) book by Richard McElreath tries to avoid cognitive overload for its readers by not requireing them to learn Bayesian statistics and MCMC at the same time. The posterior distribution is in most interesting cases analytically intractable and hence MCMC is used to numerically determine it.
 
 As a simpler alternative to MCMC one can you Quadratic Approximation[^1]. A lot of people has ported the R code examples from Statistical Rethinking to Python using frameworks like PYMC, Pyro, NumPyro, and TensorFlow Probability. Apparently there is no Quadratic Approximation solution available for PYMC[^2]. Numpyro has [AutoLaplaceApproximation](https://num.pyro.ai/en/latest/autoguide.html#numpyro.infer.autoguide.AutoLaplaceApproximation)[^3] but it is not clear to me that this is the same as Quadratic Approximation.
 
 quad5 leverages [PYMC](https://www.pymc.io/welcome.html) and works by adding a custom step for the sample method on PYMC models. By doing so it benefits from standard PYMC functionality that automatically adds constant, deterministic, and observed data to the 
 [inferencedata](https://python.arviz.org/en/stable/getting_started/WorkingWithInferenceData.html) output from the sample method. This allows for easy usage of the [Arviz](https://www.arviz.org/en/latest/) visualization library for posterior distributions and more general the ecosystem around PYMC.
 
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
-I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit eihter PR's or createa issue for such cases.
+I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
+``` python
+        y = np.array([2642, 3503, 4358], dtype=np.float64)
 
+        with pm.Model() as m:
+            logsigma = pm.Uniform("logsigma", 1, 100)
+            mu = pm.Uniform("mu", 0, 10000)
+            _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
+            custom_step = QuadraticApproximation([mu, logsigma], m)
+            trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+```
 
-add photo of model
-
-and summary
-
-See more examples ...
+See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
-[^1]: The Bernstein-Von Mises Theorem states that under some regularity conditions 
-the posterior distribution is asymptotically normal. Unimodal , most of the probability mass is located symmetric around the peak
+[^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
-[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC.
+[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
-[^3]:foo
+[^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
+of variational inference of the posterior distribution.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quad5-0.1.6/quad5/quadratic_approximation.py` & `quad5-0.1.7/quad5/quadratic_approximation.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import numpy as np
 import pymc as pm
+import scipy.stats as st
 from pymc.step_methods.arraystep import ArrayStep
 from pymc.util import get_value_vars_from_user_vars
 
 
 class QuadraticApproximation(ArrayStep):
-    def __init__(self, vars, model, **kwargs):
+    def __init__(self, vars, model, start=None, **kwargs):
         self.model = model
         self.vars = vars
         self.varnames = [var.name for var in vars]
 
-        # Compute mode and covariance
-        self.mode, self.covariance = self._compute_mode_and_covariance()
+        self.mode, self.covariance = self._compute_mode_and_covariance(start)
 
         vars = get_value_vars_from_user_vars(vars, model)
 
-        # Create necessary function sets for pymc
         super().__init__(vars, [self._logp_fn], **kwargs)
 
     def _point_to_array(self, point):
         return np.array([point[varname] for varname in self.varnames])
 
     def _array_to_point(self, array):
         return {varname: val for varname, val in zip(self.varnames, array)}
 
     def _logp_fn(self, x):
         point = self._array_to_point(x)
         return self.model.logp(point)
 
-    def _compute_mode_and_covariance(self):
-        # Find the MAP estimate (mode of the posterior)
-        map = pm.find_MAP(vars=self.vars)
+    def _compute_mode_and_covariance(self, start=None):
+
+        map = pm.find_MAP(vars=self.vars, start=start)
 
         m = pm.modelcontext(None)
 
         for var in self.vars:
             if m.rvs_to_transforms[var] is not None:
                 m.rvs_to_transforms[var] = None
-                # change name so that we can use `map[var]` value
                 var_value = m.rvs_to_values[var]
                 var_value.name = var.name
 
         H = pm.find_hessian(map, vars=self.vars)
         cov = np.linalg.inv(H)
         mean = np.concatenate([np.atleast_1d(map[v.name]) for v in self.vars])
 
         return mean, cov
 
     def astep(self, q0, logp):
-        # Generate a sample from the multivariate Gaussian approximation
         sample = np.random.multivariate_normal(self.mode, self.covariance)
         return sample, []
+
+    def posterior(self):
+        return st.multivariate_normal(mean=self.mean, cov=self.covariance)
```

### Comparing `quad5-0.1.6/quad5.egg-info/PKG-INFO` & `quad5-0.1.7/quad5.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quad5
-Version: 0.1.6
+Version: 0.1.7
 Summary: Quadratic Approximation custom step sampler for PYMC.
 Home-page: https://github.com/carsten-j/quad5
 Author: Carsten Jørgensen
 Author-email: carstenj@gmail.com
 License: MIT
 Keywords: Bayesian Statistics,Probabalistic Programming Language,Python
 Classifier: Programming Language :: Python :: 3
@@ -24,24 +24,29 @@
 
 quad5 leverages [PYMC](https://www.pymc.io/welcome.html) and works by adding a custom step for the sample method on PYMC models. By doing so it benefits from standard PYMC functionality that automatically adds constant, deterministic, and observed data to the 
 [inferencedata](https://python.arviz.org/en/stable/getting_started/WorkingWithInferenceData.html) output from the sample method. This allows for easy usage of the [Arviz](https://www.arviz.org/en/latest/) visualization library for posterior distributions and more general the ecosystem around PYMC.
 
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
-I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit eihter PR's or createa issue for such cases.
+I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
+``` python
+        y = np.array([2642, 3503, 4358], dtype=np.float64)
 
+        with pm.Model() as m:
+            logsigma = pm.Uniform("logsigma", 1, 100)
+            mu = pm.Uniform("mu", 0, 10000)
+            _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
+            custom_step = QuadraticApproximation([mu, logsigma], m)
+            trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+```
 
-add photo of model
+See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
-and summary
+[^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
-See more examples ...
+[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
-[^1]: The Bernstein-Von Mises Theorem states that under some regularity conditions 
-the posterior distribution is asymptotically normal. Unimodal , most of the probability mass is located symmetric around the peak
-
-[^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC.
-
-[^3]:foo
+[^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
+of variational inference of the posterior distribution.
```

### Comparing `quad5-0.1.6/setup.py` & `quad5-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="quad5",
-    version="0.1.6",
+    version="0.1.7",
     description="""Quadratic Approximation custom step sampler for PYMC.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Carsten Jørgensen",
     packages=find_packages(include=["quad5"]),
     keywords=["Bayesian Statistics", "Probabalistic Programming Language", "Python"],
     classifiers=[
```

