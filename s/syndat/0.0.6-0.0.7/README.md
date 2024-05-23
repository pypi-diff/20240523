# Comparing `tmp/syndat-0.0.6.tar.gz` & `tmp/syndat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndat-0.0.6.tar", last modified: Tue May 21 13:54:21 2024, max compression
+gzip compressed data, was "syndat-0.0.7.tar", last modified: Wed May 22 13:17:43 2024, max compression
```

## Comparing `syndat-0.0.6.tar` & `syndat-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 13:54:17.000000 syndat-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 13:54:21.503998 syndat-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-21 13:54:17.000000 syndat-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:54:21.503998 syndat-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-21 13:54:19.000000 syndat-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/syndat/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/syndat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_jsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:17:43.090404 syndat-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-22 13:17:38.000000 syndat-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:17:43.090404 syndat-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-22 13:17:38.000000 syndat-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:17:43.090404 syndat-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 13:17:41.000000 syndat-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:17:43.090404 syndat-0.0.7/syndat/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 13:17:38.000000 syndat-0.0.7/syndat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-22 13:17:38.000000 syndat-0.0.7/syndat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-22 13:17:38.000000 syndat-0.0.7/syndat/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-22 13:17:38.000000 syndat-0.0.7/syndat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:17:43.090404 syndat-0.0.7/syndat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 13:17:43.000000 syndat-0.0.7/syndat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-22 13:17:43.000000 syndat-0.0.7/syndat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:17:43.000000 syndat-0.0.7/syndat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:17:43.000000 syndat-0.0.7/syndat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:17:43.090404 syndat-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-22 13:17:38.000000 syndat-0.0.7/tests/test_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-22 13:17:38.000000 syndat-0.0.7/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-22 13:17:38.000000 syndat-0.0.7/tests/test_jsd.py
```

### Comparing `syndat-0.0.6/LICENSE` & `syndat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syndat-0.0.6/README.md` & `syndat-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `syndat-0.0.6/setup.py` & `syndat-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='syndat',
-    version='v0.0.6',
+    version='v0.0.7',
     packages=['syndat'],
     url='https://github.com/SCAI-BIO/syndat',
     license='CC BY-NC-ND 4.0.',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `syndat-0.0.6/syndat/quality.py` & `syndat-0.0.7/syndat/quality.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,19 @@
         col_dtype_synthetic = synthetic[col].dtype
         if col_dtype_real != col_dtype_synthetic:
             logging.warning(f'Real data at col {col} is dtype {col_dtype_real} but synthetic is {col_dtype_synthetic}. '
                             f'Evaluation will be done based on the assumed data type of the real data.')
             for col_synth in synthetic.columns:
                 synthetic[col_synth] = synthetic[col_synth].astype(real[col_synth].dtype)
         if col_dtype_real == "int64" or col_dtype_real == "object":
+            # handle negative values for bincount -> shift all codes to positive (will yield same result in JSD)
+            min_value = min(real[col].min(), synthetic[col].min())
+            if min_value < 0:
+                real[col] = real[col] + abs(min_value)
+                synthetic[col] = synthetic[col] + abs(min_value)
             # categorical column
             real_binned = np.bincount(real[col])
             virtual_binned = np.bincount(synthetic[col])
         else:
             # get optimal amount of bins
             n_bins = np.histogram_bin_edges(real_wo_missing, bins='auto')
             real_binned = np.bincount(np.digitize(real_wo_missing, n_bins))
```

### Comparing `syndat-0.0.6/syndat/visualization.py` & `syndat-0.0.7/syndat/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,14 @@
     :param synthetic: The synthetic data
     :param store_destination: Path to the folder where the results should be stored.
     """
     names = ["real_corr", "syntehtic_corr"]
     for idx, patient_type in enumerate([real, synthetic]):
         plt.figure()
         plt.title("Correlation")
-        ax = sns.heatmap(patient_type.corr())
+        ax = sns.heatmap(patient_type.corr(), vmin=-1, vmax=1)
         fig = ax.get_figure()
         fig.savefig(store_destination + "/" + names[idx] + '.png', bbox_inches="tight")
```

### Comparing `syndat-0.0.6/tests/test_auc.py` & `syndat-0.0.7/tests/test_auc.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.6/tests/test_correlation.py` & `syndat-0.0.7/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.6/tests/test_jsd.py` & `syndat-0.0.7/tests/test_jsd.py`

 * *Files identical despite different names*

