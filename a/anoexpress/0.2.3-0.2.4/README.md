# Comparing `tmp/anoexpress-0.2.3.tar.gz` & `tmp/anoexpress-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoexpress-0.2.3.tar", max compression
+gzip compressed data, was "anoexpress-0.2.4.tar", max compression
```

## Comparing `anoexpress-0.2.3.tar` & `anoexpress-0.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2024-01-09 09:49:40.711594 anoexpress-0.2.3/LICENSE
--rw-r--r--   0        0        0     4129 2024-01-09 09:49:40.711594 anoexpress-0.2.3/README.md
--rw-r--r--   0        0        0       66 2024-01-09 09:49:40.711594 anoexpress-0.2.3/anoexpress/__init__.py
--rw-r--r--   0        0        0    44357 2024-01-09 09:49:40.711594 anoexpress-0.2.3/anoexpress/anoexpress.py
--rw-r--r--   0        0        0     1002 2024-01-09 09:49:55.279702 anoexpress-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 anoexpress-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-23 12:45:19.117514 anoexpress-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4129 2024-05-23 12:45:19.117514 anoexpress-0.2.4/README.md
+-rw-r--r--   0        0        0       66 2024-05-23 12:45:19.117514 anoexpress-0.2.4/anoexpress/__init__.py
+-rw-r--r--   0        0        0    47347 2024-05-23 12:45:19.117514 anoexpress-0.2.4/anoexpress/anoexpress.py
+-rw-r--r--   0        0        0     1041 2024-05-23 12:45:33.177416 anoexpress-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 anoexpress-0.2.4/PKG-INFO
```

### Comparing `anoexpress-0.2.3/LICENSE` & `anoexpress-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anoexpress-0.2.3/README.md` & `anoexpress-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `anoexpress-0.2.3/anoexpress/anoexpress.py` & `anoexpress-0.2.4/anoexpress/anoexpress.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import pandas as pd
 import numpy as np
+from tqdm.notebook import tqdm
 
 taxon_query_dict = { 'gamb_colu':"species in ['gambiae','coluzzii']", 
                   'gamb_colu_arab':"species in ['gambiae','coluzzii','arabiensis']", 
                   'gamb_colu_arab_fun':"species in ['gambiae','coluzzii','arabiensis','funestus']", 
                   'fun':"species in ['funestus']"
                     }
 
 index_col = {'fcs':'comparison',
             'pvals': 'comparison',
             'log2counts': 'sampleID'}
 
 
+gff_url =  'https://vectorbase.org/common/downloads/release-68/AgambiaePEST/gff/data/VectorBase-68_AgambiaePEST.gff'
+
+
 # AnoExpress
 def load_results_arrays(data_type, analysis):
     """
     Load the counts data for a given analysis and sample query
     """
     assert data_type in ['log2counts', 'fcs', 'pvals'], "data_type must be either 'log2counts', 'fcs' or 'pvals'"
     assert analysis in ['gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun', 'irtex'], "analysis must be either 'gamb_colu', 'gamb_colu_arab', 'gamb_colu_arab_fun', 'fun' or 'irtex'"
@@ -74,25 +78,64 @@
 
     # subset to the species of interest
     metadata = metadata.query(taxon_query_dict[analysis])
 
     return metadata
 
 
+def load_gff(type='protein_coding_gene', query=None):
+
+    df = pd.concat([chunk for chunk in tqdm(pd.read_csv(gff_url, sep="\t", comment="#", chunksize=10000), desc='Loading gff data from VectorBase')])
+    df.columns = ['contig', 'source', 'type', 'start', 'end', 'na', 'strand', 'na2', 'attributes']
+    df = df.assign(contig=lambda x: x.contig.str.split("_").str.get(1))
+    
+    if type:
+     df = df.query(f"type == '{type}'")
+
+    # may only work for protein_coding_genes 
+    df = df.assign(GeneID=df.attributes.str.split(";", expand=True).iloc[:, 0].str.split("=").str.get(1))
+
+    # combine 2R and 2L, 3R and 3L
+    offset_2R = 61545105
+    offset_3R = 53200684
+
+    gffs = []
+    for contig in tqdm(['2R', '2L', '3R', '3L']):
+        df_contig = df.query("contig == @contig").copy()
+        if contig == '2L':
+            df_contig = df_contig.assign(contig='2RL', start=lambda x: x.start + offset_2R, end=lambda x: x.end + offset_2R)
+        if contig == '3L':
+            df_contig = df_contig.assign(contig='3RL', start=lambda x: x.start + offset_3R, end=lambda x: x.end + offset_3R)
+        elif contig in ['3R', '2R']:
+            df_contig = df_contig.assign(contig=lambda x: x.contig + 'L')
+        gffs.append(df_contig)
+
+    gff = pd.concat(gffs)
+    gff = pd.concat([gff, df]).sort_values(['contig', 'start', 'end'])
+
+    if query:
+        gff = gff.query(query)
+        
+    return gff
+
 def resolve_gene_id(gene_id, analysis):
     
     if isinstance(gene_id, str):
       if gene_id.startswith(('2L', '2R', '3L', '3R', 'X', '2RL', '3RL')):
-        import malariagen_data
         if analysis == 'fun':
-          assert "Unfortunately the genome feature file in malariagen_data does not contain AFUN identifiers, so we cannot subset by genomic span for An. funestus."
+          assert "Unfortunately the genome feature file does not contain AFUN identifiers, so we cannot subset by genomic span for An. funestus."
         else:
-          ag3 = malariagen_data.Ag3()
-        gff = ag3.genome_features(region=gene_id).query("type == 'gene'")
-        gene_id = gff.ID.to_list()
+
+          contig, start_end = gene_id.split(':')
+          start, end = start_end.replace(",", "").split('-')
+          start, end = int(start), int(end)
+
+          gff = load_gff(query=f"contig == '{contig}' and start <= {end} and end >= {start}")
+          gene_id = gff.GeneID.to_list()
+
       elif gene_id.endswith(('.tsv', '.txt')):
           gene_id = pd.read_csv(gene_id, sep="\t", header=None).iloc[:, 0].to_list()
       elif gene_id.endswith('.csv'):
           gene_id = pd.read_csv(gene_id, header=None).iloc[:, 0].to_list()
       elif gene_id.endswith('.xlsx'):
           gene_id = pd.read_excel(gene_id, header=None).iloc[:, 0].to_list()
       
@@ -214,20 +257,18 @@
   elif sort_by == 'mean':
     sort_idxs = np.argsort(df.apply(np.nanmean, axis=1)).values
   elif sort_by == 'agap':
     sort_idxs = np.argsort(df.reset_index()['GeneID'].values)
   elif sort_by == 'position':
     assert analysis != 'fun', "funestus cannot be sorted by position yet"
     
-    import malariagen_data
-    ag3 = malariagen_data.Ag3()
-    gff = ag3.genome_features().query("type == 'gene' & contig in @ag3.contigs")
-    gene_ids = df.reset_index()['GeneID'].to_list()
-    ordered_genes = gff.query(f"ID in {gene_ids}")['ID'].to_list()
-    sort_idxs = [np.where(df.reset_index()['GeneID'] == gene)[0][0] for gene in ordered_genes]
+    gff = load_gff()
+    gene_ids = gff.reset_index()['GeneID'].to_list()
+    ordered_genes = gff.query(f"GeneID in {gene_ids}")['GeneID'].to_list()
+    sort_idxs = [np.where(df.reset_index()['GeneID'] == gene)[0][0] for gene in ordered_genes if gene in df.reset_index()['GeneID'].to_list()]
 
   return df.iloc[sort_idxs, :].copy()
 
 
 def query_fc_count_data(fc_data, count_data, comparison_metadata, sample_metadata, query):
     mask = comparison_metadata.eval(query).to_list()
     comparison_metadata = comparison_metadata[mask] 
@@ -1020,7 +1061,33 @@
         toolbar_location="above",
         merge_tools=True,
         sizing_mode="stretch_width",
     )
     if show:
       bkplt.show(fig)
     return fig
+
+
+def consistent_genes(analysis, direction, n_experiments, low_count_filter=None):
+    
+    fc_data = data(data_type="fcs", analysis=analysis, microarray=False, annotations=True, low_count_filter=low_count_filter)
+    pval_data = data(data_type='pvals', analysis=analysis, microarray=False, annotations=True, low_count_filter=low_count_filter)
+
+    print(f"There are {fc_data.shape[0]} genes and {fc_data.shape[1]} differential expression comparisons in {analysis}")
+    if direction == 'up':
+        res_df = fc_data[fc_data.apply(lambda x: (x > 0).sum() >= n_experiments , axis=1)]
+        res_pval = pval_data[pval_data.apply(lambda x: x < 0.05, axis=1).sum(axis=1) > n_experiments].reset_index()['GeneID'].to_list()
+        res_df = res_df.query("GeneID in @res_pval")
+
+        if res_df.empty: 
+            print(f"There are no genes expressed direction={direction} in {n_experiments} experiments")
+            return
+        else:
+            return(res_df)
+    else: 
+        res_df = fc_data[fc_data.apply(lambda x: (x < 0).sum() >= n_experiments, axis=1)]
+        res_pval = pval_data[pval_data.apply(lambda x: x < 0.05, axis=1).sum(axis=1) > n_experiments].reset_index()['GeneID'].to_list()
+        res_df = res_df.query("GeneID in @res_pval")
+    if res_df.empty:
+        print(f"There are no genes expressed {direction} in {n_experiments} experiments")
+        return
+    return(res_df)
```

### Comparing `anoexpress-0.2.3/pyproject.toml` & `anoexpress-0.2.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "anoexpress"
-version = "0.2.3"
+version = "0.2.4"
 description = "A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes"
 readme = "README.md"
 documentation = "https://sanjaynagi.github.io/AnoExpress/"
 repository = "https://github.com/sanjaynagi/AnoExpress"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "anoexpress" }
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.8, <3.12"
 malariagen_data = ">8.0.1"
 scikit-allel="*"
 pandas = [
     {version="<1.4", python=">=3.7.1,<3.8"},
-    {version="*", python=">=3.8,<3.11"}
+    {version="*", python=">=3.8,<3.12"}
 ]
 seaborn = "*"
 numpy = "*"
 bokeh = "*"
 plotly = "*"
 scipy = "*"
 tqdm = "*"
@@ -32,16 +32,16 @@
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 black = "*"
 pytest = "*"
 notebook = "*"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `anoexpress-0.2.3/PKG-INFO` & `anoexpress-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: anoexpress
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes
 Home-page: https://github.com/sanjaynagi/AnoExpress
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh
 Requires-Dist: malariagen_data (>8.0.1)
 Requires-Dist: numpy
 Requires-Dist: pandas (<1.4) ; python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: pandas ; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: pandas ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: plotly
 Requires-Dist: scikit-allel
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
 Project-URL: Documentation, https://sanjaynagi.github.io/AnoExpress/
```

