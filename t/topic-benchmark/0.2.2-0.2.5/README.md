# Comparing `tmp/topic_benchmark-0.2.2.tar.gz` & `tmp/topic_benchmark-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_benchmark-0.2.2.tar", max compression
+gzip compressed data, was "topic_benchmark-0.2.5.tar", max compression
```

## Comparing `topic_benchmark-0.2.2.tar` & `topic_benchmark-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0     1071 2024-02-19 07:38:43.381533 topic_benchmark-0.2.2/LICENSE
--rw-r--r--   0        0        0      657 2024-03-13 14:29:25.208275 topic_benchmark-0.2.2/README.md
--rw-r--r--   0        0        0      693 2024-03-13 14:28:31.728138 topic_benchmark-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      114 2024-02-25 14:07:48.958607 topic_benchmark-0.2.2/topic_benchmark/__init__.py
--rw-r--r--   0        0        0       78 2024-02-19 10:22:20.253816 topic_benchmark-0.2.2/topic_benchmark/__main__.py
--rw-r--r--   0        0        0      384 2024-02-19 09:24:15.274817 topic_benchmark-0.2.2/topic_benchmark/base.py
--rw-r--r--   0        0        0     3044 2024-03-07 13:00:54.142517 topic_benchmark-0.2.2/topic_benchmark/benchmark.py
--rw-r--r--   0        0        0     2602 2024-03-13 13:59:11.167493 topic_benchmark-0.2.2/topic_benchmark/cli.py
--rw-r--r--   0        0        0       50 2024-02-25 14:04:22.669725 topic_benchmark-0.2.2/topic_benchmark/datasets/__init__.py
--rw-r--r--   0        0        0      806 2024-03-07 13:02:16.230526 topic_benchmark-0.2.2/topic_benchmark/datasets/newsgroups.py
--rw-r--r--   0        0        0      126 2024-02-19 10:05:20.151719 topic_benchmark-0.2.2/topic_benchmark/defaults.py
--rw-r--r--   0        0        0     2070 2024-03-13 13:58:40.007412 topic_benchmark-0.2.2/topic_benchmark/figures.py
--rw-r--r--   0        0        0      133 2024-02-19 10:25:03.206775 topic_benchmark-0.2.2/topic_benchmark/metrics/__init__.py
--rw-r--r--   0        0        0      539 2024-02-25 14:06:04.842162 topic_benchmark-0.2.2/topic_benchmark/metrics/diversity.py
--rw-r--r--   0        0        0      881 2024-03-05 08:34:40.883831 topic_benchmark-0.2.2/topic_benchmark/metrics/npmi.py
--rw-r--r--   0        0        0      977 2024-03-05 08:17:42.071259 topic_benchmark-0.2.2/topic_benchmark/metrics/wec.py
--rw-r--r--   0        0        0      185 2024-02-25 14:34:59.468057 topic_benchmark-0.2.2/topic_benchmark/models/__init__.py
--rw-r--r--   0        0        0      929 2024-02-27 08:28:58.418687 topic_benchmark-0.2.2/topic_benchmark/models/bertopic.py
--rw-r--r--   0        0        0     3134 2024-02-26 08:24:31.808499 topic_benchmark-0.2.2/topic_benchmark/models/classical.py
--rw-r--r--   0        0        0      953 2024-02-26 13:33:42.988512 topic_benchmark-0.2.2/topic_benchmark/models/top2vec.py
--rw-r--r--   0        0        0     1274 2024-03-07 13:11:55.291254 topic_benchmark-0.2.2/topic_benchmark/models/turftopic.py
--rw-r--r--   0        0        0      240 2024-02-25 14:05:44.438074 topic_benchmark-0.2.2/topic_benchmark/registries.py
--rw-r--r--   0        0        0     3734 2024-03-11 08:10:06.494576 topic_benchmark-0.2.2/topic_benchmark/table.py
--rw-r--r--   0        0        0      620 2024-02-25 14:32:02.743581 topic_benchmark-0.2.2/topic_benchmark/utils.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 topic_benchmark-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-19 07:38:43.381533 topic_benchmark-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-09 07:01:18.311495 topic_benchmark-0.2.5/README.md
+-rw-r--r--   0        0        0      768 2024-05-23 12:22:05.923267 topic_benchmark-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-03-22 10:07:39.674258 topic_benchmark-0.2.5/topic_benchmark/__init__.py
+-rw-r--r--   0        0        0       78 2024-02-19 10:22:20.253816 topic_benchmark-0.2.5/topic_benchmark/__main__.py
+-rw-r--r--   0        0        0      384 2024-02-19 09:24:15.274817 topic_benchmark-0.2.5/topic_benchmark/base.py
+-rw-r--r--   0        0        0     3044 2024-03-07 13:00:54.142517 topic_benchmark-0.2.5/topic_benchmark/benchmark.py
+-rw-r--r--   0        0        0     4215 2024-05-23 12:19:51.911005 topic_benchmark-0.2.5/topic_benchmark/cli.py
+-rw-r--r--   0        0        0     2353 2024-05-23 12:19:51.911005 topic_benchmark-0.2.5/topic_benchmark/cluster_problem.py
+-rw-r--r--   0        0        0      146 2024-05-23 12:19:51.931005 topic_benchmark-0.2.5/topic_benchmark/datasets/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-23 12:19:51.931005 topic_benchmark-0.2.5/topic_benchmark/datasets/arxiv_ml.py
+-rw-r--r--   0        0        0      244 2024-05-23 12:19:51.931005 topic_benchmark-0.2.5/topic_benchmark/datasets/bbc_news.py
+-rw-r--r--   0        0        0      806 2024-03-07 13:02:16.230526 topic_benchmark-0.2.5/topic_benchmark/datasets/newsgroups.py
+-rw-r--r--   0        0        0      126 2024-02-19 10:05:20.151719 topic_benchmark-0.2.5/topic_benchmark/defaults.py
+-rw-r--r--   0        0        0       50 2024-03-22 10:07:39.678258 topic_benchmark-0.2.5/topic_benchmark/encoders/__init__.py
+-rw-r--r--   0        0        0      842 2024-03-22 10:07:39.678258 topic_benchmark-0.2.5/topic_benchmark/encoders/e5_encoders.py
+-rw-r--r--   0        0        0     3354 2024-04-09 06:46:05.698513 topic_benchmark-0.2.5/topic_benchmark/figures.py
+-rw-r--r--   0        0        0    12974 2024-05-23 12:19:51.911005 topic_benchmark-0.2.5/topic_benchmark/figures_plt.py
+-rw-r--r--   0        0        0      133 2024-02-19 10:25:03.206775 topic_benchmark-0.2.5/topic_benchmark/metrics/__init__.py
+-rw-r--r--   0        0        0      539 2024-02-25 14:06:04.842162 topic_benchmark-0.2.5/topic_benchmark/metrics/diversity.py
+-rw-r--r--   0        0        0      881 2024-03-05 08:34:40.883831 topic_benchmark-0.2.5/topic_benchmark/metrics/npmi.py
+-rw-r--r--   0        0        0     1613 2024-05-23 12:19:51.931005 topic_benchmark-0.2.5/topic_benchmark/metrics/wec.py
+-rw-r--r--   0        0        0      185 2024-02-25 14:34:59.468057 topic_benchmark-0.2.5/topic_benchmark/models/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-23 12:19:51.935005 topic_benchmark-0.2.5/topic_benchmark/models/bertopic.py
+-rw-r--r--   0        0        0     3208 2024-05-23 12:19:51.935005 topic_benchmark-0.2.5/topic_benchmark/models/classical.py
+-rw-r--r--   0        0        0     1013 2024-05-23 12:19:51.935005 topic_benchmark-0.2.5/topic_benchmark/models/top2vec.py
+-rw-r--r--   0        0        0     1463 2024-05-23 12:19:51.935005 topic_benchmark-0.2.5/topic_benchmark/models/turftopic.py
+-rw-r--r--   0        0        0      316 2024-03-22 10:07:39.678258 topic_benchmark-0.2.5/topic_benchmark/registries.py
+-rw-r--r--   0        0        0     4714 2024-05-23 12:18:52.982894 topic_benchmark-0.2.5/topic_benchmark/table.py
+-rw-r--r--   0        0        0      620 2024-02-25 14:32:02.743581 topic_benchmark-0.2.5/topic_benchmark/utils.py
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 topic_benchmark-0.2.5/PKG-INFO
```

### Comparing `topic_benchmark-0.2.2/LICENSE` & `topic_benchmark-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.2/pyproject.toml` & `topic_benchmark-0.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "topic-benchmark"
-version = "0.2.2"
+version = "0.2.5"
 description = "Benchmarking topic models for a paper"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.0"
 scikit-learn = "^1.2.0"
 sentence-transformers = "^2.2.0"
 torch = "^2.1.0"
 scipy = "^1.10.0"
 rich = "^13.6.0"
 pyro-ppl = "^1.8.0"
-turftopic = "^0.2.9"
+turftopic = "^0.2.13"
 umap-learn = "^0.5.0"
 hdbscan = "^0.8.0"
 catalogue = "^2.0.0"
 gensim = "^4.3.2"
 radicli = "^0.0.25"
 pandas = "^2.1.0"
 plotly = "^5.18.0"
+kaleido="^0.2.0"
+matplotlib="^3.6.3"
+seaborn="^0.12.2"
+datasets="^2.18.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `topic_benchmark-0.2.2/topic_benchmark/benchmark.py` & `topic_benchmark-0.2.5/topic_benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.2/topic_benchmark/datasets/newsgroups.py` & `topic_benchmark-0.2.5/topic_benchmark/datasets/newsgroups.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.2/topic_benchmark/metrics/diversity.py` & `topic_benchmark-0.2.5/topic_benchmark/metrics/diversity.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.2/topic_benchmark/metrics/npmi.py` & `topic_benchmark-0.2.5/topic_benchmark/metrics/npmi.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.2/topic_benchmark/models/bertopic.py` & `topic_benchmark-0.2.5/topic_benchmark/models/top2vec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+from functools import partial
+
 from hdbscan import HDBSCAN
 from sklearn.feature_extraction.text import CountVectorizer
 from turftopic import ClusteringTopicModel
 from umap.umap_ import UMAP
 
 from topic_benchmark.base import Loader
 from topic_benchmark.registries import model_registry
 
 
-@model_registry.register("BERTopic")
-def load_bertopic(encoder, vectorizer: CountVectorizer) -> Loader:
-    dim_red = UMAP(n_neighbors=15, n_components=5, metric="cosine")
+@model_registry.register("Top2Vec")
+def load_top2vec(encoder, vectorizer: CountVectorizer) -> Loader:
+    dim_red = UMAP(
+        n_neighbors=15, n_components=5, metric="cosine", random_state=42
+    )
     clustering = HDBSCAN(
         min_cluster_size=15,
         metric="euclidean",
         cluster_selection_method="eom",
     )
 
     def _load(n_components: int):
         return ClusteringTopicModel(
             encoder=encoder,
             vectorizer=vectorizer,
             dimensionality_reduction=dim_red,
             clustering=clustering,
-            feature_importance="c-tf-idf",
-            reduction_method="agglomerative",
+            feature_importance="centroid",
+            reduction_method="smallest",
             n_reduce_to=n_components,
+            random_state=42,
         )
 
     return _load
```

### Comparing `topic_benchmark-0.2.2/topic_benchmark/models/classical.py` & `topic_benchmark-0.2.5/topic_benchmark/models/classical.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,19 @@
             ) from e
         document_term_matrix = vectorizer.transform(corpus)  # type: ignore
         vocab = vectorizer.get_feature_names_out()  # type: ignore
         res = TopicData(
             corpus=corpus,
             document_term_matrix=document_term_matrix,
             document_topic_matrix=document_topic_matrix,
-            document_representation=document_term_matrix
-            if document_representation == "term"
-            else document_topic_matrix,
+            document_representation=(
+                document_term_matrix
+                if document_representation == "term"
+                else document_topic_matrix
+            ),
             vocab=vocab,
             topic_term_matrix=components,
             transform=self.transform,
             topic_names=[],
         )
         return res
 
@@ -78,20 +80,20 @@
         verbose=verbose,
     )
 
 
 @model_registry.register("NMF")
 def load_nmf(encoder, vectorizer: CountVectorizer) -> Loader:
     def _load(n_components: int):
-        model = NMF(n_components)
+        model = NMF(n_components, random_state=42)
         return make_topic_pipeline(vectorizer, model)
 
     return _load
 
 
 @model_registry.register("LDA")
 def load_lda(encoder, vectorizer: CountVectorizer) -> Loader:
     def _load(n_components: int):
-        model = LatentDirichletAllocation(n_components)
+        model = LatentDirichletAllocation(n_components, random_state=42)
         return make_topic_pipeline(vectorizer, model)
 
     return _load
```

### Comparing `topic_benchmark-0.2.2/topic_benchmark/models/top2vec.py` & `topic_benchmark-0.2.5/topic_benchmark/models/bertopic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from functools import partial
-
 from hdbscan import HDBSCAN
 from sklearn.feature_extraction.text import CountVectorizer
 from turftopic import ClusteringTopicModel
 from umap.umap_ import UMAP
 
 from topic_benchmark.base import Loader
 from topic_benchmark.registries import model_registry
 
 
-@model_registry.register("Top2Vec")
-def load_top2vec(encoder, vectorizer: CountVectorizer) -> Loader:
-    dim_red = UMAP(n_neighbors=15, n_components=5, metric="cosine")
+@model_registry.register("BERTopic")
+def load_bertopic(encoder, vectorizer: CountVectorizer) -> Loader:
+    dim_red = UMAP(
+        n_neighbors=15, n_components=5, metric="cosine", random_state=42
+    )
     clustering = HDBSCAN(
         min_cluster_size=15,
         metric="euclidean",
         cluster_selection_method="eom",
     )
 
     def _load(n_components: int):
         return ClusteringTopicModel(
             encoder=encoder,
             vectorizer=vectorizer,
             dimensionality_reduction=dim_red,
             clustering=clustering,
-            feature_importance="centroid",
-            reduction_method="smallest",
+            feature_importance="c-tf-idf",
+            reduction_method="agglomerative",
             n_reduce_to=n_components,
+            random_state=42,
         )
 
     return _load
```

### Comparing `topic_benchmark-0.2.2/topic_benchmark/table.py` & `topic_benchmark-0.2.5/topic_benchmark/table.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,14 +33,28 @@
         " ".join(midrules),
         metric_names + "\\\\",
         "\\midrule",
     ]
     return lines
 
 
+def produce_footer() -> list[str]:
+    return [
+        "\\bottomrule",
+        "\\label{table:evaluation}",
+        "\\end{tabular}",
+        "}",
+        "\\egroup",
+        "\\caption{ Coherence and Diversity of Topics over Multiple Datasets \\\\",
+        "\\textit{Best in bold, second best underlined}",
+        "}",
+        "\\end{table}",
+    ]
+
+
 def format_cells(table: pd.DataFrame) -> pd.DataFrame:
     table = table[["NPMI Coherence", "Word Embedding Coherence", "Diversity"]]
     bold = {column: table[column].max() for column in table.columns}
     underline = {
         column: table[column].nlargest(n=2).iloc[-1]
         for column in table.columns
     }
@@ -68,14 +82,26 @@
     "BERTopic",
     "CombinedTM",
     "ZeroShotTM",
     "NMF",
     "LDA",
 ]
 
+EMBEDDING_ORDER = [
+    "average_word_embeddings_glove.6B.300d",
+    "all-MiniLM-L6-v2",
+    "all-mpnet-base-v2",
+    "intfloat/e5-large-v2",
+]
+
+DATASET_ORDER = [
+    "20 Newsgroups Preprocessed",
+    "20 Newsgroups Raw",
+]
+
 
 def produce_body(groups: list[pd.DataFrame]) -> list[str]:
     groups = [group.reset_index().set_index("model") for group in groups]
     models = set()
     for group in groups:
         models |= set(group.index)
     models = [model for model in MODEL_ORDER if model in models]
@@ -88,41 +114,48 @@
                 row.extend(group.loc[model])
             except KeyError:
                 row.extend(["NA"] * 3)
         lines.append(" & ".join([model, *row]) + "\\\\")
     return lines
 
 
-def produce_footer() -> list[str]:
-    return [
-        "\\bottomrule",
-        "\\label{table:evaluation}",
-        "\\end{tabular}",
-        "}",
-        "\\egroup",
-        "\\caption{ Coherence and Diversity of Topics over Multiple Datasets \\\\",
-        "\\textit{Best in bold, second best underlined}",
-        "}",
-        "\\end{table}",
-    ]
-
-
-def produce_latex_table(
+def produce_encoder_rows(
     entries: list[Union[BenchmarkEntry, BenchmarkError]],
-) -> str:
+    encoder_name: str,
+) -> list[str]:
+    """Produces lines in a table for a single embedding model."""
+    encoder_name = encoder_name.replace(
+        "_", "\\_"
+    )  # Escaping underscores for LaTex
     entries = [entry for entry in entries if "error_message" not in entry]
     data = pd.DataFrame.from_records(entries)
     data = data.join(pd.json_normalize(data["results"]))
     data = data.groupby(["dataset", "model"])[
         [
             "NPMI Coherence",
             "Word Embedding Coherence",
             "Diversity",
         ]
     ].mean()
-    group_names, group_tables = zip(*data.groupby("dataset"))
+    groups = dict(list(data.groupby("dataset")))
+    # Loading tables in proper order
+    group_tables = [groups[dataset] for dataset in DATASET_ORDER]
     lines = [
-        *produce_header(group_names),
+        "\\midrule",
+        f"\\textbf{{{encoder_name}}} & & & & & & \\\\",
+        "\\midrule",
         *produce_body(group_tables),
-        *produce_footer(),
     ]
+    return lines
+
+
+def produce_full_table(
+    encoder_entries: dict[str, Union[BenchmarkEntry, BenchmarkError]],
+) -> str:
+    """Produces full table for all encoder models."""
+    lines = [*produce_header(DATASET_ORDER)]
+    for encoder in EMBEDDING_ORDER:
+        if encoder not in encoder_entries:
+            continue
+        lines.extend(produce_encoder_rows(encoder_entries[encoder], encoder))
+    lines.extend(produce_footer())
     return "\n".join(lines)
```

### Comparing `topic_benchmark-0.2.2/topic_benchmark/utils.py` & `topic_benchmark-0.2.5/topic_benchmark/utils.py`

 * *Files identical despite different names*

