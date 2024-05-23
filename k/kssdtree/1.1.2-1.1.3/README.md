# Comparing `tmp/kssdtree-1.1.2.tar.gz` & `tmp/kssdtree-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kssdtree-1.1.2.tar", last modified: Wed May 22 06:01:30 2024, max compression
+gzip compressed data, was "kssdtree-1.1.3.tar", last modified: Wed May 22 08:08:07 2024, max compression
```

## Comparing `kssdtree-1.1.2.tar` & `kssdtree-1.1.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.415833 kssdtree-1.1.2/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       99 2024-03-15 09:41:31.000000 kssdtree-1.1.2/MANIFEST.in
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 06:01:30.415833 kssdtree-1.1.2/PKG-INFO
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5769 2024-03-15 09:41:32.000000 kssdtree-1.1.2/README.md
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11874 2024-03-15 09:41:31.000000 kssdtree-1.1.2/align.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24008 2024-03-15 09:41:31.000000 kssdtree-1.1.2/buildtree.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:31.000000 kssdtree-1.1.2/bytescale.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11214 2024-03-15 09:41:31.000000 kssdtree-1.1.2/cluster.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14308 2024-03-15 09:41:31.000000 kssdtree-1.1.2/co2mco.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     8670 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_composite.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    85597 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_dist.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1491 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_dist_wrapper.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30339 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_set.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5456 2024-03-15 09:41:31.000000 kssdtree-1.1.2/command_shuffle.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16270 2024-03-15 09:41:31.000000 kssdtree-1.1.2/distancemat.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    31139 2024-03-15 09:41:31.000000 kssdtree-1.1.2/dnj.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/dnjheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      848 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/bytescale.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2455 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/dnj.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1823 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/filebuff.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2376 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/hclust.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1476 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/matrix.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/mman.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2894 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/nj.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1349 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/nwck.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1769 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/pherror.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1442 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/phy.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1097 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/qseqs.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      863 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/str.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1630 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/threader.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      787 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/tmp.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      997 2024-03-15 09:41:33.000000 kssdtree-1.1.2/dnjheaders/vector.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7897 2024-03-15 09:41:31.000000 kssdtree-1.1.2/filebuff.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17969 2024-03-15 09:41:31.000000 kssdtree-1.1.2/global_basic.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    34136 2024-03-15 09:41:31.000000 kssdtree-1.1.2/hclust.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24287 2024-03-15 09:41:31.000000 kssdtree-1.1.2/iseq2comem.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/kssdheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1915 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/co2mco.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      965 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_composite.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3905 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_dist.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1455 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_dist_wrapper.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      931 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_set.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1337 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/command_shuffle.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7850 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/global_basic.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1482 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/iseq2comem.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/mman.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:33.000000 kssdtree-1.1.2/kssdheaders/mytime.h
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.411833 kssdtree-1.1.2/kssdtree.egg-info/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/PKG-INFO
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1274 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/SOURCES.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       32 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/dependency_links.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)        1 2024-03-15 09:42:02.000000 kssdtree-1.1.2/kssdtree.egg-info/not-zip-safe
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       20 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/requires.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       31 2024-05-22 06:01:30.000000 kssdtree-1.1.2/kssdtree.egg-info/top_level.txt
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17560 2024-05-22 04:25:44.000000 kssdtree-1.1.2/kssdtree.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16438 2024-03-15 09:41:31.000000 kssdtree-1.1.2/matrix.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3564 2024-03-15 09:41:31.000000 kssdtree-1.1.2/mman.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1362 2024-03-15 09:41:31.000000 kssdtree-1.1.2/mytime.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    35423 2024-03-15 09:41:31.000000 kssdtree-1.1.2/nj.c
-drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 06:01:30.415833 kssdtree-1.1.2/njheaders/
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3691 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/align.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4993 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/buildtree.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     6506 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/cluster.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7468 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/distancemat.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2584 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/sequence.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14344 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/tree.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3782 2024-03-15 09:41:34.000000 kssdtree-1.1.2/njheaders/util.h
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7969 2024-03-15 09:41:31.000000 kssdtree-1.1.2/nwck.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1925 2024-03-15 09:41:31.000000 kssdtree-1.1.2/pherror.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14122 2024-03-15 09:41:32.000000 kssdtree-1.1.2/phy.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5398 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pydnj.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    20098 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pykssd.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1713 2024-03-15 09:41:32.000000 kssdtree-1.1.2/pynj.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1935 2024-03-15 09:41:32.000000 kssdtree-1.1.2/qseqs.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4428 2024-03-15 09:41:32.000000 kssdtree-1.1.2/sequence.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       38 2024-05-22 06:01:30.415833 kssdtree-1.1.2/setup.cfg
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3581 2024-05-22 06:01:27.000000 kssdtree-1.1.2/setup.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1313 2024-03-15 09:41:32.000000 kssdtree-1.1.2/str.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2193 2024-03-15 09:41:32.000000 kssdtree-1.1.2/tmp.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    12433 2024-05-22 04:11:36.000000 kssdtree-1.1.2/toolutils.py
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30399 2024-03-15 09:41:32.000000 kssdtree-1.1.2/tree.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4616 2024-03-15 09:41:32.000000 kssdtree-1.1.2/util.c
--rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1267 2024-03-15 09:41:32.000000 kssdtree-1.1.2/vector.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 08:08:07.720219 kssdtree-1.1.3/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       99 2024-03-15 09:41:31.000000 kssdtree-1.1.3/MANIFEST.in
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 08:08:07.720219 kssdtree-1.1.3/PKG-INFO
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5769 2024-03-15 09:41:32.000000 kssdtree-1.1.3/README.md
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11874 2024-03-15 09:41:31.000000 kssdtree-1.1.3/align.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24008 2024-03-15 09:41:31.000000 kssdtree-1.1.3/buildtree.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:31.000000 kssdtree-1.1.3/bytescale.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    11214 2024-03-15 09:41:31.000000 kssdtree-1.1.3/cluster.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14308 2024-03-15 09:41:31.000000 kssdtree-1.1.3/co2mco.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     8670 2024-03-15 09:41:31.000000 kssdtree-1.1.3/command_composite.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    85597 2024-03-15 09:41:31.000000 kssdtree-1.1.3/command_dist.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1491 2024-03-15 09:41:31.000000 kssdtree-1.1.3/command_dist_wrapper.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30339 2024-03-15 09:41:31.000000 kssdtree-1.1.3/command_set.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5456 2024-03-15 09:41:31.000000 kssdtree-1.1.3/command_shuffle.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16270 2024-03-15 09:41:31.000000 kssdtree-1.1.3/distancemat.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    31139 2024-03-15 09:41:31.000000 kssdtree-1.1.3/dnj.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 08:08:07.720219 kssdtree-1.1.3/dnjheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      848 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/bytescale.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2455 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/dnj.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1823 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/filebuff.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2376 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/hclust.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1476 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/matrix.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/mman.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2894 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/nj.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1349 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/nwck.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1769 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/pherror.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1442 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/phy.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1097 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/qseqs.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      863 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/str.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1630 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/threader.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      787 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/tmp.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      997 2024-03-15 09:41:33.000000 kssdtree-1.1.3/dnjheaders/vector.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7897 2024-03-15 09:41:31.000000 kssdtree-1.1.3/filebuff.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17969 2024-03-15 09:41:31.000000 kssdtree-1.1.3/global_basic.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    34136 2024-03-15 09:41:31.000000 kssdtree-1.1.3/hclust.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    24287 2024-03-15 09:41:31.000000 kssdtree-1.1.3/iseq2comem.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 08:08:07.720219 kssdtree-1.1.3/kssdheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1915 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/co2mco.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      965 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/command_composite.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3905 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/command_dist.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1455 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/command_dist_wrapper.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      931 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/command_set.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1337 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/command_shuffle.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7850 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/global_basic.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1482 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/iseq2comem.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1809 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/mman.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      791 2024-03-15 09:41:33.000000 kssdtree-1.1.3/kssdheaders/mytime.h
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 08:08:07.720219 kssdtree-1.1.3/kssdtree.egg-info/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)      477 2024-05-22 08:08:07.000000 kssdtree-1.1.3/kssdtree.egg-info/PKG-INFO
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1274 2024-05-22 08:08:07.000000 kssdtree-1.1.3/kssdtree.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       32 2024-05-22 08:08:07.000000 kssdtree-1.1.3/kssdtree.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)        1 2024-03-15 09:42:02.000000 kssdtree-1.1.3/kssdtree.egg-info/not-zip-safe
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       20 2024-05-22 08:08:07.000000 kssdtree-1.1.3/kssdtree.egg-info/requires.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       31 2024-05-22 08:08:07.000000 kssdtree-1.1.3/kssdtree.egg-info/top_level.txt
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    17560 2024-05-22 04:25:44.000000 kssdtree-1.1.3/kssdtree.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    16438 2024-03-15 09:41:31.000000 kssdtree-1.1.3/matrix.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3564 2024-03-15 09:41:31.000000 kssdtree-1.1.3/mman.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1362 2024-03-15 09:41:31.000000 kssdtree-1.1.3/mytime.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    35423 2024-03-15 09:41:31.000000 kssdtree-1.1.3/nj.c
+drwxrwxr-x   0 yanghang  (1003) yanghang  (1003)        0 2024-05-22 08:08:07.720219 kssdtree-1.1.3/njheaders/
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3691 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/align.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4993 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/buildtree.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     6506 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/cluster.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7468 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/distancemat.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2584 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/sequence.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14344 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/tree.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3782 2024-03-15 09:41:34.000000 kssdtree-1.1.3/njheaders/util.h
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     7969 2024-03-15 09:41:31.000000 kssdtree-1.1.3/nwck.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1925 2024-03-15 09:41:31.000000 kssdtree-1.1.3/pherror.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    14122 2024-03-15 09:41:32.000000 kssdtree-1.1.3/phy.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     5398 2024-03-15 09:41:32.000000 kssdtree-1.1.3/pydnj.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    20098 2024-03-15 09:41:32.000000 kssdtree-1.1.3/pykssd.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1713 2024-03-15 09:41:32.000000 kssdtree-1.1.3/pynj.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1935 2024-03-15 09:41:32.000000 kssdtree-1.1.3/qseqs.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4428 2024-03-15 09:41:32.000000 kssdtree-1.1.3/sequence.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)       38 2024-05-22 08:08:07.720219 kssdtree-1.1.3/setup.cfg
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     3581 2024-05-22 08:08:05.000000 kssdtree-1.1.3/setup.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1313 2024-03-15 09:41:32.000000 kssdtree-1.1.3/str.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     2193 2024-03-15 09:41:32.000000 kssdtree-1.1.3/tmp.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    12433 2024-05-22 04:11:36.000000 kssdtree-1.1.3/toolutils.py
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)    30399 2024-03-15 09:41:32.000000 kssdtree-1.1.3/tree.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     4616 2024-03-15 09:41:32.000000 kssdtree-1.1.3/util.c
+-rw-rw-r--   0 yanghang  (1003) yanghang  (1003)     1267 2024-03-15 09:41:32.000000 kssdtree-1.1.3/vector.c
```

### Comparing `kssdtree-1.1.2/README.md` & `kssdtree-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/align.c` & `kssdtree-1.1.3/align.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/buildtree.c` & `kssdtree-1.1.3/buildtree.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/bytescale.c` & `kssdtree-1.1.3/bytescale.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/cluster.c` & `kssdtree-1.1.3/cluster.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/co2mco.c` & `kssdtree-1.1.3/co2mco.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/command_composite.c` & `kssdtree-1.1.3/command_composite.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/command_dist.c` & `kssdtree-1.1.3/command_dist.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/command_dist_wrapper.c` & `kssdtree-1.1.3/command_dist_wrapper.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/command_set.c` & `kssdtree-1.1.3/command_set.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/command_shuffle.c` & `kssdtree-1.1.3/command_shuffle.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/distancemat.c` & `kssdtree-1.1.3/distancemat.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnj.c` & `kssdtree-1.1.3/dnj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/bytescale.h` & `kssdtree-1.1.3/dnjheaders/bytescale.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/dnj.h` & `kssdtree-1.1.3/dnjheaders/dnj.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/filebuff.h` & `kssdtree-1.1.3/dnjheaders/filebuff.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/hclust.h` & `kssdtree-1.1.3/dnjheaders/hclust.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/matrix.h` & `kssdtree-1.1.3/dnjheaders/matrix.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/mman.h` & `kssdtree-1.1.3/dnjheaders/mman.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/nj.h` & `kssdtree-1.1.3/dnjheaders/nj.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/nwck.h` & `kssdtree-1.1.3/dnjheaders/nwck.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/pherror.h` & `kssdtree-1.1.3/dnjheaders/pherror.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/phy.h` & `kssdtree-1.1.3/dnjheaders/phy.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/qseqs.h` & `kssdtree-1.1.3/dnjheaders/qseqs.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/str.h` & `kssdtree-1.1.3/dnjheaders/str.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/threader.h` & `kssdtree-1.1.3/dnjheaders/threader.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/tmp.h` & `kssdtree-1.1.3/dnjheaders/tmp.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/dnjheaders/vector.h` & `kssdtree-1.1.3/dnjheaders/vector.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/filebuff.c` & `kssdtree-1.1.3/filebuff.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/global_basic.c` & `kssdtree-1.1.3/global_basic.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/hclust.c` & `kssdtree-1.1.3/hclust.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/iseq2comem.c` & `kssdtree-1.1.3/iseq2comem.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/co2mco.h` & `kssdtree-1.1.3/kssdheaders/co2mco.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/command_composite.h` & `kssdtree-1.1.3/kssdheaders/command_composite.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/command_dist.h` & `kssdtree-1.1.3/kssdheaders/command_dist.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/command_dist_wrapper.h` & `kssdtree-1.1.3/kssdheaders/command_dist_wrapper.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/command_set.h` & `kssdtree-1.1.3/kssdheaders/command_set.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/command_shuffle.h` & `kssdtree-1.1.3/kssdheaders/command_shuffle.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/global_basic.h` & `kssdtree-1.1.3/kssdheaders/global_basic.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/iseq2comem.h` & `kssdtree-1.1.3/kssdheaders/iseq2comem.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/mman.h` & `kssdtree-1.1.3/kssdheaders/mman.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdheaders/mytime.h` & `kssdtree-1.1.3/kssdheaders/mytime.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdtree.egg-info/SOURCES.txt` & `kssdtree-1.1.3/kssdtree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/kssdtree.py` & `kssdtree-1.1.3/kssdtree.py`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/matrix.c` & `kssdtree-1.1.3/matrix.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/mman.c` & `kssdtree-1.1.3/mman.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/mytime.c` & `kssdtree-1.1.3/mytime.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/nj.c` & `kssdtree-1.1.3/nj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/align.h` & `kssdtree-1.1.3/njheaders/align.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/buildtree.h` & `kssdtree-1.1.3/njheaders/buildtree.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/cluster.h` & `kssdtree-1.1.3/njheaders/cluster.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/distancemat.h` & `kssdtree-1.1.3/njheaders/distancemat.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/sequence.h` & `kssdtree-1.1.3/njheaders/sequence.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/tree.h` & `kssdtree-1.1.3/njheaders/tree.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/njheaders/util.h` & `kssdtree-1.1.3/njheaders/util.h`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/nwck.c` & `kssdtree-1.1.3/nwck.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/pherror.c` & `kssdtree-1.1.3/pherror.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/phy.c` & `kssdtree-1.1.3/phy.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/pydnj.c` & `kssdtree-1.1.3/pydnj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/pykssd.c` & `kssdtree-1.1.3/pykssd.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/pynj.c` & `kssdtree-1.1.3/pynj.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/qseqs.c` & `kssdtree-1.1.3/qseqs.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/sequence.c` & `kssdtree-1.1.3/sequence.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/setup.py` & `kssdtree-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     'pyqt5',
     'ete3',
     'requests'
 ]
 
 setup(
     name='kssdtree',
-    version='1.1.2',
+    version='1.1.3',
     author='Hang Yang',
     author_email='yhlink1207@gmail.com',
     description="Kssdtree is a versatile Python package for phylogenetic analysis. It also provides one-stop tree construction and visualization. It can handle DNA sequences of both fasta or fastq format, whether gzipped or not. ",
     url='https://github.com/yhlink/kssdtree',
     download_url='https://pypi.org/project/kssdtree',
     ext_modules=[
         Extension(MOD1, sources=sources1, include_dirs=include_dirs1, libraries=['z'],
```

### Comparing `kssdtree-1.1.2/str.c` & `kssdtree-1.1.3/str.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/tmp.c` & `kssdtree-1.1.3/tmp.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/toolutils.py` & `kssdtree-1.1.3/toolutils.py`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/tree.c` & `kssdtree-1.1.3/tree.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/util.c` & `kssdtree-1.1.3/util.c`

 * *Files identical despite different names*

### Comparing `kssdtree-1.1.2/vector.c` & `kssdtree-1.1.3/vector.c`

 * *Files identical despite different names*

