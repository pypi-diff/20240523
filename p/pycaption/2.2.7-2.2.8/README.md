# Comparing `tmp/pycaption-2.2.7.tar.gz` & `tmp/pycaption-2.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaption-2.2.7.tar", last modified: Tue May 14 07:51:14 2024, max compression
+gzip compressed data, was "pycaption-2.2.8.tar", last modified: Thu May 23 08:44:32 2024, max compression
```

## Comparing `pycaption-2.2.7.tar` & `pycaption-2.2.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-14 07:50:55.000000 pycaption-2.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 07:50:55.000000 pycaption-2.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-14 07:51:14.405020 pycaption-2.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-14 07:50:55.000000 pycaption-2.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/dfxp/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/dfxp/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/english.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/sami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.397020 pycaption-2.2.7/pycaption/scc/
--rw-r--r--   0 runner    (1001) docker     (127)    24902 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/specialized_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/state_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/scc/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-14 07:50:55.000000 pycaption-2.2.7/pycaption/webvtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/pycaption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 07:51:14.000000 pycaption-2.2.7/pycaption.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:51:14.405020 pycaption-2.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-14 07:50:55.000000 pycaption-2.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.401020 pycaption-2.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:51:14.405020 pycaption-2.2.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/sami.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/translated_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/fixtures/webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_dfxp_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_microdvd.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_microdvd_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_sami.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_sami_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_scc_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_srt_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_webvtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-14 07:50:55.000000 pycaption-2.2.7/tests/test_webvtt_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.771030 pycaption-2.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-23 08:44:19.000000 pycaption-2.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 08:44:19.000000 pycaption-2.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 08:44:32.771030 pycaption-2.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 08:44:19.000000 pycaption-2.2.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.759030 pycaption-2.2.8/pycaption/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.763030 pycaption-2.2.8/pycaption/dfxp/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50759 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/dfxp/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)   433305 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/english.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30173 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28247 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/sami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.763030 pycaption-2.2.8/pycaption/scc/
+-rw-r--r--   0 runner    (1001) docker     (127)    26057 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28154 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/specialized_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/state_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32255 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/scc/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-23 08:44:19.000000 pycaption-2.2.8/pycaption/webvtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/pycaption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 08:44:32.000000 pycaption-2.2.8/pycaption.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:44:32.771030 pycaption-2.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-23 08:44:19.000000 pycaption-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:32.767030 pycaption-2.2.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49641 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17112 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/translated_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/fixtures/webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_dfxp_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_microdvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_microdvd_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_sami.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_sami_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23573 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_scc_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_srt_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_webvtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-23 08:44:19.000000 pycaption-2.2.8/tests/test_webvtt_conversion.py
```

### Comparing `pycaption-2.2.7/LICENSE` & `pycaption-2.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/PKG-INFO` & `pycaption-2.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.7
+Version: 2.2.8
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.7/README.rst` & `pycaption-2.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/__init__.py` & `pycaption-2.2.8/pycaption/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/base.py` & `pycaption-2.2.8/pycaption/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/dfxp/base.py` & `pycaption-2.2.8/pycaption/dfxp/base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/dfxp/extras.py` & `pycaption-2.2.8/pycaption/dfxp/extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/english.pickle` & `pycaption-2.2.8/pycaption/english.pickle`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/exceptions.py` & `pycaption-2.2.8/pycaption/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/geometry.py` & `pycaption-2.2.8/pycaption/geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/microdvd.py` & `pycaption-2.2.8/pycaption/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/sami.py` & `pycaption-2.2.8/pycaption/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/scc/__init__.py` & `pycaption-2.2.8/pycaption/scc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -304,31 +304,37 @@
 
         # split line in timestamp and words
         r = re.compile(r"([0-9:;]*)([\s\t]*)((.)*)")
         parts = r.findall(line.lower())
 
         self.time_translator.start_at(parts[0][0])
 
-        # loop through each word
-        for word in parts[0][2].split(' '):
+        word_list = parts[0][2].split(' ')
+        pacs_are_doubled = len(word_list) > 1 and word_list[0] == word_list[1]
+        for idx, word in enumerate(word_list):
             # ignore empty results or invalid commands
             word = word.strip()
+            previous_is_pac = idx > 0 and _is_pac_command(word_list[idx-1])
             if len(word) == 4:
-                self._translate_word(word)
+                self._translate_word(
+                    word=word,
+                    previous_is_pac=previous_is_pac,
+                    pacs_are_doubled=pacs_are_doubled
+                )
 
-    def _translate_word(self, word):
-        if self._handle_double_command(word):
+    def _translate_word(self, word, previous_is_pac, pacs_are_doubled):
+        if self._handle_double_command(word, pacs_are_doubled):
             # count frames for timing
             self.time_translator.increment_frames()
             return
         # first check if word is a command
         # TODO - check that all the positioning commands are here, or use
         # some other strategy to determine if the word is a command.
         if word in COMMANDS or _is_pac_command(word):
-            self._translate_command(word)
+            self._translate_command(word=word, previous_is_pac=previous_is_pac)
 
         # second, check if word is a special character
         elif word in SPECIAL_CHARS:
             self._translate_special_char(word)
 
         elif word in EXTENDED_CHARS:
             self._translate_extended_char(word)
@@ -336,50 +342,64 @@
         # third, try to convert word into 2 characters
         else:
             self._translate_characters(word)
 
         # count frames for timing only after processing a command
         self.time_translator.increment_frames()
 
-    def _handle_double_command(self, word):
+    def _handle_double_command(self, word, pacs_are_doubled):
         # If the caption is to be broadcast, each of the commands are doubled
         # up for redundancy in case the signal is garbled in transmission.
         # The decoder is programmed to ignore a second command when it is the
         # same as the first.
-        # Also like codes, Special Characters are always doubled up,
+        # If we have doubled commands we're skipping also
+        # doubled special characters and doubled extended characters
         # with only one member of each pair being displayed.
-        if word in COMMANDS or _is_pac_command(word) or word in SPECIAL_CHARS or word in EXTENDED_CHARS:
-            if word == self.last_command:
-                self.last_command = ''
-                return True
+        actionable_commands = {
+            key: COMMANDS[key] for key in COMMANDS.keys() if key != "94a1"
+        }
+        doubled_types = word in actionable_commands or _is_pac_command(word)
+        if pacs_are_doubled:
+            doubled_types = doubled_types or word in SPECIAL_CHARS or word in EXTENDED_CHARS
+
+        if doubled_types and word == self.last_command:
+            return True
             # Fix for the <position> <tab offset> <position> <tab offset>
             # repetition
-            elif _is_pac_command(word) and word in self.last_command:
-                self.last_command = ''
+        elif _is_pac_command(word) and word in self.last_command:
+            self.last_command = ''
+            return True
+        elif word in PAC_TAB_OFFSET_COMMANDS:
+            if _is_pac_command(self.last_command):
+                self.last_command += f" {word}"
+                return False
+            else:
                 return True
-            elif word in PAC_TAB_OFFSET_COMMANDS:
-                if _is_pac_command(self.last_command):
-                    self.last_command += f" {word}"
-                    return False
-                else:
-                    return True
 
         self.last_command = word
         return False
 
     def _translate_special_char(self, word):
+        self.buffer.handle_backspace(word)
+        # add to buffer
         self.buffer.add_chars(SPECIAL_CHARS[word])
 
     def _translate_extended_char(self, word):
-        self.buffer.remove_ascii_duplicate(EXTENDED_CHARS[word])
-
+        """
+        Each of the 64 Extended Characters incorporates an automatic BS.
+        When an Extended Character is received, the cursor moves to the
+        left one column position (unless the Extended Character is the first
+        character on a row), erasing any character which may be in that location,
+        then displays the Extended Character.
+        """
+        self.buffer.handle_backspace(word)
         # add to buffer
         self.buffer.add_chars(EXTENDED_CHARS[word])
 
-    def _translate_command(self, word):
+    def _translate_command(self, word, previous_is_pac):
         # if command is pop_up
         if word == '9420':
             self.buffer_dict.set_active('pop')
 
         # command is paint_on [Resume Direct Captioning]
         elif word == '9429':
             self.buffer_dict.set_active('paint')
@@ -440,15 +460,18 @@
         # 942c - Erase Displayed Memory - Clear the current screen of any
         # displayed captions or text.
         elif word == '942c' and self.pop_ons_queue:
             self._pop_on(end=self.time_translator.get_time())
 
         # If command is not one of the aforementioned, add it to buffer
         else:
-            self.buffer.interpret_command(word)
+            self.buffer.interpret_command(
+                command=word,
+                previous_is_pac=previous_is_pac
+            )
 
     def _translate_characters(self, word):
         # split word into the 2 bytes
         byte1 = word[:2]
         byte2 = word[2:]
 
         # check to see if the the bytes are recognized characters
```

### Comparing `pycaption-2.2.7/pycaption/scc/constants.py` & `pycaption-2.2.8/pycaption/scc/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1048,7 +1048,13 @@
 }
 
 MID_ROW_CODES = [
     "9120", "91a1", "91a2", "9123", "91a4", "9125", "9126",
     "91a7", "91a8", "9129", "912a", "91ab", "912c", "91ad",
     "97ae", "972f", "91ae", "912f", "94a8"
 ]
+
+BACKGROUND_COLOR_CODES = [
+    "1020", "10a1", "10a2", "1023", "10a4", "1025", "1026",
+    "10a7", "10a8", "1029", "102a", "10ab", "102c", "10ad",
+    "10ae", "102f", "97ad"
+]
```

### Comparing `pycaption-2.2.7/pycaption/scc/specialized_collections.py` & `pycaption-2.2.8/pycaption/scc/specialized_collections.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from ..base import CaptionList, Caption, CaptionNode
 from ..geometry import (
     UnitEnum, Size, Layout, Point, Alignment,
     VerticalAlignmentEnum, HorizontalAlignmentEnum
 )
 from .constants import (
     PAC_BYTES_TO_POSITIONING_MAP, COMMANDS, PAC_TAB_OFFSET_COMMANDS,
-    MICROSECONDS_PER_CODEWORD, INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION,
-    MID_ROW_CODES
+    MICROSECONDS_PER_CODEWORD, BACKGROUND_COLOR_CODES,
+    MID_ROW_CODES, EXTENDED_CHARS, SPECIAL_CHARS
 )
 
 PopOnCue = collections.namedtuple("PopOnCue", "buffer, start, end")
 
 
 class PreCaption:
     """
@@ -284,14 +284,16 @@
         :return:
         """
         if not collection:
             self._collection = []
         else:
             self._collection = collection
 
+        self.last_style = None
+
         self._position_tracer = position_tracker
 
     def is_empty(self):
         """Whether any text was added to the buffer"""
         return not any(element.text for element in self._collection)
 
     def add_chars(self, *chars):
@@ -331,45 +333,68 @@
             )
             node = _InstructionNode.create_text(current_position)
             self._collection.append(node)
             self._position_tracer.acknowledge_position_changed()
 
         node.add_chars(*chars)
 
-    def interpret_command(self, command):
+    def interpret_command(self, command, previous_is_pac=None):
         """Given a command determines whether to turn italics on or off,
         or to set the positioning
 
         This is mostly used to convert from the legacy-style commands
 
         :type command: str
+        :type mode: pop or roll or paint
         """
         self._update_positioning(command)
 
         text = COMMANDS.get(command, '')
 
-        if command in MID_ROW_CODES:
-            for node in self._collection[::-1]:
-                if node.is_text_node():
-                    node.text += ' '
-                    break
+        if command == "94a1":
+            self.handle_backspace("94a1")
+
+        if command in BACKGROUND_COLOR_CODES:
+            # Since these codes are optional, they must be preceded
+            # with the space character (20h),
+            # which will be deleted when the code is applied.
+            # ex: 2080 97ad 94a1
+            if (
+                    self._collection[-1].is_text_node() and
+                    self._collection[-1].text[-1].isspace()
+            ):
+                self._collection[-1].text = self._collection[-1].text[:-1]
 
         if 'italic' in text:
             if 'end' not in text:
                 self._collection.append(
                     _InstructionNode.create_italics_style(
                         self._position_tracer.get_current_position())
                 )
+                self.last_style = "italics on"
             else:
                 self._collection.append(
                     _InstructionNode.create_italics_style(
                         self._position_tracer.get_current_position(),
                         turn_on=False
                     )
                 )
+                self.last_style = "italics off"
+
+        # mid row code that is not first code on the line
+        # (previous node is not a break node)
+        # fixes OCTO-11022
+        if command in MID_ROW_CODES and not previous_is_pac:
+            if self.last_style == "italics off":
+                self.add_chars(' ')
+            else:
+                for node in self._collection[::-1]:
+                    if node.is_text_node() and node.text:
+                        node.text += ' '
+                        break
 
     def _update_positioning(self, command):
         """Sets the positioning information to use for the next nodes
 
         :type command: str
         """
         if command in PAC_TAB_OFFSET_COMMANDS:
@@ -415,41 +440,40 @@
                 try:
                     instance._collection[-1].add_chars(' ')
                 except AttributeError:
                     pass
 
         return instance
 
-    def remove_ascii_duplicate(self, accented_character):
+    def handle_backspace(self, word):
         """
-        Characters from the Extended Characters list are usually preceded by
-        their ASCII substitute, in case the decoder is not able to display
-        the special character.
-
-        This is used to remove the substitute character in order to avoid
-        displaying both.
-
-        :type accented_character: str
+        Move cursor back one position and delete that character
         """
-        is_text_node = (
-                self._collection and
-                self._collection[-1].is_text_node() and
-                self._collection[-1].text
-                )
-        if is_text_node:
-            try:
-                ascii_char = [
-                    unicodedata.normalize('NFD', accented_character)
-                    .encode('ascii', 'strict').decode("utf-8")
-                ]
-            except (UnicodeEncodeError, UnicodeDecodeError):
-                ascii_char = INCONVERTIBLE_TO_ASCII_EXTENDED_CHARS_ASSOCIATION.get(accented_character)
-
-            if ascii_char and self._collection[-1].text[-1] in ascii_char:
-                self._collection[-1].text = self._collection[-1].text[:-1]
+        node = self.get_previous_text_node()
+        # in case of no previous text nodes or
+        # if the backspace is required while no character
+        # do nothing
+        if node is None:
+            return
+        last_char = node.text[-1]
+        delete_previous_condition = (
+            (word in SPECIAL_CHARS and last_char not in SPECIAL_CHARS.values()) or
+            (word in EXTENDED_CHARS and last_char not in EXTENDED_CHARS.values()) or
+            word == "94a1"
+        )
+        # in case of special / extended char, perform backspace
+        # only if the previous character in not also special / extended
+        if delete_previous_condition:
+            node.text = node.text[:-1]
+
+    def get_previous_text_node(self):
+        for node in self._collection[::-1]:
+            if node.is_text_node() and node.text:
+                return node
+        return None
 
 
 def _get_layout_from_tuple(position_tuple):
     """Create a Layout object from the positioning information given
 
     The row can have a value from 1 to 15 inclusive. (vertical positioning)
     The column can have a value from 0 to 31 inclusive. (horizontal)
```

### Comparing `pycaption-2.2.7/pycaption/scc/state_machines.py` & `pycaption-2.2.8/pycaption/scc/state_machines.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/scc/translator.py` & `pycaption-2.2.8/pycaption/scc/translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/srt.py` & `pycaption-2.2.8/pycaption/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/transcript.py` & `pycaption-2.2.8/pycaption/transcript.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption/webvtt.py` & `pycaption-2.2.8/pycaption/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/pycaption.egg-info/PKG-INFO` & `pycaption-2.2.8/pycaption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycaption
-Version: 2.2.7
+Version: 2.2.8
 Summary: Closed caption converter
 Author: Joe Norton
 Author-email: joey@nortoncrew.com
 Project-URL: Source, https://github.com/pbs/pycaption
 Project-URL: Documentation, https://pycaption.readthedocs.io/
 Project-URL: Release notes, https://pycaption.readthedocs.io/en/stable/changelog.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycaption-2.2.7/pycaption.egg-info/SOURCES.txt` & `pycaption-2.2.8/pycaption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/setup.py` & `pycaption-2.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 transcript_dependencies = [
     'nltk'
 ]
 
 setup(
     name='pycaption',
-    version='2.2.7',
+    version='2.2.8',
     description='Closed caption converter',
     long_description=open(README_PATH).read(),
     author='Joe Norton',
     author_email='joey@nortoncrew.com',
     project_urls={
         'Source': 'https://github.com/pbs/pycaption',
         'Documentation': 'https://pycaption.readthedocs.io/',
```

### Comparing `pycaption-2.2.7/tests/conftest.py` & `pycaption-2.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/fixtures/dfxp.py` & `pycaption-2.2.8/tests/fixtures/dfxp.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,18 +916,18 @@
    <region tts:displayAlign="before" tts:origin="40% 5%" tts:textAlign="left" xml:id="r1"/>
    <region tts:displayAlign="before" tts:origin="70% 23%" tts:textAlign="left" xml:id="r2"/>
    <region tts:displayAlign="before" tts:origin="20% 47%" tts:textAlign="left" xml:id="r3"/>
    <region tts:displayAlign="before" tts:origin="20% 89%" tts:textAlign="left" xml:id="r4"/>
    <region tts:displayAlign="before" tts:origin="40% 53%" tts:textAlign="left" xml:id="r5"/>
    <region tts:displayAlign="before" tts:origin="70% 17%" tts:textAlign="left" xml:id="r6"/>
    <region tts:displayAlign="before" tts:origin="20% 35%" tts:textAlign="left" xml:id="r7"/>
-   <region tts:displayAlign="before" tts:origin="20% 83%" tts:textAlign="left" xml:id="r8"/>
+   <region tts:displayAlign="before" tts:origin="25% 83%" tts:textAlign="left" xml:id="r8"/>
    <region tts:displayAlign="before" tts:origin="70% 11%" tts:textAlign="left" xml:id="r9"/>
    <region tts:displayAlign="before" tts:origin="40% 41%" tts:textAlign="left" xml:id="r10"/>
-   <region tts:displayAlign="before" tts:origin="20% 71%" tts:textAlign="left" xml:id="r11"/>
+   <region tts:displayAlign="before" tts:origin="25% 71%" tts:textAlign="left" xml:id="r11"/>
   </layout>
  </head>
  <body>
   <div region="bottom" xml:lang="en-US">
    <p begin="00:00:01.134" end="00:00:03.136" region="r0" style="default">
     abab
    </p>
```

### Comparing `pycaption-2.2.7/tests/fixtures/microdvd.py` & `pycaption-2.2.8/tests/fixtures/microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/fixtures/sami.py` & `pycaption-2.2.8/tests/fixtures/sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/fixtures/scc.py` & `pycaption-2.2.8/tests/fixtures/scc.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,17 +363,19 @@
 
 
 @pytest.fixture(scope="session")
 def sample_scc_duplicate_special_characters():
     return """\
 Scenarist_SCC V1.0
 
-00:23:28;01 9420 91b0 91b0 9131 9131 9132 9132 91b3 91b3 9134 9134 91b5 91b5 91b6 91b6 9137 9137 9138 9138 91b9 91b9 91ba 91ba 913b 913b 91bc 91bc 913d 913d 913e 913e 91bf 91bf 942f
+00:23:28;01 9420 9420 91b0 91b0 9131 9131 9132 9132 91b3 91b3 9134 9134 91b5 91b5 91b6 91b6 9137 9137 9138 9138 91b9 91b9 91ba 91ba 913b 913b 91bc 91bc 913d 913d 913e 913e 91bf 91bf 942f
 
-00:53:28;01 9420 91b0 9131 9132 91b3 9134 91b5 91b6 9137 9138 91b9 91ba 913b 91bc 913d 913e 91bf 942f
+00:33:28;01 9420 91b0 9131 9132 91b3 9134 91b5 91b6 9137 9138 91b9 91ba 913b 91bc 913d 913e 91bf 942f
+
+00:53:28;01 9420 91b0 9131 c1c1 9132 91b3 9134 91b5 91b6 9137 9138 91b9 91ba 913b 91bc c1c1 913d 913e 91bf 942f
 
 """
 
 
 @pytest.fixture(scope="session")
 def sample_scc_tab_offset():
     return """\
```

### Comparing `pycaption-2.2.7/tests/fixtures/srt.py` & `pycaption-2.2.8/tests/fixtures/srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/fixtures/translated_scc.py` & `pycaption-2.2.8/tests/fixtures/translated_scc.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/fixtures/webvtt.py` & `pycaption-2.2.8/tests/fixtures/webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/mixins.py` & `pycaption-2.2.8/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_base.py` & `pycaption-2.2.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_dfxp.py` & `pycaption-2.2.8/tests/test_dfxp.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_dfxp_conversion.py` & `pycaption-2.2.8/tests/test_dfxp_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_dfxp_extras.py` & `pycaption-2.2.8/tests/test_dfxp_extras.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_functions.py` & `pycaption-2.2.8/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_geometry.py` & `pycaption-2.2.8/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_microdvd.py` & `pycaption-2.2.8/tests/test_microdvd.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_microdvd_conversion.py` & `pycaption-2.2.8/tests/test_microdvd_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_sami.py` & `pycaption-2.2.8/tests/test_sami.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_sami_conversion.py` & `pycaption-2.2.8/tests/test_sami_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_scc.py` & `pycaption-2.2.8/tests/test_scc.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,25 +73,23 @@
             ((40.0, UnitEnum.PERCENT), (5.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (23.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (47.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (89.0, UnitEnum.PERCENT)),
             ((40.0, UnitEnum.PERCENT), (53.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (17.0, UnitEnum.PERCENT)),
             ((20.0, UnitEnum.PERCENT), (35.0, UnitEnum.PERCENT)),
-            ((20.0, UnitEnum.PERCENT), (83.0, UnitEnum.PERCENT)),
+            ((25.0, UnitEnum.PERCENT), (83.0, UnitEnum.PERCENT)),
             ((70.0, UnitEnum.PERCENT), (11.0, UnitEnum.PERCENT)),
             ((40.0, UnitEnum.PERCENT), (41.0, UnitEnum.PERCENT)),
-            ((20.0, UnitEnum.PERCENT), (71.0, UnitEnum.PERCENT))
+            ((25.0, UnitEnum.PERCENT), (71.0, UnitEnum.PERCENT))
         ]
-
         actual_positioning = [
             caption_.layout_info.origin.serialized()
             for caption_ in captions.get_captions('en-US')
         ]
-
         assert expected_positioning == actual_positioning
 
     def test_tab_offset(self, sample_scc_tab_offset):
         captions = SCCReader().read(sample_scc_tab_offset)
 
         # SCC generates only origin, and we always expect it.
         expected_positioning = [
@@ -206,39 +204,42 @@
 
     def test_skip_duplicate_tab_offset(self, sample_scc_duplicate_tab_offset):
         expected_lines = [
             '[Radio reporter] ',
             'The I-10 Santa Monica Freeway ',
             'westbound is jammed,',
             'due to a three-car accident ',
-            'blocking lanes 1 and 2',
+            'blocking lanes 1 and 2'
         ]
 
         caption_set = SCCReader().read(sample_scc_duplicate_tab_offset)
         actual_lines = [
             node.content
             for cap_ in caption_set.get_captions('en-US')
             for node in cap_.nodes
             if node.type_ == CaptionNode.TEXT
         ]
 
         assert expected_lines == actual_lines
 
     def test_skip_duplicate_special_characters(
             self, sample_scc_duplicate_special_characters):
-        expected_lines = ['®°½¿™¢£♪à èâêîôû', '®°½¿™¢£♪à èâêîôû']
+        expected_lines = [
+            '®°½¿™¢£♪à èâêîôû',   # double commands so we skip one
+            '®°½¿™¢£♪à èâêîôû',   # no double command, nothing skipped equal with above
+            '®°A½¿™¢£♪à èâêAîôû'  # no skips but a couple of normal chars "c1c1" = AA
+        ]
 
         caption_set = SCCReader().read(sample_scc_duplicate_special_characters)
         actual_lines = [
             node.content
             for cap_ in caption_set.get_captions('en-US')
             for node in cap_.nodes
             if node.type_ == CaptionNode.TEXT
         ]
-
         assert expected_lines == actual_lines
 
     def test_flashing_cue(self, sample_scc_flashing_cue):
         with pytest.raises(CaptionReadTimingError) as exc_info:
             SCCReader().read(sample_scc_flashing_cue)
 
         assert exc_info.value.args[0].startswith(
@@ -269,29 +270,29 @@
         # There were no tests for ROLL-UP captions, but the library processed
         # Roll-Up captions. Make sure nothing changes during the refactoring
         scc1 = SCCReader().read(sample_scc_roll_up_ru2)
         captions = scc1.get_captions('en-US')
         actual_texts = [cap_.nodes[0].content for cap_ in captions]
         expected_texts = [
             '>>> HI.',
-            "I'M KEVIN CUNNING AND AT",
-            "INVESTOR'S BANK WE BELIEVE IN",
-            'HELPING THE LOCAL NEIGHBORHOODS',
-            'AND IMPROVING THE LIVES OF ALL',
-            'WE SERVE.',
-            '®°½',
-            'ABû',
-            'ÁÉÓ¡',
-            "WHERE YOU'RE STANDING NOW,",
-            "LOOKING OUT THERE, THAT'S AL",
-            'THE CROWD.',
-            '>> IT WAS GOOD TO BE IN TH',
-            "And restore Iowa's land, water",
-            'And wildlife.',
-            '>> Bike Iowa, your source for',
+             "I'M KEVIN CUNNING AND AT",
+             "INVESTOR'S BANK WE BELIEVE IN",
+             'HELPING THE LOCAL NEIGHBORHOODS',
+             'AND IMPROVING THE LIVES OF ALL',
+             'WE SERVE.',
+             '®°½',
+             'Aû',
+             'ÁÉÓ¡',
+             "WHERE YOU'RE STANDING NOW,",
+             "LOOKING OUT THERE, THAT'S AL",
+             'THE CROWD.',
+             '>> IT WAS GOOD TO BE IN TH',
+             "And restore Iowa's land, water",
+             'And wildlife.',
+             '>> Bike Iowa, your source for'
         ]
         assert expected_texts == actual_texts
 
     def test_multiple_formats(self, sample_scc_multiple_formats):
         # Test for captions that contain both pop on and paint on formats to
         # ensure the paint on lines are not repeated
         expected_text_lines = [
@@ -379,14 +380,17 @@
         # We expect
         # 1. all the initial italics closing nodes to be removed
         # 2. all the redundant italic nodes to be trimmed
         # 3. to get new closing italic nodes before changing position,
         # 4. to get new opening italic nodes after changing position, if 3
         # happened
         # 5. to get a final italic closing node, if one is needed
+        # 9120 and 91ae are mid row codes and will add a space
+        # 9120 at the start of the following text node
+        # 91ae to the end of the previous text node
         node_creator.interpret_command('9470')  # row 15, col 0
         node_creator.interpret_command('9120')  # italics off
         node_creator.interpret_command('9120')  # italics off
         node_creator.add_chars('a')
 
         node_creator.interpret_command('9770')  # row 10 col 0
         node_creator.interpret_command('91ae')  # italics ON
@@ -397,15 +401,15 @@
         node_creator.interpret_command('9120')  # italics OFF
         node_creator.interpret_command('91ae')  # italics ON
         node_creator.interpret_command('91ae')  # italics ON
         node_creator.interpret_command('91ae')  # italics ON
         node_creator.add_chars('b')
         node_creator.interpret_command('91ae')  # italics ON again
         node_creator.add_chars('b')
-        node_creator.interpret_command('9120')  # italics OFF
+        node_creator.interpret_command('9120')  # italics OFF adds space
         node_creator.interpret_command('9120')  # italics OFF
 
         node_creator.interpret_command('1570')  # row 6 col 0
         node_creator.add_chars('c')
         node_creator.interpret_command('91ae')  # italics ON
 
         node_creator.interpret_command('9270')  # row 4 col 0
@@ -416,40 +420,43 @@
 
         node_creator.interpret_command('1570')  # row 6 col 0 - creates BR
         node_creator.add_chars('f')
 
         result = list(node_creator)
 
         assert result[0].is_text_node()
-        assert result[1].requires_repositioning()
-        assert result[2].is_italics_node()
-        assert result[2].sets_italics_on()
+        assert result[1].is_text_node()
+        assert result[2].requires_repositioning()
 
-        assert result[3].is_text_node()
+        assert result[3].is_italics_node()
+        assert result[3].sets_italics_on()
         assert result[4].is_text_node()
-        assert result[5].is_text_node()
-
-        assert result[6].is_italics_node()
-        assert result[6].sets_italics_off()
+        assert result[5].sets_italics_off()
+        assert result[6].is_text_node()
 
-        assert result[7].requires_repositioning()
-        assert result[8].is_text_node()
+        assert result[7].is_text_node()
+        assert result[8].sets_italics_on()
 
-        assert result[9].requires_repositioning()
-        assert result[10].is_italics_node()
-        assert result[10].sets_italics_on()
+        assert result[9].is_text_node()
+        assert result[10].is_text_node()
 
-        assert result[11].is_text_node()
-        assert result[12].is_explicit_break()
+        assert result[11].sets_italics_off()
+        assert result[12].is_text_node()
         assert result[13].is_text_node()
-        assert result[14].is_explicit_break()
+        assert result[14].requires_repositioning()
         assert result[15].is_text_node()
 
-        assert result[16].is_italics_node()
-        assert result[16].sets_italics_off()
+        assert result[16].requires_repositioning()
+        assert result[17].sets_italics_on()
+        assert result[18].is_text_node()
+        assert result[19].is_explicit_break()
+        assert result[20].is_text_node()
+        assert result[21].is_explicit_break()
+        assert result[22].is_text_node()
+        assert result[23].sets_italics_off()
 
 
 class CaptionDummy:
     """Mock for pycaption.base.Caption"""
 
     def __init__(self, start=0, end=0, nodes=(1, 2)):
         self.nodes = nodes
```

### Comparing `pycaption-2.2.7/tests/test_scc_conversion.py` & `pycaption-2.2.8/tests/test_scc_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_scc_translator.py` & `pycaption-2.2.8/tests/test_scc_translator.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_srt.py` & `pycaption-2.2.8/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_srt_conversion.py` & `pycaption-2.2.8/tests/test_srt_conversion.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_webvtt.py` & `pycaption-2.2.8/tests/test_webvtt.py`

 * *Files identical despite different names*

### Comparing `pycaption-2.2.7/tests/test_webvtt_conversion.py` & `pycaption-2.2.8/tests/test_webvtt_conversion.py`

 * *Files identical despite different names*

