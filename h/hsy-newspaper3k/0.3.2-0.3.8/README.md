# Comparing `tmp/hsy_newspaper3k-0.3.2.tar.gz` & `tmp/hsy-newspaper3k-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsy_newspaper3k-0.3.2.tar", last modified: Mon Mar  4 07:58:03 2024, max compression
+gzip compressed data, was "hsy-newspaper3k-0.3.8.tar", last modified: Thu May 23 04:11:54 2024, max compression
```

## Comparing `hsy_newspaper3k-0.3.2.tar` & `hsy-newspaper3k-0.3.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.983116 hsy_newspaper3k-0.3.2/
--rw-rw-rw-   0        0        0     1080 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      135 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11815 2024-03-04 07:58:03.982110 hsy_newspaper3k-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    11003 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.889596 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/
--rw-rw-rw-   0        0        0    11815 2024-03-04 07:58:03.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2024-03-04 07:58:03.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 07:58:03.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-28 02:08:13.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      237 2024-03-04 07:58:03.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-04 07:58:03.000000 hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.917598 hsy_newspaper3k-0.3.2/newspaper/
--rw-rw-rw-   0        0        0      811 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/__init__.py
--rw-rw-rw-   0        0        0     2631 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/api.py
--rw-rw-rw-   0        0        0    19563 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/article.py
--rw-rw-rw-   0        0        0    10419 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/cleaners.py
--rw-rw-rw-   0        0        0     4401 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/configuration.py
--rw-rw-rw-   0        0        0    42043 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/extractors.py
--rw-rw-rw-   0        0        0     7575 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/images.py
--rw-rw-rw-   0        0        0     4074 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/mthreading.py
--rw-rw-rw-   0        0        0     4291 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/network.py
--rw-rw-rw-   0        0        0     5911 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/nlp.py
--rw-rw-rw-   0        0        0     6092 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/outputformatters.py
--rw-rw-rw-   0        0        0     7803 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/parsers.py
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.877587 hsy_newspaper3k-0.3.2/newspaper/resources/
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.924596 hsy_newspaper3k-0.3.2/newspaper/resources/misc/
--rw-rw-rw-   0        0        0   349280 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/misc/google_sources.txt
--rw-rw-rw-   0        0        0     4264 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/misc/popular_sources.txt
--rw-rw-rw-   0        0        0     2389 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/misc/stopwords-nlp-en.txt
--rw-rw-rw-   0        0        0     4241 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/misc/useragents.txt
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.977118 hsy_newspaper3k-0.3.2/newspaper/resources/text/
--rw-rw-rw-   0        0        0     1450 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ar.txt
--rw-rw-rw-   0        0        0      936 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-be.txt
--rw-rw-rw-   0        0        0     2409 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-bg.txt
--rw-rw-rw-   0        0        0      484 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-da.txt
--rw-rw-rw-   0        0        0     5967 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-de.txt
--rw-rw-rw-   0        0        0    13903 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-el.txt
--rw-rw-rw-   0        0        0     3585 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-en.txt
--rw-rw-rw-   0        0        0     2185 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-es.txt
--rw-rw-rw-   0        0        0      189 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-et.txt
--rw-rw-rw-   0        0        0     7710 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-fa.txt
--rw-rw-rw-   0        0        0      464 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-fi.txt
--rw-rw-rw-   0        0        0     2002 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-fr.txt
--rw-rw-rw-   0        0        0     1836 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-he.txt
--rw-rw-rw-   0        0        0     2790 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hi.txt
--rw-rw-rw-   0        0        0      870 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hr.txt
--rw-rw-rw-   0        0        0     2337 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hu.txt
--rw-rw-rw-   0        0        0    10499 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-id.txt
--rw-rw-rw-   0        0        0     1696 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-it.txt
--rw-rw-rw-   0        0        0     1006 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ja.txt
--rw-rw-rw-   0        0        0      459 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ko.txt
--rw-rw-rw-   0        0        0      763 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-lt.txt
--rw-rw-rw-   0        0        0     1504 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-mk.txt
--rw-rw-rw-   0        0        0      587 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-nb.txt
--rw-rw-rw-   0        0        0      177 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-nl.txt
--rw-rw-rw-   0        0        0      513 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-no.txt
--rw-rw-rw-   0        0        0     2015 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-pl.txt
--rw-rw-rw-   0        0        0     3610 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-pt.txt
--rw-rw-rw-   0        0        0     1915 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ro.txt
--rw-rw-rw-   0        0        0     4958 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ru.txt
--rw-rw-rw-   0        0        0     2435 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sl.txt
--rw-rw-rw-   0        0        0      776 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sr.txt
--rw-rw-rw-   0        0        0     3956 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sv.txt
--rw-rw-rw-   0        0        0      407 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sw.txt
--rw-rw-rw-   0        0        0     1420 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-th.txt
--rw-rw-rw-   0        0        0     1368 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-tr.txt
--rw-rw-rw-   0        0        0     4029 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-uk.txt
--rw-rw-rw-   0        0        0      724 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-vi.txt
--rw-rw-rw-   0        0        0      623 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-zh.txt
--rw-rw-rw-   0        0        0     1649 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/settings.py
--rw-rw-rw-   0        0        0    15336 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/source.py
--rw-rw-rw-   0        0        0     6046 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/text.py
--rw-rw-rw-   0        0        0    10222 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/urls.py
--rw-rw-rw-   0        0        0    12195 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/utils.py
--rw-rw-rw-   0        0        0      296 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/newspaper/version.py
-drwxrwxrwx   0        0        0        0 2024-03-04 07:58:03.981105 hsy_newspaper3k-0.3.2/newspaper/videos/
--rw-rw-rw-   0        0        0        0 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/videos/__init__.py
--rw-rw-rw-   0        0        0     3793 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/videos/extractors.py
--rw-rw-rw-   0        0        0      421 2024-02-28 01:52:20.000000 hsy_newspaper3k-0.3.2/newspaper/videos/videos.py
--rw-rw-rw-   0        0        0      286 2024-02-28 01:52:19.000000 hsy_newspaper3k-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-04 07:58:03.983116 hsy_newspaper3k-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1665 2024-03-04 07:57:14.000000 hsy_newspaper3k-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.701616 hsy-newspaper3k-0.3.8/
+-rw-rw-rw-   0        0        0     1080 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      135 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    12101 2024-05-23 04:11:54.699622 hsy-newspaper3k-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11073 2024-03-27 09:03:00.000000 hsy-newspaper3k-0.3.8/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.468107 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/
+-rw-rw-rw-   0        0        0    12101 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      237 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 04:11:54.000000 hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.532478 hsy-newspaper3k-0.3.8/newspaper/
+-rw-rw-rw-   0        0        0      811 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/__init__.py
+-rw-rw-rw-   0        0        0     2631 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/api.py
+-rw-rw-rw-   0        0        0    19563 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/article.py
+-rw-rw-rw-   0        0        0    10419 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/cleaners.py
+-rw-rw-rw-   0        0        0     4401 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/configuration.py
+-rw-rw-rw-   0        0        0    42043 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/extractors.py
+-rw-rw-rw-   0        0        0     7575 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/images.py
+-rw-rw-rw-   0        0        0     4074 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/mthreading.py
+-rw-rw-rw-   0        0        0     4291 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/network.py
+-rw-rw-rw-   0        0        0     5911 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/nlp.py
+-rw-rw-rw-   0        0        0     6092 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/outputformatters.py
+-rw-rw-rw-   0        0        0     7803 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/parsers.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.436946 hsy-newspaper3k-0.3.8/newspaper/resources/
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.551832 hsy-newspaper3k-0.3.8/newspaper/resources/misc/
+-rw-rw-rw-   0        0        0   349280 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/misc/google_sources.txt
+-rw-rw-rw-   0        0        0     4264 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/misc/popular_sources.txt
+-rw-rw-rw-   0        0        0     2389 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/misc/stopwords-nlp-en.txt
+-rw-rw-rw-   0        0        0     4241 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/misc/useragents.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.687926 hsy-newspaper3k-0.3.8/newspaper/resources/text/
+-rw-rw-rw-   0        0        0     1450 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ar.txt
+-rw-rw-rw-   0        0        0      936 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-be.txt
+-rw-rw-rw-   0        0        0     2409 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-bg.txt
+-rw-rw-rw-   0        0        0      484 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-da.txt
+-rw-rw-rw-   0        0        0     5967 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-de.txt
+-rw-rw-rw-   0        0        0    13903 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-el.txt
+-rw-rw-rw-   0        0        0     3585 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-en.txt
+-rw-rw-rw-   0        0        0     2185 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-es.txt
+-rw-rw-rw-   0        0        0      189 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-et.txt
+-rw-rw-rw-   0        0        0     7710 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-fa.txt
+-rw-rw-rw-   0        0        0      464 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-fi.txt
+-rw-rw-rw-   0        0        0     2002 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-fr.txt
+-rw-rw-rw-   0        0        0     1836 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-he.txt
+-rw-rw-rw-   0        0        0     2790 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hi.txt
+-rw-rw-rw-   0        0        0      870 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hr.txt
+-rw-rw-rw-   0        0        0     2337 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hu.txt
+-rw-rw-rw-   0        0        0    10499 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-id.txt
+-rw-rw-rw-   0        0        0     1696 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-it.txt
+-rw-rw-rw-   0        0        0     1006 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ja.txt
+-rw-rw-rw-   0        0        0      459 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ko.txt
+-rw-rw-rw-   0        0        0      763 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-lt.txt
+-rw-rw-rw-   0        0        0     1504 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-mk.txt
+-rw-rw-rw-   0        0        0      587 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-nb.txt
+-rw-rw-rw-   0        0        0      177 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-nl.txt
+-rw-rw-rw-   0        0        0      513 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-no.txt
+-rw-rw-rw-   0        0        0     2015 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-pl.txt
+-rw-rw-rw-   0        0        0     3610 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-pt.txt
+-rw-rw-rw-   0        0        0     1915 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ro.txt
+-rw-rw-rw-   0        0        0     4958 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ru.txt
+-rw-rw-rw-   0        0        0     2435 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sl.txt
+-rw-rw-rw-   0        0        0      776 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sr.txt
+-rw-rw-rw-   0        0        0     3956 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sv.txt
+-rw-rw-rw-   0        0        0      407 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sw.txt
+-rw-rw-rw-   0        0        0     1420 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-th.txt
+-rw-rw-rw-   0        0        0     1368 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-tr.txt
+-rw-rw-rw-   0        0        0     4029 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-uk.txt
+-rw-rw-rw-   0        0        0      724 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-vi.txt
+-rw-rw-rw-   0        0        0      623 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-zh.txt
+-rw-rw-rw-   0        0        0     1649 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/settings.py
+-rw-rw-rw-   0        0        0    15336 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/source.py
+-rw-rw-rw-   0        0        0     6046 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/text.py
+-rw-rw-rw-   0        0        0    10222 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/urls.py
+-rw-rw-rw-   0        0        0    12195 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/utils.py
+-rw-rw-rw-   0        0        0      296 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/newspaper/version.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:11:54.696418 hsy-newspaper3k-0.3.8/newspaper/videos/
+-rw-rw-rw-   0        0        0        0 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/videos/__init__.py
+-rw-rw-rw-   0        0        0     3793 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/videos/extractors.py
+-rw-rw-rw-   0        0        0      421 2024-02-28 01:52:20.000000 hsy-newspaper3k-0.3.8/newspaper/videos/videos.py
+-rw-rw-rw-   0        0        0      286 2024-02-28 01:52:19.000000 hsy-newspaper3k-0.3.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:11:54.701616 hsy-newspaper3k-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1904 2024-05-23 04:11:08.000000 hsy-newspaper3k-0.3.8/setup.py
```

### Comparing `hsy_newspaper3k-0.3.2/LICENSE` & `hsy-newspaper3k-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/PKG-INFO` & `hsy-newspaper3k-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
-Name: hsy_newspaper3k
-Version: 0.3.2
+Name: hsy-newspaper3k
+Version: 0.3.8
 Summary: Simplified python article discovery & extraction.
 Home-page: https://github.com/huangsiyuan924/newspaper/
-Author: Lucas Ou-Yang
-Author-email: lucasyangpersonal@gmail.com
+Author: Siyuan Huang
+Author-email: huangsiyuan924@gmail.com
 License: MIT
+Project-URL: Source, https://github.com/huangsiyuan924/newspaper/
+Project-URL: Documentation, https://github.com/huangsiyuan924/newspaper/
+Project-URL: Bug Tracker, https://github.com/huangsiyuan924/newspaper//issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 License-File: LICENSE
 
 Newspaper3k: Article scraping & curation
 ========================================
 
 .. image:: https://badge.fury.io/py/newspaper3k.svg
     :target: http://badge.fury.io/py/newspaper3k.svg
         :alt: Latest version
 
-.. image:: https://travis-ci.org/codelucas/newspaper.svg
-        :target: http://travis-ci.org/codelucas/newspaper/
+.. image:: https://travis-ci.org/huangsiyuan924/newspaper.svg
+        :target: http://travis-ci.org/huangsiyuan924/newspaper/
         :alt: Build status
 
-.. image:: https://coveralls.io/repos/github/codelucas/newspaper/badge.svg?branch=master
-        :target: https://coveralls.io/github/codelucas/newspaper
+.. image:: https://coveralls.io/repos/github/huangsiyuan924/newspaper/badge.svg?branch=master
+        :target: https://coveralls.io/github/huangsiyuan924/newspaper
         :alt: Coverage status
 
 
 Inspired by `requests`_ for its simplicity and powered by `lxml`_ for its speed:
 
     "Newspaper is an amazing python library for extracting & curating articles."
     -- `tweeted by`_ Kenneth Reitz, Author of `requests`_
@@ -36,15 +39,15 @@
     "Newspaper delivers Instapaper style article extraction." -- `The Changelog`_
 
 .. _`tweeted by`: https://twitter.com/kennethreitz/status/419520678862548992
 .. _`The Changelog`: http://thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
 
 **Newspaper is a Python3 library**! Or, view our **deprecated and buggy** `Python2 branch`_
 
-.. _`Python2 branch`: https://github.com/codelucas/newspaper/tree/python-2-head
+.. _`Python2 branch`: https://github.com/huangsiyuan924/newspaper/tree/python-2-head
 
 A Glance:
 ---------
 
 .. code-block:: pycon
 
     >>> from newspaper import Article
@@ -279,15 +282,15 @@
 
     $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev
 
 NOTE: If you find problem installing ``libpng12-dev``, try installing ``libpng-dev``.
 
 - Download NLP related corpora::
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 - Install the distribution via pip::
 
     $ pip3 install newspaper3k
 
 **If you are on OSX**, install using the following, you may use both homebrew or macports:
 
@@ -295,47 +298,47 @@
 
     $ brew install libxml2 libxslt
 
     $ brew install libtiff libjpeg webp little-cms2
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 
 **Otherwise**, install with the following:
 
 NOTE: You will still most likely need to install the following libraries via your package manager
 
 - PIL: ``libjpeg-dev`` ``zlib1g-dev`` ``libpng12-dev``
 - lxml: ``libxml2-dev`` ``libxslt-dev``
 - Python Development version: ``python-dev``
 
 ::
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 Donations
 ---------
 
 Your donations are greatly appreciated! They will free me up to work on this project more,
 to take on things like: adding new features, bug-fix support, addressing concerns with the library.
 
-- My PayPal link: `https://www.paypal.me/codelucas`_
+- My PayPal link: `https://www.paypal.me/huangsiyuan924`_
 - My `Venmo`_ handle: @Lucas-Ou-Yang
 
 Development
 -----------
 
 If you'd like to contribute and hack on the newspaper project, feel free to clone
 a development version of this repository locally::
 
-    git clone git://github.com/codelucas/newspaper.git
+    git clone git://github.com/huangsiyuan924/newspaper.git
 
 Once you have a copy of the source, you can embed it in your Python package,
 or install it into your site-packages easily::
 
     $ pip3 install -r requirements.txt
     $ python3 setup.py install
 
@@ -364,20 +367,20 @@
 automatic extraction.
 
 Newspaper uses a lot of `python-goose's`_ parsing code. View their license `here`_.
 
 Please feel free to `email & contact me`_ if you run into issues or just would like
 to talk about the future of this library and news extraction in general!
 
-.. _`Lucas Ou-Yang`: http://codelucas.com
+.. _`Lucas Ou-Yang`: http://huangsiyuan924.com
 .. _`email & contact me`: mailto:lucasyangpersonal@gmail.com
 .. _`python-goose's`: https://github.com/grangier/python-goose
-.. _`here`: https://github.com/codelucas/newspaper/blob/master/GOOSE-LICENSE.txt
+.. _`here`: https://github.com/huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt
 
-.. _`https://www.paypal.me/codelucas`: https://www.paypal.me/codelucas
+.. _`https://www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924
 .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang
 
 .. _`Quickstart guide`: https://newspaper.readthedocs.io/en/latest/
 .. _`The Docs`: https://newspaper.readthedocs.io
 .. _`lxml`: http://lxml.de/
 .. _`requests`: https://github.com/kennethreitz/requests
 .. _`Parse.ly`: http://parse.ly
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1 Name: hsy_newspaper3k Version: 0.3.2 Summary: Simplified
+Metadata-Version: 2.1 Name: hsy-newspaper3k Version: 0.3.8 Summary: Simplified
 python article discovery & extraction. Home-page: https://github.com/
-huangsiyuan924/newspaper/ Author: Lucas Ou-Yang Author-email:
-lucasyangpersonal@gmail.com License: MIT Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers License-File: LICENSE Newspaper3k:
-Article scraping & curation ======================================== .. image::
-https://badge.fury.io/py/newspaper3k.svg :target: http://badge.fury.io/py/
+huangsiyuan924/newspaper/ Author: Siyuan Huang Author-email:
+huangsiyuan924@gmail.com License: MIT Project-URL: Source, https://github.com/
+huangsiyuan924/newspaper/ Project-URL: Documentation, https://github.com/
+huangsiyuan924/newspaper/ Project-URL: Bug Tracker, https://github.com/
+huangsiyuan924/newspaper//issues Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3 Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers License-File: LICENSE Newspaper3k: Article
+scraping & curation ======================================== .. image:: https:/
+/badge.fury.io/py/newspaper3k.svg :target: http://badge.fury.io/py/
 newspaper3k.svg :alt: Latest version .. image:: https://travis-ci.org/
-codelucas/newspaper.svg :target: http://travis-ci.org/codelucas/newspaper/ :
-alt: Build status .. image:: https://coveralls.io/repos/github/codelucas/
-newspaper/badge.svg?branch=master :target: https://coveralls.io/github/
-codelucas/newspaper :alt: Coverage status Inspired by `requests`_ for its
-simplicity and powered by `lxml`_ for its speed: "Newspaper is an amazing
-python library for extracting & curating articles." -- `tweeted by`_ Kenneth
-Reitz, Author of `requests`_ "Newspaper delivers Instapaper style article
-extraction." -- `The Changelog`_ .. _`tweeted by`: https://twitter.com/
+huangsiyuan924/newspaper.svg :target: http://travis-ci.org/huangsiyuan924/
+newspaper/ :alt: Build status .. image:: https://coveralls.io/repos/github/
+huangsiyuan924/newspaper/badge.svg?branch=master :target: https://coveralls.io/
+github/huangsiyuan924/newspaper :alt: Coverage status Inspired by `requests`_
+for its simplicity and powered by `lxml`_ for its speed: "Newspaper is an
+amazing python library for extracting & curating articles." -- `tweeted by`_
+Kenneth Reitz, Author of `requests`_ "Newspaper delivers Instapaper style
+article extraction." -- `The Changelog`_ .. _`tweeted by`: https://twitter.com/
 kennethreitz/status/419520678862548992 .. _`The Changelog`: http://
 thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
 **Newspaper is a Python3 library**! Or, view our **deprecated and buggy**
-`Python2 branch`_ .. _`Python2 branch`: https://github.com/codelucas/newspaper/
-tree/python-2-head A Glance: --------- .. code-block:: pycon >>> from newspaper
-import Article >>> url = 'http://fox13now.com/2013/12/30/new-year-new-laws-
-obamacare-pot-guns-and-drones/' >>> article = Article(url) .. code-block::
-pycon >>> article.download() >>> article.html '
+`Python2 branch`_ .. _`Python2 branch`: https://github.com/huangsiyuan924/
+newspaper/tree/python-2-head A Glance: --------- .. code-block:: pycon >>> from
+newspaper import Article >>> url = 'http://fox13now.com/2013/12/30/new-year-
+new-laws-obamacare-pot-guns-and-drones/' >>> article = Article(url) .. code-
+block:: pycon >>> article.download() >>> article.html '
 . code-block:: pycon >>> article.parse() >>> article.authors ['Leigh Ann
 Caldwell', 'John Honway'] >>> article.publish_date datetime.datetime(2013, 12,
 30, 0, 0) >>> article.text 'Washington (CNN) -- Not everyone subscribes to a
 New Year's resolution...' >>> article.top_image 'http://someCDN.com/blah/blah/
 blah/file.png' >>> article.movies ['http://youtube.com/path/to/link.com', ...]
 .. code-block:: pycon >>> article.nlp() >>> article.keywords ['New Years',
 'resolution', ...] >>> article.summary 'The study shows that 93% of people ...'
@@ -91,47 +94,48 @@
 following: - Install ``pip3`` command needed to install ``newspaper3k``
 package:: $ sudo apt-get install python3-pip - Python development version,
 needed for Python.h:: $ sudo apt-get install python-dev - lxml requirements:: $
 sudo apt-get install libxml2-dev libxslt-dev - For PIL to recognize .jpg
 images:: $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev NOTE: If
 you find problem installing ``libpng12-dev``, try installing ``libpng-dev``. -
 Download NLP related corpora:: $ curl https://raw.githubusercontent.com/
-codelucas/newspaper/master/download_corpora.py | python3 - Install the
+huangsiyuan924/newspaper/master/download_corpora.py | python3 - Install the
 distribution via pip:: $ pip3 install newspaper3k **If you are on OSX**,
 install using the following, you may use both homebrew or macports: :: $ brew
 install libxml2 libxslt $ brew install libtiff libjpeg webp little-cms2 $ pip3
-install newspaper3k $ curl https://raw.githubusercontent.com/codelucas/
+install newspaper3k $ curl https://raw.githubusercontent.com/huangsiyuan924/
 newspaper/master/download_corpora.py | python3 **Otherwise**, install with the
 following: NOTE: You will still most likely need to install the following
 libraries via your package manager - PIL: ``libjpeg-dev`` ``zlib1g-dev``
 ``libpng12-dev`` - lxml: ``libxml2-dev`` ``libxslt-dev`` - Python Development
 version: ``python-dev`` :: $ pip3 install newspaper3k $ curl https://
-raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py |
+raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py |
 python3 Donations --------- Your donations are greatly appreciated! They will
 free me up to work on this project more, to take on things like: adding new
 features, bug-fix support, addressing concerns with the library. - My PayPal
-link: `https://www.paypal.me/codelucas`_ - My `Venmo`_ handle: @Lucas-Ou-Yang
-Development ----------- If you'd like to contribute and hack on the newspaper
-project, feel free to clone a development version of this repository locally::
-git clone git://github.com/codelucas/newspaper.git Once you have a copy of the
-source, you can embed it in your Python package, or install it into your site-
-packages easily:: $ pip3 install -r requirements.txt $ python3 setup.py install
-Feel free to give our testing suite a shot, everything is mocked!:: $ python3
-tests/unit_tests.py Planning on tweaking our full-text algorithm? Add the
-``fulltext`` parameter:: $ python3 tests/unit_tests.py fulltext Demo ---- View
-a working online demo here: http://newspaper-demo.herokuapp.com This is another
-working online demo: http://newspaper.chinazt.cc/ LICENSE ------- Authored and
-maintained by `Lucas Ou-Yang`_. `Parse.ly`_ sponsored some work on newspaper,
-specifically focused on automatic extraction. Newspaper uses a lot of `python-
-goose's`_ parsing code. View their license `here`_. Please feel free to `email
-& contact me`_ if you run into issues or just would like to talk about the
-future of this library and news extraction in general! .. _`Lucas Ou-Yang`:
-http://codelucas.com .. _`email & contact me`: mailto:
-lucasyangpersonal@gmail.com .. _`python-goose's`: https://github.com/grangier/
-python-goose .. _`here`: https://github.com/codelucas/newspaper/blob/master/
-GOOSE-LICENSE.txt .. _`https://www.paypal.me/codelucas`: https://www.paypal.me/
-codelucas .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart
-guide`: https://newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
+link: `https://www.paypal.me/huangsiyuan924`_ - My `Venmo`_ handle: @Lucas-Ou-
+Yang Development ----------- If you'd like to contribute and hack on the
+newspaper project, feel free to clone a development version of this repository
+locally:: git clone git://github.com/huangsiyuan924/newspaper.git Once you have
+a copy of the source, you can embed it in your Python package, or install it
+into your site-packages easily:: $ pip3 install -r requirements.txt $ python3
+setup.py install Feel free to give our testing suite a shot, everything is
+mocked!:: $ python3 tests/unit_tests.py Planning on tweaking our full-text
+algorithm? Add the ``fulltext`` parameter:: $ python3 tests/unit_tests.py
+fulltext Demo ---- View a working online demo here: http://newspaper-
+demo.herokuapp.com This is another working online demo: http://
+newspaper.chinazt.cc/ LICENSE ------- Authored and maintained by `Lucas Ou-
+Yang`_. `Parse.ly`_ sponsored some work on newspaper, specifically focused on
+automatic extraction. Newspaper uses a lot of `python-goose's`_ parsing code.
+View their license `here`_. Please feel free to `email & contact me`_ if you
+run into issues or just would like to talk about the future of this library and
+news extraction in general! .. _`Lucas Ou-Yang`: http://huangsiyuan924.com ..
+_`email & contact me`: mailto:lucasyangpersonal@gmail.com .. _`python-goose's`:
+https://github.com/grangier/python-goose .. _`here`: https://github.com/
+huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt .. _`https://
+www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924 ..
+_`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart guide`: https://
+newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
 newspaper.readthedocs.io .. _`lxml`: http://lxml.de/ .. _`requests`: https://
 github.com/kennethreitz/requests .. _`Parse.ly`: http://parse.ly .. _`It takes
 only one click`: https://tracking.gitads.io/
 ?campaign=gitads&repo=newspaper&redirect=gitads.io
```

### Comparing `hsy_newspaper3k-0.3.2/README.rst` & `hsy-newspaper3k-0.3.8/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Newspaper3k: Article scraping & curation
 ========================================
 
 .. image:: https://badge.fury.io/py/newspaper3k.svg
     :target: http://badge.fury.io/py/newspaper3k.svg
         :alt: Latest version
 
-.. image:: https://travis-ci.org/codelucas/newspaper.svg
-        :target: http://travis-ci.org/codelucas/newspaper/
+.. image:: https://travis-ci.org/huangsiyuan924/newspaper.svg
+        :target: http://travis-ci.org/huangsiyuan924/newspaper/
         :alt: Build status
 
-.. image:: https://coveralls.io/repos/github/codelucas/newspaper/badge.svg?branch=master
-        :target: https://coveralls.io/github/codelucas/newspaper
+.. image:: https://coveralls.io/repos/github/huangsiyuan924/newspaper/badge.svg?branch=master
+        :target: https://coveralls.io/github/huangsiyuan924/newspaper
         :alt: Coverage status
 
 
 Inspired by `requests`_ for its simplicity and powered by `lxml`_ for its speed:
 
     "Newspaper is an amazing python library for extracting & curating articles."
     -- `tweeted by`_ Kenneth Reitz, Author of `requests`_
@@ -22,15 +22,15 @@
     "Newspaper delivers Instapaper style article extraction." -- `The Changelog`_
 
 .. _`tweeted by`: https://twitter.com/kennethreitz/status/419520678862548992
 .. _`The Changelog`: http://thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
 
 **Newspaper is a Python3 library**! Or, view our **deprecated and buggy** `Python2 branch`_
 
-.. _`Python2 branch`: https://github.com/codelucas/newspaper/tree/python-2-head
+.. _`Python2 branch`: https://github.com/huangsiyuan924/newspaper/tree/python-2-head
 
 A Glance:
 ---------
 
 .. code-block:: pycon
 
     >>> from newspaper import Article
@@ -265,15 +265,15 @@
 
     $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev
 
 NOTE: If you find problem installing ``libpng12-dev``, try installing ``libpng-dev``.
 
 - Download NLP related corpora::
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 - Install the distribution via pip::
 
     $ pip3 install newspaper3k
 
 **If you are on OSX**, install using the following, you may use both homebrew or macports:
 
@@ -281,47 +281,47 @@
 
     $ brew install libxml2 libxslt
 
     $ brew install libtiff libjpeg webp little-cms2
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 
 **Otherwise**, install with the following:
 
 NOTE: You will still most likely need to install the following libraries via your package manager
 
 - PIL: ``libjpeg-dev`` ``zlib1g-dev`` ``libpng12-dev``
 - lxml: ``libxml2-dev`` ``libxslt-dev``
 - Python Development version: ``python-dev``
 
 ::
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 Donations
 ---------
 
 Your donations are greatly appreciated! They will free me up to work on this project more,
 to take on things like: adding new features, bug-fix support, addressing concerns with the library.
 
-- My PayPal link: `https://www.paypal.me/codelucas`_
+- My PayPal link: `https://www.paypal.me/huangsiyuan924`_
 - My `Venmo`_ handle: @Lucas-Ou-Yang
 
 Development
 -----------
 
 If you'd like to contribute and hack on the newspaper project, feel free to clone
 a development version of this repository locally::
 
-    git clone git://github.com/codelucas/newspaper.git
+    git clone git://github.com/huangsiyuan924/newspaper.git
 
 Once you have a copy of the source, you can embed it in your Python package,
 or install it into your site-packages easily::
 
     $ pip3 install -r requirements.txt
     $ python3 setup.py install
 
@@ -350,20 +350,20 @@
 automatic extraction.
 
 Newspaper uses a lot of `python-goose's`_ parsing code. View their license `here`_.
 
 Please feel free to `email & contact me`_ if you run into issues or just would like
 to talk about the future of this library and news extraction in general!
 
-.. _`Lucas Ou-Yang`: http://codelucas.com
+.. _`Lucas Ou-Yang`: http://huangsiyuan924.com
 .. _`email & contact me`: mailto:lucasyangpersonal@gmail.com
 .. _`python-goose's`: https://github.com/grangier/python-goose
-.. _`here`: https://github.com/codelucas/newspaper/blob/master/GOOSE-LICENSE.txt
+.. _`here`: https://github.com/huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt
 
-.. _`https://www.paypal.me/codelucas`: https://www.paypal.me/codelucas
+.. _`https://www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924
 .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang
 
 .. _`Quickstart guide`: https://newspaper.readthedocs.io/en/latest/
 .. _`The Docs`: https://newspaper.readthedocs.io
 .. _`lxml`: http://lxml.de/
 .. _`requests`: https://github.com/kennethreitz/requests
 .. _`Parse.ly`: http://parse.ly
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
 Newspaper3k: Article scraping & curation
 ======================================== .. image:: https://badge.fury.io/py/
 newspaper3k.svg :target: http://badge.fury.io/py/newspaper3k.svg :alt: Latest
-version .. image:: https://travis-ci.org/codelucas/newspaper.svg :target: http:
-//travis-ci.org/codelucas/newspaper/ :alt: Build status .. image:: https://
-coveralls.io/repos/github/codelucas/newspaper/badge.svg?branch=master :target:
-https://coveralls.io/github/codelucas/newspaper :alt: Coverage status Inspired
-by `requests`_ for its simplicity and powered by `lxml`_ for its speed:
-"Newspaper is an amazing python library for extracting & curating articles." -
-- `tweeted by`_ Kenneth Reitz, Author of `requests`_ "Newspaper delivers
-Instapaper style article extraction." -- `The Changelog`_ .. _`tweeted by`:
-https://twitter.com/kennethreitz/status/419520678862548992 .. _`The Changelog`:
-http://thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
-**Newspaper is a Python3 library**! Or, view our **deprecated and buggy**
-`Python2 branch`_ .. _`Python2 branch`: https://github.com/codelucas/newspaper/
-tree/python-2-head A Glance: --------- .. code-block:: pycon >>> from newspaper
-import Article >>> url = 'http://fox13now.com/2013/12/30/new-year-new-laws-
-obamacare-pot-guns-and-drones/' >>> article = Article(url) .. code-block::
-pycon >>> article.download() >>> article.html '
+version .. image:: https://travis-ci.org/huangsiyuan924/newspaper.svg :target:
+http://travis-ci.org/huangsiyuan924/newspaper/ :alt: Build status .. image::
+https://coveralls.io/repos/github/huangsiyuan924/newspaper/
+badge.svg?branch=master :target: https://coveralls.io/github/huangsiyuan924/
+newspaper :alt: Coverage status Inspired by `requests`_ for its simplicity and
+powered by `lxml`_ for its speed: "Newspaper is an amazing python library for
+extracting & curating articles." -- `tweeted by`_ Kenneth Reitz, Author of
+`requests`_ "Newspaper delivers Instapaper style article extraction." -- `The
+Changelog`_ .. _`tweeted by`: https://twitter.com/kennethreitz/status/
+419520678862548992 .. _`The Changelog`: http://thechangelog.com/newspaper-
+delivers-instapaper-style-article-extraction/ **Newspaper is a Python3
+library**! Or, view our **deprecated and buggy** `Python2 branch`_ .. _`Python2
+branch`: https://github.com/huangsiyuan924/newspaper/tree/python-2-head A
+Glance: --------- .. code-block:: pycon >>> from newspaper import Article >>>
+url = 'http://fox13now.com/2013/12/30/new-year-new-laws-obamacare-pot-guns-and-
+drones/' >>> article = Article(url) .. code-block:: pycon >>> article.download
+() >>> article.html '
 . code-block:: pycon >>> article.parse() >>> article.authors ['Leigh Ann
 Caldwell', 'John Honway'] >>> article.publish_date datetime.datetime(2013, 12,
 30, 0, 0) >>> article.text 'Washington (CNN) -- Not everyone subscribes to a
 New Year's resolution...' >>> article.top_image 'http://someCDN.com/blah/blah/
 blah/file.png' >>> article.movies ['http://youtube.com/path/to/link.com', ...]
 .. code-block:: pycon >>> article.nlp() >>> article.keywords ['New Years',
 'resolution', ...] >>> article.summary 'The study shows that 93% of people ...'
@@ -85,47 +86,48 @@
 following: - Install ``pip3`` command needed to install ``newspaper3k``
 package:: $ sudo apt-get install python3-pip - Python development version,
 needed for Python.h:: $ sudo apt-get install python-dev - lxml requirements:: $
 sudo apt-get install libxml2-dev libxslt-dev - For PIL to recognize .jpg
 images:: $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev NOTE: If
 you find problem installing ``libpng12-dev``, try installing ``libpng-dev``. -
 Download NLP related corpora:: $ curl https://raw.githubusercontent.com/
-codelucas/newspaper/master/download_corpora.py | python3 - Install the
+huangsiyuan924/newspaper/master/download_corpora.py | python3 - Install the
 distribution via pip:: $ pip3 install newspaper3k **If you are on OSX**,
 install using the following, you may use both homebrew or macports: :: $ brew
 install libxml2 libxslt $ brew install libtiff libjpeg webp little-cms2 $ pip3
-install newspaper3k $ curl https://raw.githubusercontent.com/codelucas/
+install newspaper3k $ curl https://raw.githubusercontent.com/huangsiyuan924/
 newspaper/master/download_corpora.py | python3 **Otherwise**, install with the
 following: NOTE: You will still most likely need to install the following
 libraries via your package manager - PIL: ``libjpeg-dev`` ``zlib1g-dev``
 ``libpng12-dev`` - lxml: ``libxml2-dev`` ``libxslt-dev`` - Python Development
 version: ``python-dev`` :: $ pip3 install newspaper3k $ curl https://
-raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py |
+raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py |
 python3 Donations --------- Your donations are greatly appreciated! They will
 free me up to work on this project more, to take on things like: adding new
 features, bug-fix support, addressing concerns with the library. - My PayPal
-link: `https://www.paypal.me/codelucas`_ - My `Venmo`_ handle: @Lucas-Ou-Yang
-Development ----------- If you'd like to contribute and hack on the newspaper
-project, feel free to clone a development version of this repository locally::
-git clone git://github.com/codelucas/newspaper.git Once you have a copy of the
-source, you can embed it in your Python package, or install it into your site-
-packages easily:: $ pip3 install -r requirements.txt $ python3 setup.py install
-Feel free to give our testing suite a shot, everything is mocked!:: $ python3
-tests/unit_tests.py Planning on tweaking our full-text algorithm? Add the
-``fulltext`` parameter:: $ python3 tests/unit_tests.py fulltext Demo ---- View
-a working online demo here: http://newspaper-demo.herokuapp.com This is another
-working online demo: http://newspaper.chinazt.cc/ LICENSE ------- Authored and
-maintained by `Lucas Ou-Yang`_. `Parse.ly`_ sponsored some work on newspaper,
-specifically focused on automatic extraction. Newspaper uses a lot of `python-
-goose's`_ parsing code. View their license `here`_. Please feel free to `email
-& contact me`_ if you run into issues or just would like to talk about the
-future of this library and news extraction in general! .. _`Lucas Ou-Yang`:
-http://codelucas.com .. _`email & contact me`: mailto:
-lucasyangpersonal@gmail.com .. _`python-goose's`: https://github.com/grangier/
-python-goose .. _`here`: https://github.com/codelucas/newspaper/blob/master/
-GOOSE-LICENSE.txt .. _`https://www.paypal.me/codelucas`: https://www.paypal.me/
-codelucas .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart
-guide`: https://newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
+link: `https://www.paypal.me/huangsiyuan924`_ - My `Venmo`_ handle: @Lucas-Ou-
+Yang Development ----------- If you'd like to contribute and hack on the
+newspaper project, feel free to clone a development version of this repository
+locally:: git clone git://github.com/huangsiyuan924/newspaper.git Once you have
+a copy of the source, you can embed it in your Python package, or install it
+into your site-packages easily:: $ pip3 install -r requirements.txt $ python3
+setup.py install Feel free to give our testing suite a shot, everything is
+mocked!:: $ python3 tests/unit_tests.py Planning on tweaking our full-text
+algorithm? Add the ``fulltext`` parameter:: $ python3 tests/unit_tests.py
+fulltext Demo ---- View a working online demo here: http://newspaper-
+demo.herokuapp.com This is another working online demo: http://
+newspaper.chinazt.cc/ LICENSE ------- Authored and maintained by `Lucas Ou-
+Yang`_. `Parse.ly`_ sponsored some work on newspaper, specifically focused on
+automatic extraction. Newspaper uses a lot of `python-goose's`_ parsing code.
+View their license `here`_. Please feel free to `email & contact me`_ if you
+run into issues or just would like to talk about the future of this library and
+news extraction in general! .. _`Lucas Ou-Yang`: http://huangsiyuan924.com ..
+_`email & contact me`: mailto:lucasyangpersonal@gmail.com .. _`python-goose's`:
+https://github.com/grangier/python-goose .. _`here`: https://github.com/
+huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt .. _`https://
+www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924 ..
+_`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart guide`: https://
+newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
 newspaper.readthedocs.io .. _`lxml`: http://lxml.de/ .. _`requests`: https://
 github.com/kennethreitz/requests .. _`Parse.ly`: http://parse.ly .. _`It takes
 only one click`: https://tracking.gitads.io/
 ?campaign=gitads&repo=newspaper&redirect=gitads.io
```

### Comparing `hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/PKG-INFO` & `hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: hsy-newspaper3k
-Version: 0.3.2
+Version: 0.3.8
 Summary: Simplified python article discovery & extraction.
 Home-page: https://github.com/huangsiyuan924/newspaper/
-Author: Lucas Ou-Yang
-Author-email: lucasyangpersonal@gmail.com
+Author: Siyuan Huang
+Author-email: huangsiyuan924@gmail.com
 License: MIT
+Project-URL: Source, https://github.com/huangsiyuan924/newspaper/
+Project-URL: Documentation, https://github.com/huangsiyuan924/newspaper/
+Project-URL: Bug Tracker, https://github.com/huangsiyuan924/newspaper//issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 License-File: LICENSE
 
 Newspaper3k: Article scraping & curation
 ========================================
 
 .. image:: https://badge.fury.io/py/newspaper3k.svg
     :target: http://badge.fury.io/py/newspaper3k.svg
         :alt: Latest version
 
-.. image:: https://travis-ci.org/codelucas/newspaper.svg
-        :target: http://travis-ci.org/codelucas/newspaper/
+.. image:: https://travis-ci.org/huangsiyuan924/newspaper.svg
+        :target: http://travis-ci.org/huangsiyuan924/newspaper/
         :alt: Build status
 
-.. image:: https://coveralls.io/repos/github/codelucas/newspaper/badge.svg?branch=master
-        :target: https://coveralls.io/github/codelucas/newspaper
+.. image:: https://coveralls.io/repos/github/huangsiyuan924/newspaper/badge.svg?branch=master
+        :target: https://coveralls.io/github/huangsiyuan924/newspaper
         :alt: Coverage status
 
 
 Inspired by `requests`_ for its simplicity and powered by `lxml`_ for its speed:
 
     "Newspaper is an amazing python library for extracting & curating articles."
     -- `tweeted by`_ Kenneth Reitz, Author of `requests`_
@@ -36,15 +39,15 @@
     "Newspaper delivers Instapaper style article extraction." -- `The Changelog`_
 
 .. _`tweeted by`: https://twitter.com/kennethreitz/status/419520678862548992
 .. _`The Changelog`: http://thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
 
 **Newspaper is a Python3 library**! Or, view our **deprecated and buggy** `Python2 branch`_
 
-.. _`Python2 branch`: https://github.com/codelucas/newspaper/tree/python-2-head
+.. _`Python2 branch`: https://github.com/huangsiyuan924/newspaper/tree/python-2-head
 
 A Glance:
 ---------
 
 .. code-block:: pycon
 
     >>> from newspaper import Article
@@ -279,15 +282,15 @@
 
     $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev
 
 NOTE: If you find problem installing ``libpng12-dev``, try installing ``libpng-dev``.
 
 - Download NLP related corpora::
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 - Install the distribution via pip::
 
     $ pip3 install newspaper3k
 
 **If you are on OSX**, install using the following, you may use both homebrew or macports:
 
@@ -295,47 +298,47 @@
 
     $ brew install libxml2 libxslt
 
     $ brew install libtiff libjpeg webp little-cms2
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 
 **Otherwise**, install with the following:
 
 NOTE: You will still most likely need to install the following libraries via your package manager
 
 - PIL: ``libjpeg-dev`` ``zlib1g-dev`` ``libpng12-dev``
 - lxml: ``libxml2-dev`` ``libxslt-dev``
 - Python Development version: ``python-dev``
 
 ::
 
     $ pip3 install newspaper3k
 
-    $ curl https://raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py | python3
+    $ curl https://raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py | python3
 
 Donations
 ---------
 
 Your donations are greatly appreciated! They will free me up to work on this project more,
 to take on things like: adding new features, bug-fix support, addressing concerns with the library.
 
-- My PayPal link: `https://www.paypal.me/codelucas`_
+- My PayPal link: `https://www.paypal.me/huangsiyuan924`_
 - My `Venmo`_ handle: @Lucas-Ou-Yang
 
 Development
 -----------
 
 If you'd like to contribute and hack on the newspaper project, feel free to clone
 a development version of this repository locally::
 
-    git clone git://github.com/codelucas/newspaper.git
+    git clone git://github.com/huangsiyuan924/newspaper.git
 
 Once you have a copy of the source, you can embed it in your Python package,
 or install it into your site-packages easily::
 
     $ pip3 install -r requirements.txt
     $ python3 setup.py install
 
@@ -364,20 +367,20 @@
 automatic extraction.
 
 Newspaper uses a lot of `python-goose's`_ parsing code. View their license `here`_.
 
 Please feel free to `email & contact me`_ if you run into issues or just would like
 to talk about the future of this library and news extraction in general!
 
-.. _`Lucas Ou-Yang`: http://codelucas.com
+.. _`Lucas Ou-Yang`: http://huangsiyuan924.com
 .. _`email & contact me`: mailto:lucasyangpersonal@gmail.com
 .. _`python-goose's`: https://github.com/grangier/python-goose
-.. _`here`: https://github.com/codelucas/newspaper/blob/master/GOOSE-LICENSE.txt
+.. _`here`: https://github.com/huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt
 
-.. _`https://www.paypal.me/codelucas`: https://www.paypal.me/codelucas
+.. _`https://www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924
 .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang
 
 .. _`Quickstart guide`: https://newspaper.readthedocs.io/en/latest/
 .. _`The Docs`: https://newspaper.readthedocs.io
 .. _`lxml`: http://lxml.de/
 .. _`requests`: https://github.com/kennethreitz/requests
 .. _`Parse.ly`: http://parse.ly
```

#### html2text {}

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1 Name: hsy-newspaper3k Version: 0.3.2 Summary: Simplified
+Metadata-Version: 2.1 Name: hsy-newspaper3k Version: 0.3.8 Summary: Simplified
 python article discovery & extraction. Home-page: https://github.com/
-huangsiyuan924/newspaper/ Author: Lucas Ou-Yang Author-email:
-lucasyangpersonal@gmail.com License: MIT Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers License-File: LICENSE Newspaper3k:
-Article scraping & curation ======================================== .. image::
-https://badge.fury.io/py/newspaper3k.svg :target: http://badge.fury.io/py/
+huangsiyuan924/newspaper/ Author: Siyuan Huang Author-email:
+huangsiyuan924@gmail.com License: MIT Project-URL: Source, https://github.com/
+huangsiyuan924/newspaper/ Project-URL: Documentation, https://github.com/
+huangsiyuan924/newspaper/ Project-URL: Bug Tracker, https://github.com/
+huangsiyuan924/newspaper//issues Platform: UNKNOWN Classifier: Programming
+Language :: Python :: 3 Classifier: Natural Language :: English Classifier:
+Intended Audience :: Developers License-File: LICENSE Newspaper3k: Article
+scraping & curation ======================================== .. image:: https:/
+/badge.fury.io/py/newspaper3k.svg :target: http://badge.fury.io/py/
 newspaper3k.svg :alt: Latest version .. image:: https://travis-ci.org/
-codelucas/newspaper.svg :target: http://travis-ci.org/codelucas/newspaper/ :
-alt: Build status .. image:: https://coveralls.io/repos/github/codelucas/
-newspaper/badge.svg?branch=master :target: https://coveralls.io/github/
-codelucas/newspaper :alt: Coverage status Inspired by `requests`_ for its
-simplicity and powered by `lxml`_ for its speed: "Newspaper is an amazing
-python library for extracting & curating articles." -- `tweeted by`_ Kenneth
-Reitz, Author of `requests`_ "Newspaper delivers Instapaper style article
-extraction." -- `The Changelog`_ .. _`tweeted by`: https://twitter.com/
+huangsiyuan924/newspaper.svg :target: http://travis-ci.org/huangsiyuan924/
+newspaper/ :alt: Build status .. image:: https://coveralls.io/repos/github/
+huangsiyuan924/newspaper/badge.svg?branch=master :target: https://coveralls.io/
+github/huangsiyuan924/newspaper :alt: Coverage status Inspired by `requests`_
+for its simplicity and powered by `lxml`_ for its speed: "Newspaper is an
+amazing python library for extracting & curating articles." -- `tweeted by`_
+Kenneth Reitz, Author of `requests`_ "Newspaper delivers Instapaper style
+article extraction." -- `The Changelog`_ .. _`tweeted by`: https://twitter.com/
 kennethreitz/status/419520678862548992 .. _`The Changelog`: http://
 thechangelog.com/newspaper-delivers-instapaper-style-article-extraction/
 **Newspaper is a Python3 library**! Or, view our **deprecated and buggy**
-`Python2 branch`_ .. _`Python2 branch`: https://github.com/codelucas/newspaper/
-tree/python-2-head A Glance: --------- .. code-block:: pycon >>> from newspaper
-import Article >>> url = 'http://fox13now.com/2013/12/30/new-year-new-laws-
-obamacare-pot-guns-and-drones/' >>> article = Article(url) .. code-block::
-pycon >>> article.download() >>> article.html '
+`Python2 branch`_ .. _`Python2 branch`: https://github.com/huangsiyuan924/
+newspaper/tree/python-2-head A Glance: --------- .. code-block:: pycon >>> from
+newspaper import Article >>> url = 'http://fox13now.com/2013/12/30/new-year-
+new-laws-obamacare-pot-guns-and-drones/' >>> article = Article(url) .. code-
+block:: pycon >>> article.download() >>> article.html '
 . code-block:: pycon >>> article.parse() >>> article.authors ['Leigh Ann
 Caldwell', 'John Honway'] >>> article.publish_date datetime.datetime(2013, 12,
 30, 0, 0) >>> article.text 'Washington (CNN) -- Not everyone subscribes to a
 New Year's resolution...' >>> article.top_image 'http://someCDN.com/blah/blah/
 blah/file.png' >>> article.movies ['http://youtube.com/path/to/link.com', ...]
 .. code-block:: pycon >>> article.nlp() >>> article.keywords ['New Years',
 'resolution', ...] >>> article.summary 'The study shows that 93% of people ...'
@@ -91,47 +94,48 @@
 following: - Install ``pip3`` command needed to install ``newspaper3k``
 package:: $ sudo apt-get install python3-pip - Python development version,
 needed for Python.h:: $ sudo apt-get install python-dev - lxml requirements:: $
 sudo apt-get install libxml2-dev libxslt-dev - For PIL to recognize .jpg
 images:: $ sudo apt-get install libjpeg-dev zlib1g-dev libpng12-dev NOTE: If
 you find problem installing ``libpng12-dev``, try installing ``libpng-dev``. -
 Download NLP related corpora:: $ curl https://raw.githubusercontent.com/
-codelucas/newspaper/master/download_corpora.py | python3 - Install the
+huangsiyuan924/newspaper/master/download_corpora.py | python3 - Install the
 distribution via pip:: $ pip3 install newspaper3k **If you are on OSX**,
 install using the following, you may use both homebrew or macports: :: $ brew
 install libxml2 libxslt $ brew install libtiff libjpeg webp little-cms2 $ pip3
-install newspaper3k $ curl https://raw.githubusercontent.com/codelucas/
+install newspaper3k $ curl https://raw.githubusercontent.com/huangsiyuan924/
 newspaper/master/download_corpora.py | python3 **Otherwise**, install with the
 following: NOTE: You will still most likely need to install the following
 libraries via your package manager - PIL: ``libjpeg-dev`` ``zlib1g-dev``
 ``libpng12-dev`` - lxml: ``libxml2-dev`` ``libxslt-dev`` - Python Development
 version: ``python-dev`` :: $ pip3 install newspaper3k $ curl https://
-raw.githubusercontent.com/codelucas/newspaper/master/download_corpora.py |
+raw.githubusercontent.com/huangsiyuan924/newspaper/master/download_corpora.py |
 python3 Donations --------- Your donations are greatly appreciated! They will
 free me up to work on this project more, to take on things like: adding new
 features, bug-fix support, addressing concerns with the library. - My PayPal
-link: `https://www.paypal.me/codelucas`_ - My `Venmo`_ handle: @Lucas-Ou-Yang
-Development ----------- If you'd like to contribute and hack on the newspaper
-project, feel free to clone a development version of this repository locally::
-git clone git://github.com/codelucas/newspaper.git Once you have a copy of the
-source, you can embed it in your Python package, or install it into your site-
-packages easily:: $ pip3 install -r requirements.txt $ python3 setup.py install
-Feel free to give our testing suite a shot, everything is mocked!:: $ python3
-tests/unit_tests.py Planning on tweaking our full-text algorithm? Add the
-``fulltext`` parameter:: $ python3 tests/unit_tests.py fulltext Demo ---- View
-a working online demo here: http://newspaper-demo.herokuapp.com This is another
-working online demo: http://newspaper.chinazt.cc/ LICENSE ------- Authored and
-maintained by `Lucas Ou-Yang`_. `Parse.ly`_ sponsored some work on newspaper,
-specifically focused on automatic extraction. Newspaper uses a lot of `python-
-goose's`_ parsing code. View their license `here`_. Please feel free to `email
-& contact me`_ if you run into issues or just would like to talk about the
-future of this library and news extraction in general! .. _`Lucas Ou-Yang`:
-http://codelucas.com .. _`email & contact me`: mailto:
-lucasyangpersonal@gmail.com .. _`python-goose's`: https://github.com/grangier/
-python-goose .. _`here`: https://github.com/codelucas/newspaper/blob/master/
-GOOSE-LICENSE.txt .. _`https://www.paypal.me/codelucas`: https://www.paypal.me/
-codelucas .. _`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart
-guide`: https://newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
+link: `https://www.paypal.me/huangsiyuan924`_ - My `Venmo`_ handle: @Lucas-Ou-
+Yang Development ----------- If you'd like to contribute and hack on the
+newspaper project, feel free to clone a development version of this repository
+locally:: git clone git://github.com/huangsiyuan924/newspaper.git Once you have
+a copy of the source, you can embed it in your Python package, or install it
+into your site-packages easily:: $ pip3 install -r requirements.txt $ python3
+setup.py install Feel free to give our testing suite a shot, everything is
+mocked!:: $ python3 tests/unit_tests.py Planning on tweaking our full-text
+algorithm? Add the ``fulltext`` parameter:: $ python3 tests/unit_tests.py
+fulltext Demo ---- View a working online demo here: http://newspaper-
+demo.herokuapp.com This is another working online demo: http://
+newspaper.chinazt.cc/ LICENSE ------- Authored and maintained by `Lucas Ou-
+Yang`_. `Parse.ly`_ sponsored some work on newspaper, specifically focused on
+automatic extraction. Newspaper uses a lot of `python-goose's`_ parsing code.
+View their license `here`_. Please feel free to `email & contact me`_ if you
+run into issues or just would like to talk about the future of this library and
+news extraction in general! .. _`Lucas Ou-Yang`: http://huangsiyuan924.com ..
+_`email & contact me`: mailto:lucasyangpersonal@gmail.com .. _`python-goose's`:
+https://github.com/grangier/python-goose .. _`here`: https://github.com/
+huangsiyuan924/newspaper/blob/master/GOOSE-LICENSE.txt .. _`https://
+www.paypal.me/huangsiyuan924`: https://www.paypal.me/huangsiyuan924 ..
+_`Venmo`: https://www.venmo.com/Lucas-Ou-Yang .. _`Quickstart guide`: https://
+newspaper.readthedocs.io/en/latest/ .. _`The Docs`: https://
 newspaper.readthedocs.io .. _`lxml`: http://lxml.de/ .. _`requests`: https://
 github.com/kennethreitz/requests .. _`Parse.ly`: http://parse.ly .. _`It takes
 only one click`: https://tracking.gitads.io/
 ?campaign=gitads&repo=newspaper&redirect=gitads.io
```

### Comparing `hsy_newspaper3k-0.3.2/hsy_newspaper3k.egg-info/SOURCES.txt` & `hsy-newspaper3k-0.3.8/hsy_newspaper3k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/__init__.py` & `hsy-newspaper3k-0.3.8/newspaper/__init__.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/api.py` & `hsy-newspaper3k-0.3.8/newspaper/api.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/article.py` & `hsy-newspaper3k-0.3.8/newspaper/article.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/cleaners.py` & `hsy-newspaper3k-0.3.8/newspaper/cleaners.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/configuration.py` & `hsy-newspaper3k-0.3.8/newspaper/configuration.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/extractors.py` & `hsy-newspaper3k-0.3.8/newspaper/extractors.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/images.py` & `hsy-newspaper3k-0.3.8/newspaper/images.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/mthreading.py` & `hsy-newspaper3k-0.3.8/newspaper/mthreading.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/network.py` & `hsy-newspaper3k-0.3.8/newspaper/network.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/nlp.py` & `hsy-newspaper3k-0.3.8/newspaper/nlp.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/outputformatters.py` & `hsy-newspaper3k-0.3.8/newspaper/outputformatters.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/parsers.py` & `hsy-newspaper3k-0.3.8/newspaper/parsers.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/misc/google_sources.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/misc/google_sources.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/misc/popular_sources.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/misc/popular_sources.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/misc/stopwords-nlp-en.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/misc/stopwords-nlp-en.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/misc/useragents.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/misc/useragents.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ar.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ar.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-be.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-be.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-bg.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-bg.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-de.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-de.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-el.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-el.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-en.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-en.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-es.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-es.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-fa.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-fa.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-fr.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-fr.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-he.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-he.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hi.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hi.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hr.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hr.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-hu.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-hu.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-id.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-id.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-it.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-it.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ja.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ja.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-lt.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-lt.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-mk.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-mk.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-nb.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-nb.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-no.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-no.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-pl.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-pl.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-pt.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-pt.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ro.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ro.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-ru.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-ru.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sl.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sl.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sr.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sr.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-sv.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-sv.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-th.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-th.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-tr.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-tr.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-uk.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-uk.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-vi.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-vi.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/resources/text/stopwords-zh.txt` & `hsy-newspaper3k-0.3.8/newspaper/resources/text/stopwords-zh.txt`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/settings.py` & `hsy-newspaper3k-0.3.8/newspaper/settings.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/source.py` & `hsy-newspaper3k-0.3.8/newspaper/source.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/text.py` & `hsy-newspaper3k-0.3.8/newspaper/text.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/urls.py` & `hsy-newspaper3k-0.3.8/newspaper/urls.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/utils.py` & `hsy-newspaper3k-0.3.8/newspaper/utils.py`

 * *Files identical despite different names*

### Comparing `hsy_newspaper3k-0.3.2/newspaper/videos/extractors.py` & `hsy-newspaper3k-0.3.8/newspaper/videos/extractors.py`

 * *Files identical despite different names*

