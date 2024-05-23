# Comparing `tmp/pgscatalog_calc-0.1.0.tar.gz` & `tmp/pgscatalog_calc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_calc-0.1.0.tar", max compression
+gzip compressed data, was "pgscatalog_calc-0.1.1.tar", max compression
```

## Comparing `pgscatalog_calc-0.1.0.tar` & `pgscatalog_calc-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1888 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/README.md
--rw-r--r--   0        0        0      962 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      485 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/__init__.py
--rw-r--r--   0        0        0       70 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/cli/__init__.py
--rw-r--r--   0        0        0     2483 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/cli/aggregate_cli.py
--rw-r--r--   0        0        0     5925 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/cli/ancestry_cli.py
--rw-r--r--   0        0        0      512 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_ancestry/__init__.py
--rw-r--r--   0        0        0     3182 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_ancestry/read.py
--rw-r--r--   0        0        0    28254 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_ancestry/tools.py
--rw-r--r--   0        0        0      114 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_config.py
--rw-r--r--   0        0        0    16504 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/polygenicscore.py
--rw-r--r--   0        0        0     5778 2024-03-22 15:00:16.066641 pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/principalcomponents.py
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pgscatalog_calc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1888 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/README.md
+-rw-r--r--   0        0        0     1033 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      508 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/__init__.py
+-rw-r--r--   0        0        0       70 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/cli/__init__.py
+-rw-r--r--   0        0        0     2483 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/cli/aggregate_cli.py
+-rw-r--r--   0        0        0     5925 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/cli/ancestry_cli.py
+-rw-r--r--   0        0        0      512 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_ancestry/__init__.py
+-rw-r--r--   0        0        0     3182 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_ancestry/read.py
+-rw-r--r--   0        0        0    28231 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_ancestry/tools.py
+-rw-r--r--   0        0        0      114 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_config.py
+-rw-r--r--   0        0        0    17188 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/polygenicscore.py
+-rw-r--r--   0        0        0     5778 2024-05-23 15:04:18.533888 pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/principalcomponents.py
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 pgscatalog_calc-0.1.1/PKG-INFO
```

### Comparing `pgscatalog_calc-0.1.0/README.md` & `pgscatalog_calc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/pyproject.toml` & `pgscatalog_calc-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pgscatalog.calc"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Libraries and applications for working with calculated polygenic scores"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 readme = "README.md"
 packages = [
     { include = "pgscatalog", from = "src" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/cli/aggregate_cli.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/cli/aggregate_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/cli/ancestry_cli.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/cli/ancestry_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/__init__.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_ancestry/read.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_ancestry/read.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/_ancestry/tools.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/_ancestry/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,18 +335,18 @@
         # Makes melting easier later
         sum_col = "SUM|{}".format(c_pgs)
         results_ref[sum_col] = ref_df[c_pgs]
         results_target[sum_col] = target_df[c_pgs]
         results_models = {}
 
         # Check that PGS has variance (e.g. not all 0)
-        if 0 in [np.var(results_ref[sum_col]), np.var(results_target[sum_col])]:
+        if np.var(results_ref[sum_col]) == 0:
             scorecols_drop.add(c_pgs)
             logger.warning(
-                "Skipping adjustment: {} has 0 variance in PGS SUM".format(c_pgs)
+                "Skipping adjustment: {} has 0 variance in PGS SUM [REFERENCE]".format(c_pgs)
             )
 
     # Report PGS values with respect to distribution of PGS in the most similar reference population
     if "empirical" in use_method:
         logger.debug(
             "Adjusting PGS using most similar reference population distribution."
         )
```

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/polygenicscore.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/polygenicscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -379,23 +379,37 @@
         df.index.names = ["sampleset", "IID"]
         df = df[_select_agg_cols(df.columns)]
         return df
 
     def write(self, outdir, split=False, melt=True):
         """Write PGS to a compressed TSV"""
         outdir = pathlib.Path(outdir)
-        for chunk in self:
+        for i, chunk in enumerate(self):
+            chunk = PolygenicScore(df=chunk, sampleset=self.sampleset)
+
             if melt:
-                chunk = _melt(chunk, "SUM")
+                logger.info(f"Melting chunk {i}")
+                chunk = chunk.melt()
+            else:
+                logger.info(f"Preparing chunk {i}")
+                # don't do anything, just materialise the df generator
+                chunk = pd.concat(chunk.df, axis=0)
 
+            logger.info(f"Writing chunk {i}")
             if split:
+                if i == 0:
+                    logger.info("Writing results split by sampleset")
+
                 for sampleset, group in chunk.groupby("sampleset"):
                     fout = outdir / f"{sampleset}_pgs.txt.gz"
                     chunk.to_csv(fout, sep="\t", compression="gzip", mode="a")
             else:
+                if i == 0:
+                    logger.info("Writing combined results (aggregated_scores.txt.gz)")
+
                 fout = outdir / "aggregated_scores.txt.gz"
                 chunk.to_csv(fout, sep="\t", compression="gzip", mode="a")
 
     def average(self):
         """Recalculate average.
 
         This is an eager operation, and immediately returns a dataframe
@@ -409,15 +423,17 @@
             chunk_list.append(avgs)
         return pd.concat(chunk_list, axis=0)
 
     def melt(self):
         """Melt dataframe from wide format to long format"""
         sum_df = _melt(pd.concat(self.df, axis=0), value_name="SUM")
         avg_df = _melt(self.average(), value_name="AVG")
-        return pd.concat([sum_df, avg_df.AVG], axis=1)
+        df = pd.concat([sum_df, avg_df.AVG], axis=1)
+        # melted chunks need a consistent column order
+        return df[["PGS", "SUM", "DENOM", "AVG"]]
 
 
 def _select_agg_cols(cols):
     """Select aggregatable columns"""
     keep_cols = ["DENOM"]
     return [
         x
```

### Comparing `pgscatalog_calc-0.1.0/src/pgscatalog/calc/lib/principalcomponents.py` & `pgscatalog_calc-0.1.1/src/pgscatalog/calc/lib/principalcomponents.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_calc-0.1.0/PKG-INFO` & `pgscatalog_calc-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pgscatalog.calc
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Libraries and applications for working with calculated polygenic scores
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

