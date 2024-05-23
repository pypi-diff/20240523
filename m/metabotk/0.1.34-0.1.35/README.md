# Comparing `tmp/metabotk-0.1.34.tar.gz` & `tmp/metabotk-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabotk-0.1.34.tar", max compression
+gzip compressed data, was "metabotk-0.1.35.tar", max compression
```

## Comparing `metabotk-0.1.34.tar` & `metabotk-0.1.35.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0      138 2024-04-11 07:38:28.279469 metabotk-0.1.34/README.md
--rw-r--r--   0        0        0      430 2024-05-08 10:19:59.019797 metabotk-0.1.34/metabotk/__init__.py
--rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.34/metabotk/cli.py
--rw-r--r--   0        0        0    25645 2024-05-08 10:52:37.591242 metabotk-0.1.34/metabotk/dataset_manager.py
--rw-r--r--   0        0        0     2385 2024-05-06 14:27:57.915425 metabotk-0.1.34/metabotk/dimensionality_reduction.py
--rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.34/metabotk/feature_selection.py
--rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.34/metabotk/imputation.py
--rw-r--r--   0        0        0     6549 2024-05-10 08:47:44.397753 metabotk-0.1.34/metabotk/interface.py
--rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.34/metabotk/missing_handler.py
--rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.34/metabotk/models_handler.py
--rw-r--r--   0        0        0     5834 2024-05-10 14:35:55.026236 metabotk-0.1.34/metabotk/normalization.py
--rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.34/metabotk/outliers_handler.py
--rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.34/metabotk/providers_handler.py
--rw-r--r--   0        0        0     9052 2024-05-03 16:08:37.603788 metabotk-0.1.34/metabotk/statistics_handler.py
--rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.34/metabotk/utils.py
--rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.34/metabotk/visualization_handler.py
--rw-r--r--   0        0        0      716 2024-05-10 15:50:44.645762 metabotk-0.1.34/pyproject.toml
--rw-r--r--   0        0        0     1051 1970-01-01 00:00:00.000000 metabotk-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0     2184 2024-05-23 10:36:38.955800 metabotk-0.1.35/README.md
+-rw-r--r--   0        0        0      531 2024-05-23 10:28:10.899057 metabotk-0.1.35/metabotk/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-23 10:38:44.289244 metabotk-0.1.35/metabotk/_version.py
+-rwxr-xr-x   0        0        0    13804 2024-04-30 08:47:50.191430 metabotk-0.1.35/metabotk/cli.py
+-rw-r--r--   0        0        0    26255 2024-05-23 10:33:39.163099 metabotk-0.1.35/metabotk/dataset_manager.py
+-rw-r--r--   0        0        0     2388 2024-05-21 18:11:30.585916 metabotk-0.1.35/metabotk/dimensionality_reduction.py
+-rw-r--r--   0        0        0     6455 2024-05-07 14:31:53.501469 metabotk-0.1.35/metabotk/feature_selection.py
+-rw-r--r--   0        0        0     2543 2024-05-08 11:21:56.531467 metabotk-0.1.35/metabotk/imputation.py
+-rw-r--r--   0        0        0     6549 2024-05-12 14:39:51.768689 metabotk-0.1.35/metabotk/interface.py
+-rw-r--r--   0        0        0     5007 2024-05-07 11:52:22.276298 metabotk-0.1.35/metabotk/missing_handler.py
+-rw-r--r--   0        0        0     2761 2024-04-16 18:00:17.034722 metabotk-0.1.35/metabotk/models_handler.py
+-rw-r--r--   0        0        0     6051 2024-05-17 13:37:46.018747 metabotk-0.1.35/metabotk/normalization.py
+-rw-r--r--   0        0        0     3277 2024-04-30 14:59:52.276566 metabotk-0.1.35/metabotk/outliers_handler.py
+-rw-r--r--   0        0        0     5527 2024-05-08 10:50:11.939978 metabotk-0.1.35/metabotk/providers_handler.py
+-rw-r--r--   0        0        0     9052 2024-05-23 10:29:17.747712 metabotk-0.1.35/metabotk/statistics_handler.py
+-rw-r--r--   0        0        0     3235 2024-04-30 15:27:18.722846 metabotk-0.1.35/metabotk/utils.py
+-rw-r--r--   0        0        0     4658 2024-05-10 15:46:25.623360 metabotk-0.1.35/metabotk/visualization_handler.py
+-rw-r--r--   0        0        0      735 2024-05-23 10:38:52.105569 metabotk-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0     3137 1970-01-01 00:00:00.000000 metabotk-0.1.35/PKG-INFO
```

### Comparing `metabotk-0.1.34/metabotk/cli.py` & `metabotk-0.1.35/metabotk/cli.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/dataset_manager.py` & `metabotk-0.1.35/metabotk/dataset_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,7 +632,29 @@
         pandas.DataFrame
             Extracted chemical annotations for the specified metabolites.
         """
         if not isinstance(metabolites_to_extract, list):
             metabolites_to_extract = [metabolites_to_extract]
         # convert to string to match the CHEM_ID column in chemical_annotation
         return self.chemical_annotation.loc[[str(i) for i in metabolites_to_extract]]
+
+    def sort_samples(self, by, ascending=True):
+        """
+        Sort samples in the dataset.
+
+        Parameters
+        ----------
+        by : str
+            Column name to sort by.
+        ascending : bool, optional
+            If True, sort in ascending order, by default True
+
+        Returns
+        -------
+        pandas.DataFrame
+            Sorted dataset
+        """
+        self.sample_metadata = self.sample_metadata.sort_values(
+            by=by, ascending=ascending
+        )
+        self.data = self.data.loc[self.sample_metadata.index]
+        self.samples = self.sample_metadata.index
```

### Comparing `metabotk-0.1.34/metabotk/dimensionality_reduction.py` & `metabotk-0.1.35/metabotk/dimensionality_reduction.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         # Perform PCA
         pca = PCA(n_components=n_components).fit(scaled_data)
 
         # Transform data
         pca_transformed = pd.DataFrame(
             pca.transform(scaled_data),
             columns=[f"PC{i}" for i in range(1, n_components + 1)],
-            index=self.data_manager.samples,
+            index=self.data_manager.data.index,
         )
 
         # Concatenate with sample metadata
         pca_transformed = self.data_manager.sample_metadata.merge(
             pca_transformed, left_index=True, right_index=True
         )
         if get_pca_object == True:
```

### Comparing `metabotk-0.1.34/metabotk/feature_selection.py` & `metabotk-0.1.35/metabotk/feature_selection.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/imputation.py` & `metabotk-0.1.35/metabotk/imputation.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/interface.py` & `metabotk-0.1.35/metabotk/interface.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/missing_handler.py` & `metabotk-0.1.35/metabotk/missing_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/models_handler.py` & `metabotk-0.1.35/metabotk/models_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/normalization.py` & `metabotk-0.1.35/metabotk/normalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import pyserrf as srf
+from skloess import LOESS
 
 
 class NormalizationHandler:
     """
     Class for performing normalization on metabolomics data.
 
     This class provides a simple interface to perform normalization on the data using various approaches.
     For now only SERRF is included.
     """
 
     def __init__(
         self,
-        # dataset_manager,
+        dataset_manager,
     ):
         """
         Initialize the class.
         """
-        # self._dataset_manager = dataset_manager
+        self._dataset_manager = dataset_manager
 
     def serrf(
         self,
         dataset,
         sample_type_column="measurement_group",
         batch_column="batch",
         time_column="time",
@@ -136,7 +137,13 @@
             time_column=time_column,
             other_columns=other_columns,
             n_correlated_metabolites=n_correlated_metabolites,
             random_state=random_state,
             threads=threads,
         )
         return raw_variations, normalized_variations
+
+    def loess_single_metabolite_single_batch(
+        self, metabolite_qc, metabolite_samples, degree, smoothing
+    ):
+        est = LOESS(degree=degree, smoothing=smoothing)
+        est.fit()
```

### Comparing `metabotk-0.1.34/metabotk/outliers_handler.py` & `metabotk-0.1.35/metabotk/outliers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/providers_handler.py` & `metabotk-0.1.35/metabotk/providers_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/statistics_handler.py` & `metabotk-0.1.35/metabotk/statistics_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/utils.py` & `metabotk-0.1.35/metabotk/utils.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/metabotk/visualization_handler.py` & `metabotk-0.1.35/metabotk/visualization_handler.py`

 * *Files identical despite different names*

### Comparing `metabotk-0.1.34/pyproject.toml` & `metabotk-0.1.35/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabotk"
-version = "0.1.34"
+version = "0.1.35"
 description = "Python toolkit for working with metabolomics data"
 authors = ["matteobolner <matteo.bolner2@unibo.it>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4"
 requests = "^2.31.0"
@@ -14,14 +14,15 @@
 scikit-learn = "^1.4.2"
 seaborn = "^0.13.2"
 statsmodels = "^0.14.1"
 dill = "^0.3.8"
 boruta-py-versioned = "^0.1.0"
 sphinx-rtd-theme = "^2.0.0"
 pyserrf = "^0.1.5"
+skloess = "^0.1.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">7.0"
```

