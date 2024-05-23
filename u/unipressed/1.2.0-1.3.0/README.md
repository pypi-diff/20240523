# Comparing `tmp/unipressed-1.2.0.tar.gz` & `tmp/unipressed-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipressed-1.2.0.tar", max compression
+gzip compressed data, was "unipressed-1.3.0.tar", max compression
```

## Comparing `unipressed-1.2.0.tar` & `unipressed-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-06-05 12:43:55.653550 unipressed-1.2.0/LICENSE
--rw-r--r--   0        0        0    21175 2023-06-05 12:43:55.657549 unipressed-1.2.0/README.md
--rw-r--r--   0        0        0     1600 2023-06-11 07:14:56.292402 unipressed-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       83 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/__init__.py
--rw-r--r--   0        0        0     1045 2023-06-05 14:00:21.355796 unipressed-1.2.0/unipressed/dataset/__init__.py
--rw-r--r--   0        0        0      480 2023-06-05 13:57:49.292173 unipressed-1.2.0/unipressed/dataset/arba.py
--rw-r--r--   0        0        0      590 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/citations.py
--rw-r--r--   0        0        0     6939 2023-06-11 07:14:56.292402 unipressed-1.2.0/unipressed/dataset/core.py
--rw-r--r--   0        0        0      456 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/database.py
--rw-r--r--   0        0        0      486 2023-06-05 12:43:55.657549 unipressed-1.2.0/unipressed/dataset/diseases.py
--rw-r--r--   0        0        0     1695 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/arba.py
--rw-r--r--   0        0        0     1254 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/citations.py
--rw-r--r--   0        0        0      934 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/database.py
--rw-r--r--   0        0        0      900 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/diseases.py
--rw-r--r--   0        0        0     1402 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/keywords.py
--rw-r--r--   0        0        0      997 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/locations.py
--rw-r--r--   0        0        0     2081 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/proteomes.py
--rw-r--r--   0        0        0     2752 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/taxonomy.py
--rw-r--r--   0        0        0     3907 2023-06-11 07:14:56.296402 unipressed-1.2.0/unipressed/dataset/generated_types/uniparc.py
--rw-r--r--   0        0        0    27932 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/uniprotkb.py
--rw-r--r--   0        0        0     2419 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/uniref.py
--rw-r--r--   0        0        0     2056 2023-06-11 07:14:56.300402 unipressed-1.2.0/unipressed/dataset/generated_types/unirule.py
--rw-r--r--   0        0        0      601 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/keywords.py
--rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/locations.py
--rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/proteomes.py
--rw-r--r--   0        0        0     6804 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/search.py
--rw-r--r--   0        0        0      665 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/taxonomy.py
--rw-r--r--   0        0        0      235 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/type_vars.py
--rw-r--r--   0        0        0      623 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniparc.py
--rw-r--r--   0        0        0      715 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniprotkb.py
--rw-r--r--   0        0        0      503 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/uniref.py
--rw-r--r--   0        0        0      527 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/dataset/unirule.py
--rw-r--r--   0        0        0       71 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/id_mapping/__init__.py
--rw-r--r--   0        0        0     2913 2023-06-05 13:55:45.672479 unipressed-1.2.0/unipressed/id_mapping/core.py
--rw-r--r--   0        0        0     3390 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/id_mapping/types.py
--rw-r--r--   0        0        0      444 2023-06-05 12:43:55.661550 unipressed-1.2.0/unipressed/util.py
--rw-r--r--   0        0        0    21998 1970-01-01 00:00:00.000000 unipressed-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 12:43:55.653550 unipressed-1.3.0/LICENSE
+-rw-r--r--   0        0        0    21175 2023-06-05 12:43:55.657549 unipressed-1.3.0/README.md
+-rw-r--r--   0        0        0     1611 2024-05-23 12:28:12.561529 unipressed-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-05-23 12:35:02.706925 unipressed-1.3.0/unipressed/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-05 14:00:21.355796 unipressed-1.3.0/unipressed/dataset/__init__.py
+-rw-r--r--   0        0        0      480 2023-06-05 13:57:49.292173 unipressed-1.3.0/unipressed/dataset/arba.py
+-rw-r--r--   0        0        0      590 2023-06-05 12:43:55.657549 unipressed-1.3.0/unipressed/dataset/citations.py
+-rw-r--r--   0        0        0     6939 2023-06-11 07:14:56.292402 unipressed-1.3.0/unipressed/dataset/core.py
+-rw-r--r--   0        0        0      456 2023-06-05 12:43:55.657549 unipressed-1.3.0/unipressed/dataset/database.py
+-rw-r--r--   0        0        0      486 2023-06-05 12:43:55.657549 unipressed-1.3.0/unipressed/dataset/diseases.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:19:53.711831 unipressed-1.3.0/unipressed/dataset/generated_types/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/arba.py
+-rw-r--r--   0        0        0     1254 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/citations.py
+-rw-r--r--   0        0        0      935 2024-05-21 13:18:37.671764 unipressed-1.3.0/unipressed/dataset/generated_types/database.py
+-rw-r--r--   0        0        0      900 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/diseases.py
+-rw-r--r--   0        0        0     1655 2024-05-21 13:18:37.671764 unipressed-1.3.0/unipressed/dataset/generated_types/keywords.py
+-rw-r--r--   0        0        0      997 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/locations.py
+-rw-r--r--   0        0        0     2081 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/proteomes.py
+-rw-r--r--   0        0        0     2726 2024-05-21 13:18:37.671764 unipressed-1.3.0/unipressed/dataset/generated_types/taxonomy.py
+-rw-r--r--   0        0        0     5013 2024-05-21 13:18:37.675764 unipressed-1.3.0/unipressed/dataset/generated_types/uniparc.py
+-rw-r--r--   0        0        0    28007 2024-05-22 12:15:16.767056 unipressed-1.3.0/unipressed/dataset/generated_types/uniprotkb.py
+-rw-r--r--   0        0        0     2419 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/uniref.py
+-rw-r--r--   0        0        0     2056 2024-05-18 12:16:33.317216 unipressed-1.3.0/unipressed/dataset/generated_types/unirule.py
+-rw-r--r--   0        0        0      601 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/keywords.py
+-rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/locations.py
+-rw-r--r--   0        0        0      495 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/proteomes.py
+-rw-r--r--   0        0        0     6804 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/search.py
+-rw-r--r--   0        0        0      665 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/taxonomy.py
+-rw-r--r--   0        0        0      235 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/type_vars.py
+-rw-r--r--   0        0        0      623 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/uniparc.py
+-rw-r--r--   0        0        0      715 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/uniprotkb.py
+-rw-r--r--   0        0        0      503 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/uniref.py
+-rw-r--r--   0        0        0      527 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/dataset/unirule.py
+-rw-r--r--   0        0        0       71 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/id_mapping/__init__.py
+-rw-r--r--   0        0        0     2913 2023-06-05 13:55:45.672479 unipressed-1.3.0/unipressed/id_mapping/core.py
+-rw-r--r--   0        0        0     3428 2024-05-21 13:18:37.675764 unipressed-1.3.0/unipressed/id_mapping/types.py
+-rw-r--r--   0        0        0      444 2023-06-05 12:43:55.661550 unipressed-1.3.0/unipressed/util.py
+-rw-r--r--   0        0        0    22052 1970-01-01 00:00:00.000000 unipressed-1.3.0/PKG-INFO
```

### Comparing `unipressed-1.2.0/LICENSE` & `unipressed-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/README.md` & `unipressed-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/pyproject.toml` & `unipressed-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "unipressed"
-version = "1.2.0"
+version = "1.3.0"
 description = "Comprehensive Python client for the Uniprot REST API"
 authors = ["Michael Milton <michael.r.milton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://multimeric.github.io/Unipressed"
 repository = "https://github.com/multimeric/Unipressed"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 requests = "^2.28.1"
 typing-extensions = "^4.3.0"
+mkdocstrings-python = "^1.10.2"
 
 [tool.poetry.group.tests.dependencies]
 pytest = { version = "^7.1.2" }
 fastaparser = "^1.1"
 
 [tool.poetry.group.docs.dependencies]
-mkdocstrings = { extras = ["python"], version = "^0.19.0" }
+mkdocstrings = { version = "^0.25.1" }
 mkdocs = { version = "^1.3.1" }
 mkdocs-material = { version = "^8.3.9" }
 mkdocs-include-markdown-plugin = { version = "^3.6.1" }
 rich = { git = "https://github.com/multimeric/rich.git", branch = "max-depth-install" }
 
 [tool.poetry.group.readme.dependencies]
 jupyter = { version = "^1.0.0", python = ">=3.8" }
```

### Comparing `unipressed-1.2.0/unipressed/dataset/__init__.py` & `unipressed-1.3.0/unipressed/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/citations.py` & `unipressed-1.3.0/unipressed/dataset/citations.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/core.py` & `unipressed-1.3.0/unipressed/dataset/core.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/arba.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/arba.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/citations.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/citations.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/database.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,13 +23,13 @@
 DatabaseCrossReference: TypeAlias = Literal[
     "id",
     "name",
     "abbrev",
     "pubmed_id",
     "doi_id",
     "link_type",
-    "server",
+    "servers",
     "dbUrl",
     "category",
     "statistics",
 ]
 DatabaseFields: TypeAlias = Literal[DatabaseCrossReference,]
```

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/diseases.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/diseases.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/keywords.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/keywords.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 from __future__ import annotations
 
 from datetime import date
 from typing import Iterable, Union
 
 from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict
 
+Category: TypeAlias = Literal[
+    "technical_term",
+    "ptm",
+    "molecular_function",
+    "ligand",
+    "domain",
+    "disease",
+    "developmental_stage",
+    "coding_sequence_diversity",
+    "cellular_component",
+    "biological_process",
+]
+
 
 class KeywordsQueryDict(TypedDict):
     and_: NotRequired[Iterable["KeywordsQuery"]]
     "Two or more filters that must both be satisfied"
     or_: NotRequired[Iterable["KeywordsQuery"]]
     "Two or more filters, any of which can be satisfied"
     not_: NotRequired[Iterable["KeywordsQuery"]]
     "Negate a filter"
     name: NotRequired[str]
     "Name\ne.g. 2Fe-2S"
     keyword_id: NotRequired[str]
     "Keyword [AC]\ne.g. KW-0001"
-    category: NotRequired[str]
+    category: NotRequired[Category]
     "Category\ne.g. Domain\n* technical_term: Technical term [KW-9990]\n* ptm: PTM [KW-9991]\n* molecular_function: Molecular function [KW-9992]\n* ligand: Ligand [KW-9993]\n* domain: Domain [KW-9994]\n* disease: Disease [KW-9995]\n* developmental_stage: Developmental stage [KW-9996]\n* coding_sequence_diversity: Coding sequence diversity [KW-9997]\n* cellular_component: Cellular component [KW-9998]\n* biological_process: Biological process [KW-9999]"
 
 
 KeywordsQuery: TypeAlias = Union[KeywordsQueryDict, str]
 KeywordsKeyword: TypeAlias = Literal[
     "id",
     "name",
```

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/locations.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/locations.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/proteomes.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/proteomes.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/taxonomy.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     rank: NotRequired[Rank]
     "Rank\ne.g. SPECIES_GROUP\n* SUPERKINGDOM: Superkingdom\n* KINGDOM: Kingdom\n* SUBKINGDOM: Subkingdom\n* SUPERPHYLUM: Superphylum\n* PHYLUM: Phylum\n* SUBPHYLUM: Subphylum\n* SUPERCLASS: Superclass\n* CLASS: Class\n* SUBCLASS: Subclass\n* INFRACLASS: Infraclass\n* COHORT: Cohort\n* SUBCOHORT: Subcohort\n* SUPERORDER: Superorder\n* ORDER: Order\n* SUBORDER: Suborder\n* INFRAORDER: Infraorder\n* PARVORDER: Parvorder\n* SUPERFAMILY: Superfamily\n* FAMILY: Family\n* SUBFAMILY: Subfamily\n* TRIBE: Tribe\n* SUBTRIBE: Subtribe\n* GENUS: Genus\n* SUBGENUS: Subgenus\n* SPECIES_GROUP: Species group\n* SPECIES_SUBGROUP: Species subgroup\n* SPECIES: Species\n* SUBSPECIES: Subspecies\n* VARIETAS: Varietas\n* FORMA: Forma\n* NO_RANK: No rank"
     strain: NotRequired[str]
     "Strain\ne.g. SPECIES_GROUP"
     host: NotRequired[int]
     "Virus host\ne.g. 85621"
     linked: NotRequired[bool]
-    "With external info\ne.g. true\n* true: Yes\n* false: No"
+    "With external info\ne.g. true"
     parent: NotRequired[str]
     "Parent\ne.g. 9606"
     ancestor: NotRequired[str]
     "Ancestor\ne.g. 85621"
 
 
 TaxonomyQuery: TypeAlias = Union[TaxonomyQueryDict, str]
```

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/uniparc.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/uniparc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,88 @@
 from __future__ import annotations
 
 from datetime import date
 from typing import Iterable, Union
 
 from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict
 
+Database: TypeAlias = Literal[
+    "EnsemblBacteria",
+    "EnsemblFungi",
+    "EnsemblMetazoa",
+    "EnsemblPlants",
+    "EnsemblProtists",
+    "embl-cds",
+    "EMBL_CON",
+    "EMBL_TPA",
+    "EMBL_TSA",
+    "EMBLWGS",
+    "Ensembl",
+    "EnsemblRapid",
+    "EPO",
+    "FlyBase",
+    "FusionGDB",
+    "H-InvDB",
+    "IPI",
+    "JPO",
+    "KIPO",
+    "PATRIC",
+    "PDB",
+    "PIR",
+    "PIRARC",
+    "PRF",
+    "RefSeq",
+    "REMTREMBL",
+    "SEED",
+    "SGD",
+    "UniProt",
+    "isoforms",
+    "TAIR",
+    "TREMBLNEW",
+    "TREMBL_VARSPLIC",
+    "TROME",
+    "UNIMES",
+    "USPTO",
+    "VectorBase",
+    "VEGA",
+    "WBParaSite",
+    "WormBase",
+]
+Active: TypeAlias = Literal[
+    "EnsemblBacteria",
+    "EnsemblFungi",
+    "EnsemblMetazoa",
+    "EnsemblPlants",
+    "EnsemblProtists",
+    "embl-cds",
+    "EMBL_CON",
+    "EMBL_TSA",
+    "EMBLWGS",
+    "Ensembl",
+    "EnsemblRapid",
+    "EPO",
+    "FlyBase",
+    "FusionGDB",
+    "JPO",
+    "KIPO",
+    "PATRIC",
+    "PDB",
+    "RefSeq",
+    "SEED",
+    "SGD",
+    "UniProt",
+    "isoforms",
+    "TAIR",
+    "TROME",
+    "USPTO",
+    "VEGA",
+    "WBParaSite",
+    "WormBase",
+]
+
 
 class UniparcQueryDict(TypedDict):
     and_: NotRequired[Iterable["UniparcQuery"]]
     "Two or more filters that must both be satisfied"
     or_: NotRequired[Iterable["UniparcQuery"]]
     "Two or more filters, any of which can be satisfied"
     not_: NotRequired[Iterable["UniparcQuery"]]
@@ -18,27 +92,27 @@
     uniprotkb: NotRequired[str]
     "UniProtKB AC\ne.g. P12345"
     isoform: NotRequired[str]
     "UniProtKB isoform ID\ne.g. P12345"
     upid: NotRequired[str]
     "Proteome ID\ne.g. UP123456789"
     taxonomy_name: NotRequired[str]
-    "Taxonomy [OC]\ne.g. sample name"
+    "Taxonomy [OC]\ne.g. Human"
     taxonomy_id: NotRequired[str]
     "Taxonomy id"
     gene: NotRequired[str]
-    "Gene name [GN]\ne.g. sample gene"
+    "Gene name [GN]\ne.g. PROZ"
     protein: NotRequired[str]
-    "Protein name\ne.g. sample protein"
-    database: NotRequired[str]
-    "Database\ne.g. sample database\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TPA: EMBL_TPA\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* H-InvDB: H-InvDB\n* IPI: IPI\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* PIR: PIR\n* PIRARC: PIRARC\n* PRF: PRF\n* RefSeq: RefSeq\n* REMTREMBL: REMTREMBL\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TREMBLNEW: TREMBLNEW\n* TREMBL_VARSPLIC: TREMBL_VARSPLIC\n* TROME: TROME\n* UNIMES: UNIMES\n* USPTO: USPTO\n* VectorBase: VectorBase\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
-    active: NotRequired[str]
-    "Active\ne.g. sample active\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* RefSeq: RefSeq\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TROME: TROME\n* USPTO: USPTO\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
+    "Protein name\ne.g. Protein Z"
+    database: NotRequired[Database]
+    "Database\ne.g. Gene3D\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TPA: EMBL_TPA\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* H-InvDB: H-InvDB\n* IPI: IPI\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* PIR: PIR\n* PIRARC: PIRARC\n* PRF: PRF\n* RefSeq: RefSeq\n* REMTREMBL: REMTREMBL\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TREMBLNEW: TREMBLNEW\n* TREMBL_VARSPLIC: TREMBL_VARSPLIC\n* TROME: TROME\n* UNIMES: UNIMES\n* USPTO: USPTO\n* VectorBase: VectorBase\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
+    active: NotRequired[Active]
+    "Active\ne.g. Gene3D\n* EnsemblBacteria: EnsemblBacteria\n* EnsemblFungi: EnsemblFungi\n* EnsemblMetazoa: EnsemblMetazoa\n* EnsemblPlants: EnsemblPlants\n* EnsemblProtists: EnsemblProtists\n* embl-cds: EMBL CDS\n* EMBL_CON: EMBL_CON\n* EMBL_TSA: EMBL_TSA\n* EMBLWGS: EMBLWGS\n* Ensembl: Ensembl\n* EnsemblRapid: EnsemblRapid\n* EPO: EPO\n* FlyBase: FlyBase\n* FusionGDB: FusionGDB\n* JPO: JPO\n* KIPO: KIPO\n* PATRIC: PATRIC\n* PDB: PDB\n* RefSeq: RefSeq\n* SEED: SEED\n* SGD: SGD\n* UniProt: UniProtKB\n* isoforms: UniProtKB/Swiss-Prot isoforms\n* TAIR: TAIR\n* TROME: TROME\n* USPTO: USPTO\n* VEGA: VEGA\n* WBParaSite: WBParaSite\n* WormBase: WormBase"
     checksum: NotRequired[str]
-    "Checksum (CRC64/MD5)\ne.g. sample checksum"
+    "Checksum (CRC64/MD5)\ne.g. B8824CE1ECAEEEAE"
     length: NotRequired[
         tuple[
             Union[
                 int,
                 Literal["*",],
             ],
             Union[
@@ -71,15 +145,15 @@
     "Pfam",
     "PIRSF",
     "PRINTS",
     "PROSITE",
     "SFLD",
     "SMART",
     "SUPFAM",
-    "TIGRFAMs",
+    "NCBIfam",
 ]
 UniparcFields: TypeAlias = Literal[
     UniparcNamesTaxonomy,
     UniparcSequences,
     UniparcMiscellaneous,
     UniparcDateOf,
     UniparcFamilyDomains,
```

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/uniprotkb.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/uniprotkb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Iterable, Union
 
 from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict
 
 Existence: TypeAlias = Literal["1", "2", "3", "4", "5"]
 Organelle: TypeAlias = Literal[
     "mitochondrion",
+    "plasmid",
     "plastid",
     "chloroplast",
     "cyanelle",
     "apicoplast",
     "organellar chromatophore",
     "non-photosynthetic plastid",
     "nucleomorph",
@@ -241,15 +242,15 @@
     interactor: NotRequired[str]
     "Binary Interaction\ne.g. EBI-1042898"
     cc_subunit: NotRequired[str]
     "Cc subunit\ne.g. homodimer"
     cc_subunit_exp: NotRequired[str]
     "Cc subunit exp\ne.g. homodimer"
     structure_3d: NotRequired[bool]
-    "3D Structure\ne.g. true\n* true: Yes\n* false: No"
+    "3D Structure\ne.g. true"
     ft_secstruct: NotRequired[str]
     "Ft secstruct\ne.g. *"
     ft_secstruct_exp: NotRequired[str]
     "Ft secstruct exp\ne.g. *"
     ft_helix: NotRequired[str]
     "Ft helix\ne.g. *"
     ft_helix_exp: NotRequired[str]
@@ -371,19 +372,19 @@
     ft_unsure_exp: NotRequired[str]
     "Ft unsure exp\ne.g. *"
     ft_positional: NotRequired[str]
     "Ft positional\ne.g. colorectal"
     ft_positional_exp: NotRequired[str]
     "Ft positional exp\ne.g. colorectal"
     fragment: NotRequired[bool]
-    "Fragment\ne.g. true\n* true: Yes\n* false: No"
+    "Fragment\ne.g. true"
     organelle: NotRequired[Organelle]
-    "Encoded in\ne.g. mitochondrion\n* mitochondrion: Mitochondrion\n* plastid: Plastid\n* chloroplast: Chloroplast\n* cyanelle: Cyanelle\n* apicoplast: Apicoplast\n* organellar chromatophore: Organellar chromatophore\n* non-photosynthetic plastid: Non-photosynthetic plastid\n* nucleomorph: Nucleomorph\n* hydrogenosome: Hydrogenosome"
+    "Encoded in\ne.g. mitochondrion\n* mitochondrion: Mitochondrion\n* plasmid: Plasmid\n* plastid: Plastid\n* chloroplast: Chloroplast\n* cyanelle: Cyanelle\n* apicoplast: Apicoplast\n* organellar chromatophore: Organellar chromatophore\n* non-photosynthetic plastid: Non-photosynthetic plastid\n* nucleomorph: Nucleomorph\n* hydrogenosome: Hydrogenosome"
     precursor: NotRequired[bool]
-    "Precursor\ne.g. true\n* true: Yes\n* false: No"
+    "Precursor\ne.g. true"
     tissue: NotRequired[str]
     "Tissue\ne.g. head"
     strain: NotRequired[str]
     "Strain\ne.g. berkeley"
     plasmid: NotRequired[str]
     "Plasmid\ne.g. pO113"
     transposon: NotRequired[str]
@@ -399,17 +400,17 @@
     family: NotRequired[str]
     "Protein family\ne.g. pa28"
     ft_coiled: NotRequired[str]
     "Ft coiled\ne.g. *"
     ft_coiled_exp: NotRequired[str]
     "Ft coiled exp\ne.g. *"
     ft_compbias: NotRequired[str]
-    "Ft compbias\ne.g. glu-rich"
+    "Ft compbias\ne.g. basic residues"
     ft_compbias_exp: NotRequired[str]
-    "Ft compbias exp\ne.g. glu-rich"
+    "Ft compbias exp\ne.g. basic residues"
     ft_motif: NotRequired[str]
     "Ft motif\ne.g. motif"
     ft_motif_exp: NotRequired[str]
     "Ft motif exp\ne.g. motif"
     ft_region: NotRequired[str]
     "Ft region\ne.g. motif"
     ft_region_exp: NotRequired[str]
@@ -557,17 +558,17 @@
     proteome: NotRequired[str]
     "Proteome ID\ne.g. UP000005640"
     proteomecomponent: NotRequired[str]
     "Proteome Component\ne.g. chromosome"
     scope: NotRequired[str]
     "Cited for\ne.g. microtubule"
     reviewed: NotRequired[bool]
-    "Reviewed\ne.g. true\n* true: Yes\n* false: No"
+    "Reviewed\ne.g. true"
     active: NotRequired[bool]
-    "Active\ne.g. true\n* true: Yes\n* false: No"
+    "Active\ne.g. true"
     uniref_cluster_50: NotRequired[str]
     "UniRef50\ne.g. UniRef50_P05067"
     uniref_cluster_90: NotRequired[str]
     "UniRef90\ne.g. UniRef90_P05067"
     uniref_cluster_100: NotRequired[str]
     "UniRef100\ne.g. UniRef100_P05067"
     uniparc: NotRequired[str]
@@ -673,35 +674,37 @@
     "ft_propep",
     "ft_signal",
     "ft_transit",
 ]
 UniprotkbStructure: TypeAlias = Literal[
     "structure_3d", "ft_strand", "ft_helix", "ft_turn"
 ]
-UniprotkbPublications: TypeAlias = Literal["lit_pubmed_id",]
+UniprotkbPublications: TypeAlias = Literal["lit_pubmed_id", "lit_doi_id"]
 UniprotkbDateOf: TypeAlias = Literal[
     "date_created", "date_modified", "date_sequence_modified", "version"
 ]
 UniprotkbFamilyDomains: TypeAlias = Literal[
     "ft_coiled",
     "ft_compbias",
     "cc_domain",
     "ft_domain",
     "ft_motif",
     "protein_families",
     "ft_region",
     "ft_repeat",
+    "cc_similarity",
     "ft_zn_fing",
 ]
 UniprotkbSequence: TypeAlias = Literal[
-    "xref_ccds", "xref_embl", "xref_pir", "xref_refseq"
+    "xref_ccds", "xref_embl", "xref_generif", "xref_pir", "xref_refseq"
 ]
 UniprotkbThreedStructure: TypeAlias = Literal[
     "xref_alphafolddb",
     "xref_bmrb",
+    "xref_emdb",
     "xref_pcddb",
     "xref_pdb",
     "xref_pdbsum",
     "xref_sasbdb",
     "xref_smr",
 ]
 UniprotkbProteinProteinInteraction: TypeAlias = Literal[
@@ -745,15 +748,15 @@
     "xref_metosite",
     "xref_phosphositeplus",
     "xref_swisspalm",
     "xref_unicarbkb",
     "xref_iptmnet",
 ]
 UniprotkbPolymorphismAndMutation: TypeAlias = Literal[
-    "xref_biomuta", "xref_dmdm", "xref_dbsnp"
+    "xref_alzforum", "xref_biomuta", "xref_dmdm", "xref_dbsnp"
 ]
 UniprotkbTwodGel: TypeAlias = Literal[
     "xref_compluyeast-2dpage",
     "xref_dosac-cobs-2dpage",
     "xref_ogp",
     "xref_reproduction-2dpage",
     "xref_swiss-2dpage",
@@ -766,14 +769,15 @@
     "xref_massive",
     "xref_maxqb",
     "xref_pride",
     "xref_paxdb",
     "xref_peptideatlas",
     "xref_promex",
     "xref_proteomicsdb",
+    "xref_pumba",
     "xref_topdownproteomics",
     "xref_jpost",
 ]
 UniprotkbProtocolsAndMaterials: TypeAlias = Literal[
     "xref_abcd", "xref_antibodypedia", "xref_cptc", "xref_dnasu"
 ]
 UniprotkbGenomeAnnotation: TypeAlias = Literal[
@@ -787,15 +791,14 @@
     "xref_gramene",
     "xref_kegg",
     "xref_mane-select",
     "xref_patric",
     "xref_ucsc",
     "xref_vectorbase",
     "xref_wbparasite",
-    "xref_wbparasitetranscriptprotein",
 ]
 UniprotkbOrganismSpecific: TypeAlias = Literal[
     "xref_agr",
     "xref_arachnoserver",
     "xref_araport",
     "xref_cgd",
     "xref_ctd",
@@ -803,14 +806,16 @@
     "xref_disgenet",
     "xref_echobase",
     "xref_flybase",
     "xref_genecards",
     "xref_genereviews",
     "xref_hgnc",
     "xref_hpa",
+    "xref_ic4r",
+    "xref_japonicusdb",
     "xref_legiolist",
     "xref_leproma",
     "xref_mgi",
     "xref_mim",
     "xref_maizegdb",
     "xref_malacards",
     "xref_niagads",
@@ -856,18 +861,22 @@
 ]
 UniprotkbOther: TypeAlias = Literal[
     "xref_biogrid-orcs",
     "xref_chitars",
     "xref_evolutionarytrace",
     "xref_genewiki",
     "xref_genomernai",
+    "xref_orcid",
+    "xref_pgenn",
     "xref_phi-base",
     "xref_pro",
     "xref_pharos",
+    "xref_pubtator",
     "xref_rnact",
+    "xref_emind",
 ]
 UniprotkbGeneExpression: TypeAlias = Literal[
     "xref_bgee",
     "xref_cleanex",
     "xref_collectf",
     "xref_expressionatlas",
     "xref_genevisible",
@@ -875,24 +884,23 @@
 UniprotkbFamilyAndDomain: TypeAlias = Literal[
     "xref_cdd",
     "xref_disprot",
     "xref_gene3d",
     "xref_hamap",
     "xref_ideal",
     "xref_interpro",
+    "xref_ncbifam",
     "xref_panther",
     "xref_pirsf",
     "xref_prints",
     "xref_prosite",
     "xref_pfam",
-    "xref_prodom",
     "xref_sfld",
     "xref_smart",
     "xref_supfam",
-    "xref_tigrfams",
 ]
 UniprotkbFields: TypeAlias = Literal[
     UniprotkbNamesTaxonomy,
     UniprotkbSequences,
     UniprotkbFunction,
     UniprotkbMiscellaneous,
     UniprotkbInteraction,
```

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/uniref.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/uniref.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/generated_types/unirule.py` & `unipressed-1.3.0/unipressed/dataset/generated_types/unirule.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/keywords.py` & `unipressed-1.3.0/unipressed/dataset/keywords.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/search.py` & `unipressed-1.3.0/unipressed/dataset/search.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/taxonomy.py` & `unipressed-1.3.0/unipressed/dataset/taxonomy.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/uniparc.py` & `unipressed-1.3.0/unipressed/dataset/uniparc.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/uniprotkb.py` & `unipressed-1.3.0/unipressed/dataset/uniprotkb.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/dataset/unirule.py` & `unipressed-1.3.0/unipressed/dataset/unirule.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/id_mapping/core.py` & `unipressed-1.3.0/unipressed/id_mapping/core.py`

 * *Files identical despite different names*

### Comparing `unipressed-1.2.0/unipressed/id_mapping/types.py` & `unipressed-1.3.0/unipressed/id_mapping/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "HGNC",
     "LegioList",
     "Leproma",
     "MaizeGDB",
     "MGI",
     "MIM",
     "neXtProt",
+    "OpenTargets",
     "Orphanet",
     "PharmGKB",
     "PomBase",
     "PseudoCAP",
     "RGD",
     "SGD",
     "TubercuList",
@@ -163,14 +164,15 @@
     "HGNC",
     "LegioList",
     "Leproma",
     "MaizeGDB",
     "MGI",
     "MIM",
     "neXtProt",
+    "OpenTargets",
     "Orphanet",
     "PharmGKB",
     "PomBase",
     "PseudoCAP",
     "RGD",
     "SGD",
     "TubercuList",
```

### Comparing `unipressed-1.2.0/PKG-INFO` & `unipressed-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: unipressed
-Version: 1.2.0
+Version: 1.3.0
 Summary: Comprehensive Python client for the Uniprot REST API
 Home-page: https://multimeric.github.io/Unipressed
 License: MIT
 Author: Michael Milton
 Author-email: michael.r.milton@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: mkdocstrings-python (>=1.10.2,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Project-URL: Repository, https://github.com/multimeric/Unipressed
 Description-Content-Type: text/markdown
 
 # Unipressed
```

