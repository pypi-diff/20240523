# Comparing `tmp/pgscatalog_core-0.1.1.tar.gz` & `tmp/pgscatalog_core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_core-0.1.1.tar", max compression
+gzip compressed data, was "pgscatalog_core-0.1.2.tar", max compression
```

## Comparing `pgscatalog_core-0.1.1.tar` & `pgscatalog_core-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1907 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/README.md
--rw-r--r--   0        0        0     1199 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1553 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/__init__.py
--rw-r--r--   0        0        0     1946 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/_combine.py
--rwxr-xr-x   0        0        0     5858 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/combine_cli.py
--rwxr-xr-x   0        0        0     4907 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/download_cli.py
--rw-r--r--   0        0        0     3054 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/cli/relabel_cli.py
--rw-r--r--   0        0        0     1485 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/__init__.py
--rw-r--r--   0        0        0      910 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_config.py
--rw-r--r--   0        0        0     5499 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_download.py
--rw-r--r--   0        0        0    14151 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_normalise.py
--rw-r--r--   0        0        0     2876 2024-04-09 09:23:41.215807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_read.py
--rw-r--r--   0        0        0     5581 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_relabel.py
--rw-r--r--   0        0        0    13836 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/catalogapi.py
--rw-r--r--   0        0        0     1585 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/genomebuild.py
--rw-r--r--   0        0        0     4620 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/pgsexceptions.py
--rw-r--r--   0        0        0    33063 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorefiles.py
--rw-r--r--   0        0        0     7546 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorevariant.py
--rw-r--r--   0        0        0     7538 2024-04-09 09:23:41.219807 pgscatalog_core-0.1.1/src/pgscatalog/core/lib/targetvariants.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pgscatalog_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1907 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/README.md
+-rw-r--r--   0        0        0     1199 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1576 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/cli/__init__.py
+-rw-r--r--   0        0        0     1946 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/cli/_combine.py
+-rwxr-xr-x   0        0        0     5906 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/cli/combine_cli.py
+-rwxr-xr-x   0        0        0     4907 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/cli/download_cli.py
+-rw-r--r--   0        0        0     3054 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/cli/relabel_cli.py
+-rw-r--r--   0        0        0     1485 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/__init__.py
+-rw-r--r--   0        0        0      909 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_config.py
+-rw-r--r--   0        0        0     5499 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_download.py
+-rw-r--r--   0        0        0    14358 2024-05-23 14:56:55.468650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_normalise.py
+-rw-r--r--   0        0        0     2876 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_read.py
+-rw-r--r--   0        0        0     5582 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_relabel.py
+-rw-r--r--   0        0        0    13835 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/catalogapi.py
+-rw-r--r--   0        0        0     1585 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/genomebuild.py
+-rw-r--r--   0        0        0     4620 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/pgsexceptions.py
+-rw-r--r--   0        0        0    33063 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/scorefiles.py
+-rw-r--r--   0        0        0     7547 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/scorevariant.py
+-rw-r--r--   0        0        0     7538 2024-05-23 14:56:55.472650 pgscatalog_core-0.1.2/src/pgscatalog/core/lib/targetvariants.py
+-rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 pgscatalog_core-0.1.2/PKG-INFO
```

### Comparing `pgscatalog_core-0.1.1/README.md` & `pgscatalog_core-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.1/pyproject.toml` & `pgscatalog_core-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgscatalog.core"
-version = "0.1.1"
+version = "0.1.2"
 description = "Core tools for working with polygenic scores (PGS) and the PGS Catalog"
 license = "Apache-2.0"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 readme = "README.md"
 packages = [
     { include = "pgscatalog", from = "src" },
 ]
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/__init__.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,7 +69,9 @@
     "TargetVariants",
     "NormalisedScoringFile",
     "EffectType",
     "RelabelArgs",
     "relabel",
     "relabel_write",
 ]
+
+__version__ = "0.1.2"
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/_combine.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/cli/_combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" This module contains functions useful for normalising scoring files into a
+"""This module contains functions useful for normalising scoring files into a
 standardised format, combining them, and calculating some statistics. Only really
 useful for the CLI, not good for importing elsewhere."""
+
 import collections
 import csv
 import functools
 import gzip
 import logging
 import os
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/combine_cli.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/cli/combine_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,26 @@
         if not chain_dir.exists():
             logger.critical(f"Chain directory is missing: {chain_dir}")
             raise FileNotFoundError
 
         liftover_kwargs = {
             "liftover": True,
             "chain_dir": chain_dir,
-            "target_build": target_build,
         }
     else:
         liftover_kwargs = {"liftover": False}
 
     for scorefile in tqdm(scoring_files, total=len(scoring_files)):
         logger.info(f"Processing {scorefile.pgs_id}")
         normalised_score = list(
-            scorefile.normalise(drop_missing=args.drop_missing, **liftover_kwargs)
+            scorefile.normalise(
+                drop_missing=args.drop_missing,
+                **liftover_kwargs,
+                target_build=target_build,
+            )
         )
         # TODO: go back to concurrent execution + write to multiple files
         writer = TextFileWriter(compress=compress_output, filename=out_path)
         writer.write(normalised_score)
         variant_log.append(get_variant_log(normalised_score))
 
     score_log = []
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/download_cli.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/cli/relabel_cli.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/cli/relabel_cli.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/__init__.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_config.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" This module managers global package configuration"""
+"""This module managers global package configuration"""
 
 import importlib.metadata
 import pathlib
 
 
 class Config:
     """This class stores global package configuration as class attributes
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_download.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" This module contains functions that simplify downloading data from the PGS Catalog.
+"""This module contains functions that simplify downloading data from the PGS Catalog.
 HTTPS download is preferred, with FTP fallback available.
 """
+
 import hashlib
 import logging
 import os
 import pathlib
 import tempfile
 import urllib
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_normalise.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_normalise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" This module contains a data processing pipeline to format ScoreVariants in a
+"""This module contains a data processing pipeline to format ScoreVariants in a
 standard way. Each step in the data processing pipeline is a generator that operates
 on a list of ScoreVariants and yields updated ScoreVariants. This makes it easy to
 plug in extra steps where needed, and lazily works on millions of objects."""
 
 import logging
 import pathlib
 
@@ -35,15 +35,15 @@
             current_build=scoring_file.genome_build,
             target_build=target_build,
             chain_dir=chain_dir,
         )
     else:
         variants = scoring_file.variants
 
-    variants = remap_harmonised(variants, scoring_file.harmonised)
+    variants = remap_harmonised(variants, scoring_file.harmonised, target_build)
     variants = check_bad_variant(variants, drop_missing)
 
     if drop_missing:
         variants = drop_hla(variants)
 
     variants = assign_effect_type(variants)
     variants = check_effect_weight(variants)
@@ -199,34 +199,36 @@
                 variant.effect_type = EffectType.RECESSIVE
             case _:
                 logger.critical(f"Bad effect type setting: {variant}")
                 raise Exception
         yield variant
 
 
-def remap_harmonised(variants, harmonised):
+def remap_harmonised(variants, harmonised, target_build):
     """
     Overwrite key attributes with harmonised data, if available.
 
     In this case chr_name, chr_position, and other allele are missing.
     Perhaps authors submitted rsID and effect allele originally:
 
     >>> variant = ScoreVariant(**{"effect_allele": "A", "effect_weight": 5, "accession": "test", "row_nr": 0, "hm_chr": 1, "hm_pos": 100, "hm_inferOtherAllele": "A"})
-    >>> list(remap_harmonised([variant], harmonised=True)) # doctest: +ELLIPSIS
+    >>> list(remap_harmonised([variant], harmonised=True, target_build=GenomeBuild.GRCh38)) # doctest: +ELLIPSIS
     [ScoreVariant(...,chr_name=1,chr_position=100,...other_allele='A'...)]
     """
     if harmonised:
         for variant in variants:
             # using the harmonised field in the header to make sure we don't accidentally overwrite
             # positions with empty data (e.g. in an unharmonised file)
             # if harmonisation has failed we _always_ want to use that information
             variant.chr_name = variant.hm_chr
             variant.chr_position = variant.hm_pos
             if variant.other_allele is None:
                 variant.other_allele = variant.hm_inferOtherAllele
+            # update the accession to reflect the harmonised data
+            variant.accession = f"{variant.accession}_hmPOS_{str(target_build)}"
             yield variant
     else:
         for variant in variants:
             # can't remap, so don't try
             yield variant
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_read.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains functions for reading data from PGS Catalog files.
-These functions aren't really meant to be imported outside corelib """
+These functions aren't really meant to be imported outside corelib"""
+
 import logging
 import pathlib
 
 from xopen import xopen
 
 from .scorevariant import ScoreVariant
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/_relabel.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/_relabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def _read_map(in_map, col_from, col_to):
     """Read a column from a mapping file into a dictionary"""
     mapping = {}
     logger.debug(f"Reading map {in_map}")
     with xopen(in_map) as map_f:
-        reader = csv.DictReader(map_f, delimiter=" ")
+        reader = csv.DictReader(map_f, delimiter="\t")
         for line in reader:
             mapping[line[col_from]] = line[col_to]
 
     return mapping
 
 
 def _read_maps(map_list, col_from, col_to):
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/catalogapi.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/catalogapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-""" Classes and functions related to the PGS Catalog API """
+"""Classes and functions related to the PGS Catalog API"""
+
 import enum
 import logging
 
 import httpx
 import tenacity
 
 from .pgsexceptions import QueryError, InvalidAccessionError
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/genomebuild.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/genomebuild.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/pgsexceptions.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/pgsexceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" This module defines a custom PGS exception hierarchy.
+"""This module defines a custom PGS exception hierarchy.
 
 This module overrides sys.excepthook. Uncaught exceptions are intercepted,
 and ``sys.exit()`` is called with a custom code. This can be helpful to debug
 problems in other applications, because there are relatively few failure states.
 
 The hierarchy:
 
@@ -39,14 +39,15 @@
   - SamplesheetError
 
     - GenomesNotFound
 
     - SamplesheetFormatError
 
 """
+
 import sys
 from types import MappingProxyType
 
 
 class BasePGSException(Exception):
     """The base class from which all PGS errors must inherit.
     The purpose of this class is to simplify finding PGS exceptions and exiting python
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorefiles.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/scorefiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" This module contains classes to compose and contain a ``ScoringFile``: a file
+"""This module contains classes to compose and contain a ``ScoringFile``: a file
 in the PGS Catalog that contains a list of genetic variants and their effect weights.
 Scoring files are used to calculate PGS for new target genomes."""
+
 import csv
 import itertools
 import logging
 import pathlib
 
 from xopen import xopen
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/scorevariant.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/scorevariant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains classes that compose a ScoreVariant: a variant in a PGS
 Catalog Scoring File."""
+
 from enum import Enum
 from typing import Optional
 
 
 class EffectAllele:
     """A class that represents an effect allele found in PGS Catalog scoring files
```

### Comparing `pgscatalog_core-0.1.1/src/pgscatalog/core/lib/targetvariants.py` & `pgscatalog_core-0.1.2/src/pgscatalog/core/lib/targetvariants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" This module contains classes to work with target variants. When a scoring file is
+"""This module contains classes to work with target variants. When a scoring file is
 being reused to calculate scores for new genotypes, the new genotypes are target
 genomes."""
+
 import enum
 import csv
 import itertools
 import pathlib
 
 from xopen import xopen
```

### Comparing `pgscatalog_core-0.1.1/PKG-INFO` & `pgscatalog_core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgscatalog.core
-Version: 0.1.1
+Version: 0.1.2
 Summary: Core tools for working with polygenic scores (PGS) and the PGS Catalog
 License: Apache-2.0
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

