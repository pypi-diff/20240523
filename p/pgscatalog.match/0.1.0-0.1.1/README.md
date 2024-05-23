# Comparing `tmp/pgscatalog_match-0.1.0.tar.gz` & `tmp/pgscatalog_match-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgscatalog_match-0.1.0.tar", max compression
+gzip compressed data, was "pgscatalog_match-0.1.1.tar", max compression
```

## Comparing `pgscatalog_match-0.1.0.tar` & `pgscatalog_match-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1096 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/README.md
--rw-r--r--   0        0        0      969 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      539 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/cli/__init__.py
--rw-r--r--   0        0        0      892 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/cli/_config.py
--rw-r--r--   0        0        0     1855 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/cli/_write.py
--rw-r--r--   0        0        0    11575 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/cli/match_cli.py
--rw-r--r--   0        0        0     6230 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/cli/merge_cli.py
--rw-r--r--   0        0        0      522 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/__init__.py
--rw-r--r--   0        0        0      587 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_arrow.py
--rw-r--r--   0        0        0      114 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_config.py
--rw-r--r--   0        0        0        0 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/__init__.py
--rw-r--r--   0        0        0     3259 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/filter.py
--rw-r--r--   0        0        0    13783 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/label.py
--rw-r--r--   0        0        0     4181 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/log.py
--rw-r--r--   0        0        0     4884 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/match.py
--rw-r--r--   0        0        0     4883 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/plink.py
--rw-r--r--   0        0        0     2141 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/preprocess.py
--rw-r--r--   0        0        0     3052 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_plinkframe.py
--rw-r--r--   0        0        0    12763 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/matchresult.py
--rw-r--r--   0        0        0     3534 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/plinkscorefiles.py
--rw-r--r--   0        0        0     4866 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/scoringfileframe.py
--rw-r--r--   0        0        0     3204 2024-03-22 14:44:12.243661 pgscatalog_match-0.1.0/src/pgscatalog/match/lib/variantframe.py
--rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 pgscatalog_match-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/README.md
+-rw-r--r--   0        0        0     1043 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      562 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/_config.py
+-rw-r--r--   0        0        0     2165 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/_write.py
+-rw-r--r--   0        0        0    14935 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/intersect_cli.py
+-rw-r--r--   0        0        0    12325 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/match_cli.py
+-rw-r--r--   0        0        0     6896 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/cli/merge_cli.py
+-rw-r--r--   0        0        0      522 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_arrow.py
+-rw-r--r--   0        0        0      114 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_config.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/__init__.py
+-rw-r--r--   0        0        0     3259 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/filter.py
+-rw-r--r--   0        0        0    14078 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/label.py
+-rw-r--r--   0        0        0     4181 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/log.py
+-rw-r--r--   0        0        0     4884 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/match.py
+-rw-r--r--   0        0        0     5004 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/plink.py
+-rw-r--r--   0        0        0     2131 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/preprocess.py
+-rw-r--r--   0        0        0     3181 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_plinkframe.py
+-rw-r--r--   0        0        0    12942 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/matchresult.py
+-rw-r--r--   0        0        0     3542 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/plinkscorefiles.py
+-rw-r--r--   0        0        0     4866 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/scoringfileframe.py
+-rw-r--r--   0        0        0     3204 2024-05-23 15:04:03.860663 pgscatalog_match-0.1.1/src/pgscatalog/match/lib/variantframe.py
+-rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 pgscatalog_match-0.1.1/PKG-INFO
```

### Comparing `pgscatalog_match-0.1.0/README.md` & `pgscatalog_match-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/pyproject.toml` & `pgscatalog_match-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgscatalog.match"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tools for matching variants in PGS scoring files and target variant information files"
 authors = ["Benjamin Wingfield <bwingfield@ebi.ac.uk>", "Samuel Lambert <sl925@medschl.cam.ac.uk>", "Laurent Gil <lg10@sanger.ac.uk>"]
 readme = "README.md"
 packages = [
     { include = "pgscatalog", from = "src" },
 ]
 
@@ -13,14 +13,15 @@
 "pgscatalog.core" = "^0.1.0"
 polars = "^0.20.5"
 pyarrow = "^15.0.0"
 
 [tool.poetry.scripts]
 pgscatalog-match = 'pgscatalog.match.cli.match_cli:run_match'
 pgscatalog-matchmerge = 'pgscatalog.match.cli.merge_cli:run_merge'
+pgscatalog-intersect = 'pgscatalog.match.cli.intersect_cli:run_intersect'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/__init__.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 
-from .lib.variantframe import VariantFrame
-from .lib.scoringfileframe import ScoringFileFrame, match_variants
-from .lib.matchresult import MatchResult, MatchResults
-from .lib.plinkscorefiles import PlinkScoreFiles
-
+from .variantframe import VariantFrame
+from .scoringfileframe import ScoringFileFrame, match_variants
+from .matchresult import MatchResult, MatchResults
+from .plinkscorefiles import PlinkScoreFiles
 
 log_fmt = "%(name)s: %(asctime)s %(levelname)-8s %(message)s"
 logging.basicConfig(format=log_fmt, datefmt="%Y-%m-%d %H:%M:%S")
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "VariantFrame",
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/cli/_config.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/cli/_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" This module contains a simple class that stores CLI configuration as class attributes """
+"""This module contains a simple class that stores CLI configuration as class attributes"""
 
 
 class Config:
     # what's the label for the target variants data?
     DATASET = None
     # where do scorefiles get written to?
     OUTDIR = None
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/cli/_write.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/cli/_write.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,55 @@
-""" This module contains internal functions for writing match results to scoring files and logs
+"""This module contains internal functions for writing match results to scoring files and logs
 
 It expects Config class attributes to be set up before being called
 """
+
 import gzip
 import itertools
 
+from pgscatalog.core import MatchRateError
+
 from ..lib.plinkscorefiles import PlinkScoreFiles
 
 from ._config import Config
 
 
 def write_matches(matchresults, score_df):
     """Write matchresults out to scoring files and logs"""
-    match (Config.SPLIT, Config.COMBINED):
-        case (True, True):
-            # requires extra work: first write split
-            outfs = matchresults.write_scorefiles(
-                directory=Config.OUTDIR,
-                split=True,
-                score_df=score_df,
-                min_overlap=Config.MIN_OVERLAP,
-                **Config.MATCH_PARAMS,
-            )
-            # now re-combine without recomputing matches
-            PlinkScoreFiles(*list(itertools.chain(*outfs))).merge(Config.OUTDIR)
-        case (True, False) | (False, True):
-            # split parameter can handle this case OK
-            _ = matchresults.write_scorefiles(
-                directory=Config.OUTDIR,
-                split=Config.SPLIT,
-                score_df=score_df,
-                min_overlap=Config.MIN_OVERLAP,
-                **Config.MATCH_PARAMS,
-            )
-        case _:
-            raise ValueError
+    try:
+        match (Config.SPLIT, Config.COMBINED):
+            case (True, True):
+                # requires extra work: first write split
+                outfs = matchresults.write_scorefiles(
+                    directory=Config.OUTDIR,
+                    split=True,
+                    score_df=score_df,
+                    min_overlap=Config.MIN_OVERLAP,
+                    **Config.MATCH_PARAMS,
+                )
+                # now re-combine without recomputing matches
+                PlinkScoreFiles(*list(itertools.chain(*outfs))).merge(Config.OUTDIR)
+            case (True, False) | (False, True):
+                # split parameter can handle this case OK
+                _ = matchresults.write_scorefiles(
+                    directory=Config.OUTDIR,
+                    split=Config.SPLIT,
+                    score_df=score_df,
+                    min_overlap=Config.MIN_OVERLAP,
+                    **Config.MATCH_PARAMS,
+                )
+            case _:
+                raise ValueError
+    except MatchRateError as e:
+        # write logs in case of errors
+        write_log(matchresults=matchresults, score_df=score_df)
+        raise e
+    else:
+        write_log(matchresults=matchresults, score_df=score_df)
 
-    write_log(matchresults=matchresults, score_df=score_df)
     # returns labelled and filtered data for checking after merging
     return matchresults.df
 
 
 def write_log(matchresults, score_df):
     logfname = Config.OUTDIR / f"{Config.DATASET}_log.csv.gz"
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/cli/match_cli.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/cli/match_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import argparse
 import atexit
 import logging
 import pathlib
+import shutil
 import sys
 import tempfile
 import textwrap
 
 import polars as pl
 
 from ..lib import (
@@ -20,37 +21,45 @@
 from ._write import write_matches
 
 logger = logging.getLogger(__name__)
 
 
 def _exit(cleanup):
     if cleanup:
-        # should already be emptied by context managers
-        Config.TMPDIR.rmdir()
+        if Config.TMPDIR and Config.TMPDIR.exists():
+            shutil.rmtree(Config.TMPDIR)
+        if Config.MATCHTMP and Config.MATCHTMP.exists():
+            shutil.rmtree(Config.MATCHTMP)
 
 
 def run_match():
-    atexit.register(_exit, cleanup=Config.CLEANUP)
     args = parse_args()
 
     if args.verbose:
         logging.getLogger("pgscatalog.core").setLevel(logging.DEBUG)
         logging.getLogger("pgscatalog.match").setLevel(logging.DEBUG)
         logger.setLevel(logging.DEBUG)
         logger.debug("Verbose logging enabled")
 
     Config.DATASET = args.dataset
-    Config.CLEANUP = False
+    Config.CLEANUP = args.cleanup
     Config.OUTDIR = pathlib.Path(args.outdir)
 
     Config.SCOREFILE = pathlib.Path(args.scorefile)
 
     if not Config.OUTDIR.exists():
         raise FileNotFoundError(f"{Config.OUTDIR} does not exist")
 
+    atexit.register(_exit, cleanup=Config.CLEANUP)
+
+    if Config.CLEANUP:
+        logger.info("--cleanup set (default), temporary files will be deleted")
+    else:
+        logger.info("--no-cleanup set, temporary files won't be deleted")
+
     Config.MATCHTMP = Config.OUTDIR / "matchtmp"
     Config.MATCHTMP.mkdir(exist_ok=False)
     Config.TMPDIR = Config.OUTDIR / "tmp"
     Config.TMPDIR.mkdir(exist_ok=False)
     Config.CHROM = args.chrom
     Config.MIN_OVERLAP = args.min_overlap
 
@@ -87,22 +96,29 @@
             matchresults.append(
                 MatchResult.from_ipc(
                     matchresults_ipc_path=ipc_path, dataset=Config.DATASET
                 )
             )
 
         if args.only_match:
+            for i, match in enumerate(matchresults):
+                ipc_path = pathlib.Path(match.ipc_path)
+                out_path = Config.OUTDIR / f"{i}.ipc.zst"
+                logger.info(f"Renaming {ipc_path} to {out_path}")
+                ipc_path.rename(out_path)
+
             logger.warning("--only_match set, exiting with grace and aplomb")
             logger.warning(
                 f"You'll need to combine match candidates using the Arrow IPC files in {Config.OUTDIR}"
             )
-            sys.exit()
+            return
         else:
             matchresults = MatchResults(*matchresults)
             _ = write_matches(matchresults=matchresults, score_df=score_df)
+    logger.info("finished matching :)")
 
 
 def get_match_candidates(target, score_df, chrom, dataset, **kwargs):
     # don't clean this up, useful for debugging
     _, fout = tempfile.mkstemp(dir=Config.MATCHTMP)  # file names don't matter
     variants = VariantFrame(path=target, chrom=chrom, dataset=dataset, **kwargs)
     with variants as target_df:
@@ -189,14 +205,17 @@
     parser.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         action="store_true",
         help="<Optional> Extra logging information",
     )
+    parser.add_argument(
+        "--cleanup", dest="cleanup", default=True, action=argparse.BooleanOptionalAction
+    )
     # variant matching arguments -------------------------------------------------------
     parser.add_argument(
         "--keep_ambiguous",
         dest="remove_ambiguous",
         action="store_false",
         help="""<Optional> Flag to force the program to keep variants with
                         ambiguous alleles, (e.g. A/T and G/C SNPs), which are normally
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/cli/merge_cli.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/cli/merge_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 import argparse
+import atexit
 import logging
 import pathlib
+import shutil
 
 from ._config import Config
 from ._write import write_matches
 
 from ..lib import ScoringFileFrame, MatchResult, MatchResults
 
 import polars as pl
 
 logger = logging.getLogger(__name__)
 
 
+def _exit(cleanup):
+    if cleanup:
+        if Config.TMPDIR and Config.TMPDIR.exists():
+            shutil.rmtree(Config.TMPDIR)
+        if Config.MATCHTMP and Config.MATCHTMP.exists():
+            shutil.rmtree(Config.MATCHTMP)
+
+
 def run_merge():
     args = parse_args()
 
     if args.verbose:
         logging.getLogger("pgscatalog.core").setLevel(logging.DEBUG)
         logging.getLogger("pgscatalog.match").setLevel(logging.DEBUG)
         logger.setLevel(logging.DEBUG)
         logger.debug("Verbose logging enabled")
 
     Config.DATASET = args.dataset
-    Config.CLEANUP = False
+    Config.CLEANUP = args.cleanup
     Config.OUTDIR = pathlib.Path(args.outdir)
     Config.SCOREFILE = pathlib.Path(args.scorefile)
 
     if not Config.OUTDIR.exists():
         raise FileNotFoundError(f"{Config.OUTDIR} does not exist")
 
+    atexit.register(_exit, cleanup=Config.CLEANUP)
+
+    if Config.CLEANUP:
+        logger.info("--cleanup set (default), temporary files will be deleted")
+    else:
+        logger.info("--no-cleanup set, temporary files won't be deleted")
+
     Config.TMPDIR = Config.OUTDIR / "tmp"
     Config.TMPDIR.mkdir(exist_ok=False)
 
     # parameters that control how the best match candidate is chosen
     # missing parameters will be set to defaults specified in matchlib
     Config.MATCH_PARAMS = {
         k: v for k in Config.MATCH_KWARGS if (v := getattr(args, k)) is not None
@@ -48,14 +65,15 @@
         tmpdir=Config.TMPDIR,
     ) as score_df, pl.StringCache():
         matchresults = MatchResults(
             *(MatchResult.from_ipc(x, dataset=Config.DATASET) for x in args.matches)
         )
         matchdf = write_matches(matchresults=matchresults, score_df=score_df)
         _check_duplicate_vars(matchdf)
+    logger.info("finished merging :)")
 
 
 def _check_duplicate_vars(matches):
     max_occurrence = (
         matches.filter(pl.col("match_status") == "matched")
         .group_by(["accession", "ID"])
         .len()
@@ -141,14 +159,17 @@
     parser.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         action="store_true",
         help="<Optional> Extra logging information",
     )
+    parser.add_argument(
+        "--cleanup", dest="cleanup", default=True, action=argparse.BooleanOptionalAction
+    )
     # variant matching arguments -------------------------------------------------------
     parser.add_argument(
         "--keep_ambiguous",
         dest="remove_ambiguous",
         action="store_false",
         help="""<Optional> Flag to force the program to keep variants with
                         ambiguous alleles, (e.g. A/T and G/C SNPs), which are normally
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/__init__.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import logging
 
-from .variantframe import VariantFrame
-from .scoringfileframe import ScoringFileFrame, match_variants
-from .matchresult import MatchResult, MatchResults
-from .plinkscorefiles import PlinkScoreFiles
+from .lib.variantframe import VariantFrame
+from .lib.scoringfileframe import ScoringFileFrame, match_variants
+from .lib.matchresult import MatchResult, MatchResults
+from .lib.plinkscorefiles import PlinkScoreFiles
+
 
 log_fmt = "%(name)s: %(asctime)s %(levelname)-8s %(message)s"
 logging.basicConfig(format=log_fmt, datefmt="%Y-%m-%d %H:%M:%S")
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "VariantFrame",
     "ScoringFileFrame",
     "MatchResult",
     "MatchResults",
     "PlinkScoreFiles",
     "match_variants",
 ]
+
+__version__ = "0.1.1"
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_arrow.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_arrow.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/filter.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-""" This module contains functions to filter match candidates and report overall match rates"""
+"""This module contains functions to filter match candidates and report overall match rates"""
+
 import logging
 
 import polars as pl
 
 logger = logging.getLogger(__name__)
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/label.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/label.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-""" This module labels match candidates with various flag columns, with the aim of
+"""This module labels match candidates with various flag columns, with the aim of
 producing a final set of best match candidates (one maximum for each variant).
 
 These operations are all quite data-framey and involve calculating a horizontal
 maximum across boolean columns to determine if a variant should be given a true value
 in an exclude column.
 """
 
 import logging
+import pathlib
 
 import polars as pl
+from xopen import xopen
 
 from .preprocess import complement_valid_alleles
 
 logger = logging.getLogger(__name__)
 
 
 def label_matches(
@@ -297,22 +299,27 @@
             .alias("exclude")
         )
     else:
         logger.debug("Not excluding flipped matches")
         return df.with_columns(match_IDs=pl.lit("NA"))
 
 
-def _label_filter(df: pl.LazyFrame, filter_IDs: list) -> pl.LazyFrame:
+def _label_filter(df: pl.LazyFrame, filter_IDs: pathlib.Path) -> pl.LazyFrame:
     if filter_IDs is not None:
-        nIDs = len(filter_IDs)
+        logger.debug("Reading filter file (variant IDs)")
+        with xopen(filter_IDs, "r") as f:
+            filt_series = pl.Series([line.strip() for line in f], dtype=pl.Utf8)
+
+        nIDs = len(filt_series)
         logger.debug(
             "Excluding variants that are not in ID list (read {} IDs)".format(nIDs)
         )
-        df = df.with_columns(pl.col("ID").is_in(filter_IDs).alias("match_IDs"))
+        df = df.with_columns(pl.col("ID").is_in(filt_series).alias("match_IDs"))
         return df.with_columns(
-            pl.when(pl.col("match_IDs"))
+            pl.when(~pl.col("match_IDs"))
             .then(True)
             .otherwise(pl.col("exclude"))
             .alias("exclude")
         )
     else:
+        logger.info("--filter_IDs not set, skipping filtering")
         return df
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/log.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/log.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/match.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/match.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/plink.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/plink.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,24 @@
 def pivot_score(df: pl.DataFrame) -> pl.DataFrame:
     """Format a dataframe to plink2 --score standard
     Minimum example:
     ID | effect_allele | effect_weight
     Multiple scores are OK too:
     ID | effect_allele | weight_1 | ... | weight_n
     """
+    # fill_null: value = 0 not strategy = "zero"
+    # we always handle effect weights as strings because we never modify them
     return (
         df.pivot(
             index=["ID", "matched_effect_allele", "effect_type"],
             values="effect_weight",
             columns="accession",
         )
         .rename({"matched_effect_allele": "effect_allele"})
-        .fill_null(strategy="zero")
+        .fill_null(value="0")
         .drop("effect_type")
     )
 
 
 def _check_column_types(matches: pl.LazyFrame):
     logger.debug("Checking column types")
     # these columns are most important for writing out
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_match/preprocess.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_match/preprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,11 +49,11 @@
         .alias("is_multiallelic")
     )
 
     if (
         df.select("is_multiallelic").unique().collect().get_column("is_multiallelic")
     ).any():
         logger.debug("Exploding dataframe to handle multiallelic variants")
-        return df.with_columns(pl.col("ALT").str.split_and_pivot(by=",")).explode("ALT")
+        return df.with_columns(pl.col("ALT").str.split(by=",")).explode("ALT")
     else:
         logger.debug("No multiallelic variants detected")
         return df
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/_plinkframe.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/_plinkframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-""" This module contains internal classes that store matched variants and format them
+"""This module contains internal classes that store matched variants and format them
 to be compatible with plink2 --score
 """
+
 import collections.abc
 import gzip
 import pathlib
 
 from ._match.plink import plinkify, pivot_score
 
 
@@ -78,10 +79,14 @@
 
     @classmethod
     def from_matchresult(cls, matchresult):
         effect_types = plinkify(matchresult)
         plinkframes = []
         for effect_type, dataframes in effect_types.items():
             for i, df in enumerate(dataframes):
-                plinkframes.append(PlinkFrame(effect_type=effect_type, n=i, df=df))
+                df = df.collect()
+                if not df.is_empty():
+                    plinkframes.append(
+                        PlinkFrame(effect_type=effect_type, n=i, df=df.lazy())
+                    )
 
         return cls(*plinkframes)
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/matchresult.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/matchresult.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,20 +252,14 @@
         """
         if not self._labelled:
             _ = self.label(**kwargs)  # self.df gets updated
 
         if not self._filtered:
             _ = self.filter(score_df=score_df, min_overlap=min_overlap)
 
-        if not all(x[1] for x in self.filter_summary.iter_rows()):
-            logger.warning(f"{self.filter_summary}")
-            raise MatchRateError(
-                f"All scores fail to meet match threshold {min_overlap}"
-            )
-
         # a summary log contains up to one variant (the best match) for each variant
         # in the scoring file
         self.summary_log = make_summary_log(
             match_candidates=self.df,
             dataset=self.dataset,
             filter_summary=self.filter_summary.lazy(),
             scorefile=score_df,
@@ -278,14 +272,25 @@
         outfs = []
         for frame in plink:
             f = frame.write(directory=directory, split=split, dataset=self.dataset)
             outfs.append(f)
 
         # collect after joining in check_log_count (can't join df and lazy df)
         self.summary_log = self.summary_log.collect()
+
+        # error at the end, to allow logs to be generated
+        if not all(x[1] for x in self.filter_summary.iter_rows()):
+            logger.warning(f"{self.filter_summary}")
+            [
+                x.unlink() for xs in outfs for x in xs
+            ]  # don't provide dodgy scoring files
+            raise MatchRateError(
+                f"All scores fail to meet match threshold {min_overlap}"
+            )
+
         return outfs
 
     def full_variant_log(self, score_df, **kwargs):
         """Generate a log for each variant in a scoring file
 
         Multiple match candidates may exist for each variant in the original file.
         Describe each variant (one variant per row) with match metadata
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/plinkscorefiles.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/plinkscorefiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-""" This module contains the PlinkScoreFiles class, which represents one or more
+"""This module contains the PlinkScoreFiles class, which represents one or more
 scoring files ready to be used with plink2 --score"""
+
 import collections.abc
 import gzip
 import io
 import itertools
 import pathlib
 
 import polars as pl
 
 
 class PlinkScoreFiles(collections.abc.Sequence):
     """Represents a sequence of scoring files files written by :class:`MatchResults`"""
 
     def __init__(self, *elements):
-        self._elements = [pathlib.Path(x) for x in list(elements)]
+        self._elements = [pathlib.Path(x) for x in sorted(list(elements))]
 
     def __len__(self):
         return len(self._elements)
 
     def __getitem__(self, item):
         return self._elements[item]
```

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/scoringfileframe.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/scoringfileframe.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/src/pgscatalog/match/lib/variantframe.py` & `pgscatalog_match-0.1.1/src/pgscatalog/match/lib/variantframe.py`

 * *Files identical despite different names*

### Comparing `pgscatalog_match-0.1.0/PKG-INFO` & `pgscatalog_match-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgscatalog.match
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for matching variants in PGS scoring files and target variant information files
 Author: Benjamin Wingfield
 Author-email: bwingfield@ebi.ac.uk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

