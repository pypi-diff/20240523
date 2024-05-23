# Comparing `tmp/sosap-0.1.3.tar.gz` & `tmp/sosap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosap-0.1.3.tar", last modified: Thu May  2 03:10:35 2024, max compression
+gzip compressed data, was "sosap-0.2.0.tar", last modified: Thu May 23 03:55:07 2024, max compression
```

## Comparing `sosap-0.1.3.tar` & `sosap-0.2.0.tar`

### file list

```diff
@@ -1,164 +1,161 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.895029 sosap-0.1.3/
--rw-r--r--   0 seanghay   (501) staff       (20)     1095 2024-05-02 02:14:09.000000 sosap-0.1.3/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)       23 2024-05-02 02:49:00.000000 sosap-0.1.3/MANIFEST.in
--rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 03:10:35.894800 sosap-0.1.3/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      453 2024-05-02 02:14:09.000000 sosap-0.1.3/README.md
--rw-r--r--   0 seanghay   (501) staff       (20)      770 2024-05-02 03:10:30.000000 sosap-0.1.3/pyproject.toml
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-02 03:10:35.895072 sosap-0.1.3/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)     1045 2024-05-02 03:09:30.000000 sosap-0.1.3/setup.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.873596 sosap-0.1.3/src/
--rw-r--r--   0 seanghay   (501) staff       (20)     6148 2024-05-02 02:43:16.000000 sosap-0.1.3/src/.DS_Store
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.871853 sosap-0.1.3/src/Phonetisaurus/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.871667 sosap-0.1.3/src/Phonetisaurus/3rdparty/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.873699 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.874278 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/
--rw-r--r--   0 seanghay   (501) staff       (20)    11960 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h
--rwxr-xr-x   0 seanghay   (501) staff       (20)    11769 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h
--rwxr-xr-x   0 seanghay   (501) staff       (20)     8640 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1521 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.875954 sosap-0.1.3/src/Phonetisaurus/include/
--rw-r--r--   0 seanghay   (501) staff       (20)    12608 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/ARPA2WFST.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2752 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/LatticePruner.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5322 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMDecodable.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5394 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMHash.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2257 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMReader.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5364 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/M2MFstAligner.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14648 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/PhonetisaurusRex.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7286 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/PhonetisaurusScript.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9986 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/RnnLMDecoder.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4859 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/RnnLMPy.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2492 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/include/util.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.876378 sosap-0.1.3/src/Phonetisaurus/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)     5283 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/lib/LatticePruner.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    21805 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/lib/M2MFstAligner.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     1850 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/lib/feature-reader.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     8616 2024-05-02 02:14:09.000000 sosap-0.1.3/src/Phonetisaurus/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)   328385 2024-05-02 03:09:39.000000 sosap-0.1.3/src/core.cpp
--rw-r--r--   0 seanghay   (501) staff       (20)      599 2024-05-02 02:45:21.000000 sosap-0.1.3/src/core.pyx
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.872058 sosap-0.1.3/src/openfst/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.872002 sosap-0.1.3/src/openfst/include/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.892640 sosap-0.1.3/src/openfst/include/fst/
--rw-r--r--   0 seanghay   (501) staff       (20)    29524 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/accumulator.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7442 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/add-on.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6405 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/arc-arena.h
--rw-r--r--   0 seanghay   (501) staff       (20)    39401 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/arc-map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     8353 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/arc.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2314 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/arcfilter.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6587 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/arcsort.h
--rw-r--r--   0 seanghay   (501) staff       (20)    15136 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/bi-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)    42957 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/cache.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4269 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/closure.h
--rw-r--r--   0 seanghay   (501) staff       (20)    52849 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/compact-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2749 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/compat.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7726 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/complement.h
--rw-r--r--   0 seanghay   (501) staff       (20)    19892 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/compose-filter.h
--rw-r--r--   0 seanghay   (501) staff       (20)    39087 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/compose.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7285 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/concat.h
--rw-r--r--   0 seanghay   (501) staff       (20)      414 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/config.h
--rw-r--r--   0 seanghay   (501) staff       (20)      333 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/config.h.in
--rw-r--r--   0 seanghay   (501) staff       (20)     9916 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/connect.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16266 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/const-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    40410 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/determinize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6673 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/dfs-visit.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6964 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/difference.h
--rw-r--r--   0 seanghay   (501) staff       (20)    20433 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/disambiguate.h
--rw-r--r--   0 seanghay   (501) staff       (20)    27698 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/edit-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    17732 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/encode.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2111 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/epsnormalize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6077 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/equal.h
--rw-r--r--   0 seanghay   (501) staff       (20)     8823 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/equivalent.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5394 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/expanded-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4511 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/expectation-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16699 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/factor-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4889 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/filter-state.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6664 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/flags.h
--rw-r--r--   0 seanghay   (501) staff       (20)    28674 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/float-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5232 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/fst-decl.h
--rw-r--r--   0 seanghay   (501) staff       (20)    30981 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3917 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/fstlib.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3709 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/generic-register.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4555 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/heap.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4574 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/icu.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5737 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/intersect.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12110 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/interval-set.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3893 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/invert.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5804 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/isomorphic.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18965 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/label-reachable.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5894 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/lexicographic-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1540 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/lock.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2254 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/log.h
--rw-r--r--   0 seanghay   (501) staff       (20)    23312 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/lookahead-filter.h
--rw-r--r--   0 seanghay   (501) staff       (20)    28489 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/lookahead-matcher.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2895 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3037 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/mapped-file.h
--rw-r--r--   0 seanghay   (501) staff       (20)    11433 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/matcher-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    51793 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/matcher.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12918 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/memory.h
--rw-r--r--   0 seanghay   (501) staff       (20)    21100 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/minimize.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12012 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/mutable-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4151 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/pair-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12588 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/partition.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4740 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/power-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3309 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/product-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4563 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/project.h
--rw-r--r--   0 seanghay   (501) staff       (20)    19044 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/properties.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13109 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/prune.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6039 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/push.h
--rw-r--r--   0 seanghay   (501) staff       (20)    29804 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/queue.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4145 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/randequivalent.h
--rw-r--r--   0 seanghay   (501) staff       (20)    25791 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/randgen.h
--rw-r--r--   0 seanghay   (501) staff       (20)    10110 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/rational.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3298 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/register.h
--rw-r--r--   0 seanghay   (501) staff       (20)    15947 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/relabel.h
--rw-r--r--   0 seanghay   (501) staff       (20)    22753 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/replace-util.h
--rw-r--r--   0 seanghay   (501) staff       (20)    56136 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/replace.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4243 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/reverse.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4877 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/reweight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18370 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/rmepsilon.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2536 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/rmfinalepsilon.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18358 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/set-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13204 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/shortest-distance.h
--rw-r--r--   0 seanghay   (501) staff       (20)    23200 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/shortest-path.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13538 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/signed-log-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6706 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/sparse-power-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12794 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/sparse-tuple-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18304 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/state-map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7175 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/state-reachable.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16830 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/state-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2192 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/statesort.h
--rw-r--r--   0 seanghay   (501) staff       (20)    25921 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/string-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9416 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/string.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3040 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/symbol-table-ops.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14016 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/symbol-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13573 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/synchronize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9443 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/test-properties.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2580 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/topsort.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4140 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/tuple-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1082 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/types.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2621 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/union-find.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14641 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/union-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5098 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/union.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12396 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/util.h
--rw-r--r--   0 seanghay   (501) staff       (20)    24671 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/vector-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3676 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/verify.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9330 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/visit.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12716 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/include/fst/weight.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.893932 sosap-0.1.3/src/openfst/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)      814 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/compat.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4819 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/flags.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     1231 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/fst-types.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4841 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/fst.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4136 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/mapped-file.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    17562 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/properties.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4193 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/symbol-table-ops.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    11312 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/symbol-table.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     2740 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     3929 2024-05-02 02:14:09.000000 sosap-0.1.3/src/openfst/lib/weight.cc
--rw-r--r--   0 seanghay   (501) staff       (20)      604 2024-05-02 02:14:09.000000 sosap-0.1.3/src/phonemizer.cc
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.894019 sosap-0.1.3/src/sosap/
--rw-r--r--   0 seanghay   (501) staff       (20)       32 2024-05-02 02:14:09.000000 sosap-0.1.3/src/sosap/__init__.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 03:10:35.894567 sosap-0.1.3/src/sosap.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 03:10:35.000000 sosap-0.1.3/src/sosap.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)     5174 2024-05-02 03:10:35.000000 sosap-0.1.3/src/sosap.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-02 03:10:35.000000 sosap-0.1.3/src/sosap.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       43 2024-05-02 03:10:35.000000 sosap-0.1.3/src/sosap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.210035 sosap-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 03:55:03.000000 sosap-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 03:55:03.000000 sosap-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 03:55:07.210035 sosap-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 03:55:03.000000 sosap-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-23 03:55:03.000000 sosap-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:55:07.210035 sosap-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 03:55:03.000000 sosap-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.186035 sosap-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.182036 sosap-0.2.0/src/Phonetisaurus/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.182036 sosap-0.2.0/src/Phonetisaurus/3rdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.186035 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.186035 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11769 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8640 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.186035 sosap-0.2.0/src/Phonetisaurus/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/ARPA2WFST.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/LatticePruner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMDecodable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMHash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/M2MFstAligner.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/PhonetisaurusRex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/PhonetisaurusScript.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/RnnLMDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/RnnLMPy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/include/util.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.186035 sosap-0.2.0/src/Phonetisaurus/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/lib/LatticePruner.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/lib/M2MFstAligner.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/lib/feature-reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-23 03:55:03.000000 sosap-0.2.0/src/Phonetisaurus/lib/util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 03:55:03.000000 sosap-0.2.0/src/core.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.182036 sosap-0.2.0/src/openfst/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.182036 sosap-0.2.0/src/openfst/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.206035 sosap-0.2.0/src/openfst/include/fst/
+-rw-r--r--   0 runner    (1001) docker     (127)    29524 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/accumulator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/add-on.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/arc-arena.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39401 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/arc-map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/arc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/arcfilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/arcsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/bi-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42957 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/cache.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/closure.h
+-rw-r--r--   0 runner    (1001) docker     (127)    52849 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/compact-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/complement.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19892 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/compose-filter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39087 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/compose.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/concat.h
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/connect.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/const-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/determinize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/dfs-visit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/difference.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/disambiguate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27698 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/edit-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/encode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/epsnormalize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/equal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/equivalent.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/expanded-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/expectation-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16699 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/factor-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/filter-state.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/flags.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/float-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/fst-decl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30981 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/fstlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/generic-register.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/icu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/intersect.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/interval-set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/invert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/isomorphic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/label-reachable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/lexicographic-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/lock.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23312 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/lookahead-filter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28489 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/lookahead-matcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/mapped-file.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/matcher-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)    51793 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/matcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/memory.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21100 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/minimize.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/mutable-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/pair-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12588 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/partition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/power-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/product-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/project.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/properties.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/prune.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/push.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29804 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/randequivalent.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/randgen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/rational.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/register.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15947 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/relabel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22753 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/replace-util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56136 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/replace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/reverse.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/reweight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/rmepsilon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/rmfinalepsilon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18358 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/set-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/shortest-distance.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23200 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/shortest-path.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/signed-log-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/sparse-power-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/sparse-tuple-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/state-map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/state-reachable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/state-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/statesort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25921 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/string-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/string.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/symbol-table-ops.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14016 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/symbol-table.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/synchronize.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/test-properties.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/topsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/tuple-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/union-find.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/union-weight.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/union.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/vector-fst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/verify.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/visit.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/include/fst/weight.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.210035 sosap-0.2.0/src/openfst/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/compat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/flags.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/fst-types.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/fst.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/mapped-file.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17562 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/properties.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/symbol-table-ops.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/symbol-table.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-23 03:55:03.000000 sosap-0.2.0/src/openfst/lib/weight.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.210035 sosap-0.2.0/src/sosap/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 03:55:03.000000 sosap-0.2.0/src/sosap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:55:07.210035 sosap-0.2.0/src/sosap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-23 03:55:07.000000 sosap-0.2.0/src/sosap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-23 03:55:07.000000 sosap-0.2.0/src/sosap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:55:07.000000 sosap-0.2.0/src/sosap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 03:55:07.000000 sosap-0.2.0/src/sosap.egg-info/top_level.txt
```

### Comparing `sosap-0.1.3/LICENSE` & `sosap-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/PKG-INFO` & `sosap-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sosap-0.1.3/pyproject.toml` & `sosap-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "Cython"]
+requires = ["setuptools>=67.4.0", "Cython>=0.29.33"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosap"
-version = "0.1.3"
+version = "0.2.0"
 authors = [{ name = "Seanghay Yath", email = "seanghay.dev@gmail.com" }]
 
 description = "Python binding for Phonetisaurus"
 readme = "README.md"
 requires-python = ">=3.7"
 
 classifiers = [
@@ -23,8 +23,15 @@
 [project.urls]
 repository = "https://github.com/seanghay/sosap"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
+
+[tool.cibuildwheel]
+# Setuptools bug causes collision between pypy and cpython artifacts
+before-build = "rm -rf {project}/build"
+
+[tool.cibuildwheel.linux]
+archs = ["auto64"]
```

### Comparing `sosap-0.1.3/setup.py` & `sosap-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from setuptools import setup, Extension
-from Cython.Build import cythonize
 import sys
 
 COMPILE_ARGS = ["-std=c++11", "-w"]
 
 if sys.platform.startswith("darwin"):
     COMPILE_ARGS.append("-stdlib=libc++")
     COMPILE_ARGS.append("-mmacosx-version-min=10.7")
@@ -29,8 +28,8 @@
         "src/openfst/include",
         "src/Phonetisaurus",
         "src/Phonetisaurus/3rdparty/utfcpp",
     ],
     extra_compile_args=COMPILE_ARGS,
 )
 
-setup(ext_modules=cythonize(phonetisaurus_extension))
+setup(ext_modules=[phonetisaurus_extension])
```

### Comparing `sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h` & `sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h` & `sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h` & `sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/3rdparty/utfcpp/utf8.h` & `sosap-0.2.0/src/Phonetisaurus/3rdparty/utfcpp/utf8.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/ARPA2WFST.h` & `sosap-0.2.0/src/Phonetisaurus/include/ARPA2WFST.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/LatticePruner.h` & `sosap-0.2.0/src/Phonetisaurus/include/LatticePruner.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMDecodable.h` & `sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMDecodable.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMHash.h` & `sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMHash.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/LegacyRnnLMReader.h` & `sosap-0.2.0/src/Phonetisaurus/include/LegacyRnnLMReader.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/M2MFstAligner.h` & `sosap-0.2.0/src/Phonetisaurus/include/M2MFstAligner.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/PhonetisaurusRex.h` & `sosap-0.2.0/src/Phonetisaurus/include/PhonetisaurusRex.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/PhonetisaurusScript.h` & `sosap-0.2.0/src/Phonetisaurus/include/PhonetisaurusScript.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/RnnLMDecoder.h` & `sosap-0.2.0/src/Phonetisaurus/include/RnnLMDecoder.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/RnnLMPy.h` & `sosap-0.2.0/src/Phonetisaurus/include/RnnLMPy.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/include/util.h` & `sosap-0.2.0/src/Phonetisaurus/include/util.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/lib/LatticePruner.cc` & `sosap-0.2.0/src/Phonetisaurus/lib/LatticePruner.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/lib/M2MFstAligner.cc` & `sosap-0.2.0/src/Phonetisaurus/lib/M2MFstAligner.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/lib/feature-reader.cc` & `sosap-0.2.0/src/Phonetisaurus/lib/feature-reader.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/Phonetisaurus/lib/util.cc` & `sosap-0.2.0/src/Phonetisaurus/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/core.pyx` & `sosap-0.2.0/src/core.pyx`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/accumulator.h` & `sosap-0.2.0/src/openfst/include/fst/accumulator.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/add-on.h` & `sosap-0.2.0/src/openfst/include/fst/add-on.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/arc-arena.h` & `sosap-0.2.0/src/openfst/include/fst/arc-arena.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/arc-map.h` & `sosap-0.2.0/src/openfst/include/fst/arc-map.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/arc.h` & `sosap-0.2.0/src/openfst/include/fst/arc.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/arcfilter.h` & `sosap-0.2.0/src/openfst/include/fst/arcfilter.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/arcsort.h` & `sosap-0.2.0/src/openfst/include/fst/arcsort.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/bi-table.h` & `sosap-0.2.0/src/openfst/include/fst/bi-table.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/cache.h` & `sosap-0.2.0/src/openfst/include/fst/cache.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/closure.h` & `sosap-0.2.0/src/openfst/include/fst/closure.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/compact-fst.h` & `sosap-0.2.0/src/openfst/include/fst/compact-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/compat.h` & `sosap-0.2.0/src/openfst/include/fst/compat.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/complement.h` & `sosap-0.2.0/src/openfst/include/fst/complement.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/compose-filter.h` & `sosap-0.2.0/src/openfst/include/fst/compose-filter.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/compose.h` & `sosap-0.2.0/src/openfst/include/fst/compose.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/concat.h` & `sosap-0.2.0/src/openfst/include/fst/concat.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/connect.h` & `sosap-0.2.0/src/openfst/include/fst/connect.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/const-fst.h` & `sosap-0.2.0/src/openfst/include/fst/const-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/determinize.h` & `sosap-0.2.0/src/openfst/include/fst/determinize.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/dfs-visit.h` & `sosap-0.2.0/src/openfst/include/fst/dfs-visit.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/difference.h` & `sosap-0.2.0/src/openfst/include/fst/difference.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/disambiguate.h` & `sosap-0.2.0/src/openfst/include/fst/disambiguate.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/edit-fst.h` & `sosap-0.2.0/src/openfst/include/fst/edit-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/encode.h` & `sosap-0.2.0/src/openfst/include/fst/encode.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/epsnormalize.h` & `sosap-0.2.0/src/openfst/include/fst/epsnormalize.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/equal.h` & `sosap-0.2.0/src/openfst/include/fst/equal.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/equivalent.h` & `sosap-0.2.0/src/openfst/include/fst/equivalent.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/expanded-fst.h` & `sosap-0.2.0/src/openfst/include/fst/expanded-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/expectation-weight.h` & `sosap-0.2.0/src/openfst/include/fst/expectation-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/factor-weight.h` & `sosap-0.2.0/src/openfst/include/fst/factor-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/filter-state.h` & `sosap-0.2.0/src/openfst/include/fst/filter-state.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/flags.h` & `sosap-0.2.0/src/openfst/include/fst/flags.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/float-weight.h` & `sosap-0.2.0/src/openfst/include/fst/float-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/fst-decl.h` & `sosap-0.2.0/src/openfst/include/fst/fst-decl.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/fst.h` & `sosap-0.2.0/src/openfst/include/fst/fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/fstlib.h` & `sosap-0.2.0/src/openfst/include/fst/fstlib.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/generic-register.h` & `sosap-0.2.0/src/openfst/include/fst/generic-register.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/heap.h` & `sosap-0.2.0/src/openfst/include/fst/heap.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/icu.h` & `sosap-0.2.0/src/openfst/include/fst/icu.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/intersect.h` & `sosap-0.2.0/src/openfst/include/fst/intersect.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/interval-set.h` & `sosap-0.2.0/src/openfst/include/fst/interval-set.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/invert.h` & `sosap-0.2.0/src/openfst/include/fst/invert.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/isomorphic.h` & `sosap-0.2.0/src/openfst/include/fst/isomorphic.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/label-reachable.h` & `sosap-0.2.0/src/openfst/include/fst/label-reachable.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/lexicographic-weight.h` & `sosap-0.2.0/src/openfst/include/fst/lexicographic-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/lock.h` & `sosap-0.2.0/src/openfst/include/fst/lock.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/log.h` & `sosap-0.2.0/src/openfst/include/fst/log.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/lookahead-filter.h` & `sosap-0.2.0/src/openfst/include/fst/lookahead-filter.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/lookahead-matcher.h` & `sosap-0.2.0/src/openfst/include/fst/lookahead-matcher.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/map.h` & `sosap-0.2.0/src/openfst/include/fst/map.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/mapped-file.h` & `sosap-0.2.0/src/openfst/include/fst/mapped-file.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/matcher-fst.h` & `sosap-0.2.0/src/openfst/include/fst/matcher-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/matcher.h` & `sosap-0.2.0/src/openfst/include/fst/matcher.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/memory.h` & `sosap-0.2.0/src/openfst/include/fst/memory.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/minimize.h` & `sosap-0.2.0/src/openfst/include/fst/minimize.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/mutable-fst.h` & `sosap-0.2.0/src/openfst/include/fst/mutable-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/pair-weight.h` & `sosap-0.2.0/src/openfst/include/fst/pair-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/partition.h` & `sosap-0.2.0/src/openfst/include/fst/partition.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/power-weight.h` & `sosap-0.2.0/src/openfst/include/fst/power-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/product-weight.h` & `sosap-0.2.0/src/openfst/include/fst/product-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/project.h` & `sosap-0.2.0/src/openfst/include/fst/project.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/properties.h` & `sosap-0.2.0/src/openfst/include/fst/properties.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/prune.h` & `sosap-0.2.0/src/openfst/include/fst/prune.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/push.h` & `sosap-0.2.0/src/openfst/include/fst/push.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/queue.h` & `sosap-0.2.0/src/openfst/include/fst/queue.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/randequivalent.h` & `sosap-0.2.0/src/openfst/include/fst/randequivalent.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/randgen.h` & `sosap-0.2.0/src/openfst/include/fst/randgen.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/rational.h` & `sosap-0.2.0/src/openfst/include/fst/rational.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/register.h` & `sosap-0.2.0/src/openfst/include/fst/register.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/relabel.h` & `sosap-0.2.0/src/openfst/include/fst/relabel.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/replace-util.h` & `sosap-0.2.0/src/openfst/include/fst/replace-util.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/replace.h` & `sosap-0.2.0/src/openfst/include/fst/replace.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/reverse.h` & `sosap-0.2.0/src/openfst/include/fst/reverse.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/reweight.h` & `sosap-0.2.0/src/openfst/include/fst/reweight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/rmepsilon.h` & `sosap-0.2.0/src/openfst/include/fst/rmepsilon.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/rmfinalepsilon.h` & `sosap-0.2.0/src/openfst/include/fst/rmfinalepsilon.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/set-weight.h` & `sosap-0.2.0/src/openfst/include/fst/set-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/shortest-distance.h` & `sosap-0.2.0/src/openfst/include/fst/shortest-distance.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/shortest-path.h` & `sosap-0.2.0/src/openfst/include/fst/shortest-path.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/signed-log-weight.h` & `sosap-0.2.0/src/openfst/include/fst/signed-log-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/sparse-power-weight.h` & `sosap-0.2.0/src/openfst/include/fst/sparse-power-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/sparse-tuple-weight.h` & `sosap-0.2.0/src/openfst/include/fst/sparse-tuple-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/state-map.h` & `sosap-0.2.0/src/openfst/include/fst/state-map.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/state-reachable.h` & `sosap-0.2.0/src/openfst/include/fst/state-reachable.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/state-table.h` & `sosap-0.2.0/src/openfst/include/fst/state-table.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/statesort.h` & `sosap-0.2.0/src/openfst/include/fst/statesort.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/string-weight.h` & `sosap-0.2.0/src/openfst/include/fst/string-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/string.h` & `sosap-0.2.0/src/openfst/include/fst/string.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/symbol-table-ops.h` & `sosap-0.2.0/src/openfst/include/fst/symbol-table-ops.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/symbol-table.h` & `sosap-0.2.0/src/openfst/include/fst/symbol-table.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/synchronize.h` & `sosap-0.2.0/src/openfst/include/fst/synchronize.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/test-properties.h` & `sosap-0.2.0/src/openfst/include/fst/test-properties.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/topsort.h` & `sosap-0.2.0/src/openfst/include/fst/topsort.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/tuple-weight.h` & `sosap-0.2.0/src/openfst/include/fst/tuple-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/types.h` & `sosap-0.2.0/src/openfst/include/fst/types.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/union-find.h` & `sosap-0.2.0/src/openfst/include/fst/union-find.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/union-weight.h` & `sosap-0.2.0/src/openfst/include/fst/union-weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/union.h` & `sosap-0.2.0/src/openfst/include/fst/union.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/util.h` & `sosap-0.2.0/src/openfst/include/fst/util.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/vector-fst.h` & `sosap-0.2.0/src/openfst/include/fst/vector-fst.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/verify.h` & `sosap-0.2.0/src/openfst/include/fst/verify.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/visit.h` & `sosap-0.2.0/src/openfst/include/fst/visit.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/include/fst/weight.h` & `sosap-0.2.0/src/openfst/include/fst/weight.h`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/compat.cc` & `sosap-0.2.0/src/openfst/lib/compat.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/flags.cc` & `sosap-0.2.0/src/openfst/lib/flags.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/fst-types.cc` & `sosap-0.2.0/src/openfst/lib/fst-types.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/fst.cc` & `sosap-0.2.0/src/openfst/lib/fst.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/mapped-file.cc` & `sosap-0.2.0/src/openfst/lib/mapped-file.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/properties.cc` & `sosap-0.2.0/src/openfst/lib/properties.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/symbol-table-ops.cc` & `sosap-0.2.0/src/openfst/lib/symbol-table-ops.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/symbol-table.cc` & `sosap-0.2.0/src/openfst/lib/symbol-table.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/util.cc` & `sosap-0.2.0/src/openfst/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/openfst/lib/weight.cc` & `sosap-0.2.0/src/openfst/lib/weight.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.3/src/sosap.egg-info/PKG-INFO` & `sosap-0.2.0/src/sosap.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sosap-0.1.3/src/sosap.egg-info/SOURCES.txt` & `sosap-0.2.0/src/sosap.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-src/.DS_Store
-src/core.cpp
 src/core.pyx
-src/phonemizer.cc
 src/Phonetisaurus/3rdparty/utfcpp/utf8.h
 src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h
 src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h
 src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h
 src/Phonetisaurus/include/ARPA2WFST.h
 src/Phonetisaurus/include/LatticePruner.h
 src/Phonetisaurus/include/LegacyRnnLMDecodable.h
```

