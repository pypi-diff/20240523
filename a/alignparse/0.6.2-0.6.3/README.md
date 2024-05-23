# Comparing `tmp/alignparse-0.6.2.tar.gz` & `tmp/alignparse-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alignparse-0.6.2.tar", last modified: Mon Jun 19 12:18:41 2023, max compression
+gzip compressed data, was "alignparse-0.6.3.tar", last modified: Thu May 23 18:37:35 2024, max compression
```

## Comparing `alignparse-0.6.2.tar` & `alignparse-0.6.3.tar`

### file list

```diff
@@ -1,81 +1,78 @@
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.512861 alignparse-0.6.2/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      192 2022-03-04 14:28:16.000000 alignparse-0.6.2/.flake8
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      155 2019-11-16 23:28:43.000000 alignparse-0.6.2/.gitignore
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      508 2023-06-19 10:35:29.000000 alignparse-0.6.2/.travis.yml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2273 2023-06-19 12:14:36.000000 alignparse-0.6.2/CHANGELOG.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7325 2022-03-04 14:28:16.000000 alignparse-0.6.2/CONTRIBUTING.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1601 2019-11-16 23:28:43.000000 alignparse-0.6.2/LICENSE.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2126 2023-06-19 12:18:41.511388 alignparse-0.6.2/PKG-INFO
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1728 2023-05-25 22:21:02.000000 alignparse-0.6.2/README.rst
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.152390 alignparse-0.6.2/alignparse/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      271 2023-06-19 12:14:36.000000 alignparse-0.6.2/alignparse/__init__.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    36505 2022-09-07 20:52:33.000000 alignparse-0.6.2/alignparse/ccs.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    27849 2023-05-26 04:32:42.000000 alignparse-0.6.2/alignparse/consensus.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      332 2022-03-04 14:28:16.000000 alignparse-0.6.2/alignparse/constants.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    23229 2023-05-26 04:32:42.000000 alignparse-0.6.2/alignparse/cs_tag.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    12323 2022-03-04 14:28:16.000000 alignparse-0.6.2/alignparse/minimap2.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    57158 2023-05-26 04:32:42.000000 alignparse-0.6.2/alignparse/targets.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    18494 2022-06-04 18:24:44.000000 alignparse-0.6.2/alignparse/utils.py
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.173983 alignparse-0.6.2/alignparse.egg-info/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2126 2023-06-19 12:18:40.000000 alignparse-0.6.2/alignparse.egg-info/PKG-INFO
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1937 2023-06-19 12:18:40.000000 alignparse-0.6.2/alignparse.egg-info/SOURCES.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)        1 2023-06-19 12:18:40.000000 alignparse-0.6.2/alignparse.egg-info/dependency_links.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      177 2023-06-19 12:18:40.000000 alignparse-0.6.2/alignparse.egg-info/requires.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       11 2023-06-19 12:18:40.000000 alignparse-0.6.2/alignparse.egg-info/top_level.txt
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.230288 alignparse-0.6.2/docs/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)        0 2019-11-16 23:31:36.000000 alignparse-0.6.2/docs/.nojekyll
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      725 2019-11-16 23:31:36.000000 alignparse-0.6.2/docs/Makefile
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3647 2019-11-17 02:01:22.000000 alignparse-0.6.2/docs/README.rst
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.235790 alignparse-0.6.2/docs/_static/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   172664 2019-11-16 23:31:36.000000 alignparse-0.6.2/docs/_static/BloomLogo.jpg
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      907 2020-04-10 21:49:57.000000 alignparse-0.6.2/docs/acknowledgements.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6743 2022-03-04 14:28:16.000000 alignparse-0.6.2/docs/conf.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      143 2023-06-19 12:18:35.000000 alignparse-0.6.2/docs/doc_requirements.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1205 2019-12-21 14:40:48.000000 alignparse-0.6.2/docs/examples.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2019-11-16 23:31:36.000000 alignparse-0.6.2/docs/flu_virus_seq_example.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1399 2020-04-10 21:49:57.000000 alignparse-0.6.2/docs/index.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1380 2023-06-19 12:14:36.000000 alignparse-0.6.2/docs/installation.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       48 2019-11-17 02:01:22.000000 alignparse-0.6.2/docs/lasv_pilot.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       65 2019-12-21 14:40:48.000000 alignparse-0.6.2/docs/package_index.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       46 2019-11-16 23:31:36.000000 alignparse-0.6.2/docs/recA_DMS.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      324 2023-06-19 12:14:36.000000 alignparse-0.6.2/environment.yml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      431 2019-11-16 23:28:43.000000 alignparse-0.6.2/nbval_sanitize.cfg
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.261630 alignparse-0.6.2/notebooks/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      259 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   446725 2023-06-19 12:14:36.000000 alignparse-0.6.2/notebooks/flu_virus_seq_example.ipynb
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.384170 alignparse-0.6.2/notebooks/input_files/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3361 2019-12-06 13:24:51.000000 alignparse-0.6.2/notebooks/input_files/LASV_Josiah_OPT.gb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3356 2019-12-06 13:24:51.000000 alignparse-0.6.2/notebooks/input_files/LASV_Josiah_WT.gb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2240 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    24548 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/flu_WSN_amplicons.gb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)  1065361 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/flu_WSN_ccs.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1536 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/flu_WSN_feature_parse_specs.yaml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    67258 2019-12-06 13:24:51.000000 alignparse-0.6.2/notebooks/input_files/lasv_example_ccs.fastq.gz
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      609 2019-11-17 02:01:22.000000 alignparse-0.6.2/notebooks/input_files/lasv_feature_parse_specs.yaml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      806 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/lasv_pilot_report.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2690 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_amplicon.gb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      557 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_feature_parse_specs.yaml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   383728 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_lib-1_ccs.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      588 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_lib-1_report.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   339602 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_lib-2_ccs.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      588 2019-11-16 23:28:43.000000 alignparse-0.6.2/notebooks/input_files/recA_lib-2_report.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   153351 2023-06-19 12:14:36.000000 alignparse-0.6.2/notebooks/lasv_pilot.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   130579 2023-06-19 12:14:36.000000 alignparse-0.6.2/notebooks/recA_DMS.ipynb
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.419983 alignparse-0.6.2/paper/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      424 2019-12-06 13:24:51.000000 alignparse-0.6.2/paper/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3128 2019-12-06 13:24:51.000000 alignparse-0.6.2/paper/paper.bib
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     9274 2019-12-06 13:24:51.000000 alignparse-0.6.2/paper/paper.md
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      194 2022-03-04 14:28:16.000000 alignparse-0.6.2/pytest.ini
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       38 2023-06-19 12:18:41.514065 alignparse-0.6.2/setup.cfg
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1783 2023-06-19 12:14:36.000000 alignparse-0.6.2/setup.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      244 2023-06-19 10:37:21.000000 alignparse-0.6.2/test_requirements.txt
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2023-06-19 12:18:41.488821 alignparse-0.6.2/tests/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      117 2019-11-16 23:28:43.000000 alignparse-0.6.2/tests/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    29231 2023-06-19 12:14:36.000000 alignparse-0.6.2/tests/check_Targets_align_and_parse.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7951 2022-03-04 14:28:16.000000 alignparse-0.6.2/tests/profile_recA.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    89729 2022-03-04 14:28:16.000000 alignparse-0.6.2/tests/test_Targets_objects.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    66513 2023-06-19 12:14:36.000000 alignparse-0.6.2/tests/test_Targets_parse_alignment.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     8037 2022-03-04 14:28:16.000000 alignparse-0.6.2/tests/test_Targets_parse_alignment_consistency.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   120341 2023-05-26 04:32:42.000000 alignparse-0.6.2/tests/test_ccs_summaries.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    14426 2022-03-04 14:28:16.000000 alignparse-0.6.2/tests/test_cs_tag_Alignment.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    10259 2022-03-04 14:28:16.000000 alignparse-0.6.2/tests/test_cs_tag_Alignment_accuracy.ipynb
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.951467 alignparse-0.6.3/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      164 2024-05-23 18:36:54.000000 alignparse-0.6.3/.gitignore
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2926 2024-05-23 18:36:54.000000 alignparse-0.6.3/CHANGELOG.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     5962 2024-05-23 18:36:54.000000 alignparse-0.6.3/CONTRIBUTING.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1601 2019-11-16 23:28:43.000000 alignparse-0.6.3/LICENSE.txt
+-rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     2658 2024-05-23 18:37:35.947629 alignparse-0.6.3/PKG-INFO
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1901 2024-05-23 18:36:54.000000 alignparse-0.6.3/README.rst
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.649329 alignparse-0.6.3/alignparse/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      271 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/__init__.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    36504 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/ccs.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    27953 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/consensus.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      331 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/constants.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    23228 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/cs_tag.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    12324 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/minimap2.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    57166 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/targets.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    18493 2024-05-23 18:36:54.000000 alignparse-0.6.3/alignparse/utils.py
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.941732 alignparse-0.6.3/alignparse.egg-info/
+-rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     2658 2024-05-23 18:37:35.000000 alignparse-0.6.3/alignparse.egg-info/PKG-INFO
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1901 2024-05-23 18:37:35.000000 alignparse-0.6.3/alignparse.egg-info/SOURCES.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)        1 2024-05-23 18:37:35.000000 alignparse-0.6.3/alignparse.egg-info/dependency_links.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      179 2024-05-23 18:37:35.000000 alignparse-0.6.3/alignparse.egg-info/requires.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       11 2024-05-23 18:37:35.000000 alignparse-0.6.3/alignparse.egg-info/top_level.txt
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.716010 alignparse-0.6.3/docs/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)        0 2019-11-16 23:31:36.000000 alignparse-0.6.3/docs/.nojekyll
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      725 2019-11-16 23:31:36.000000 alignparse-0.6.3/docs/Makefile
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3647 2019-11-17 02:01:22.000000 alignparse-0.6.3/docs/README.rst
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.720460 alignparse-0.6.3/docs/_static/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   172664 2019-11-16 23:31:36.000000 alignparse-0.6.3/docs/_static/BloomLogo.jpg
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      907 2020-04-10 21:49:57.000000 alignparse-0.6.3/docs/acknowledgements.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6716 2024-05-23 18:36:54.000000 alignparse-0.6.3/docs/conf.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      143 2023-06-19 12:18:35.000000 alignparse-0.6.3/docs/doc_requirements.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      899 2024-05-23 18:36:54.000000 alignparse-0.6.3/docs/examples.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2019-11-16 23:31:36.000000 alignparse-0.6.3/docs/flu_virus_seq_example.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1399 2020-04-10 21:49:57.000000 alignparse-0.6.3/docs/index.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1381 2024-05-23 18:36:54.000000 alignparse-0.6.3/docs/installation.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       48 2019-11-17 02:01:22.000000 alignparse-0.6.3/docs/lasv_pilot.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       65 2019-12-21 14:40:48.000000 alignparse-0.6.3/docs/package_index.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       46 2019-11-16 23:31:36.000000 alignparse-0.6.3/docs/recA_DMS.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      431 2019-11-16 23:28:43.000000 alignparse-0.6.3/nbval_sanitize.cfg
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.815496 alignparse-0.6.3/notebooks/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      259 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    13778 2024-05-23 18:36:54.000000 alignparse-0.6.3/notebooks/flu_virus_seq_example.ipynb
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.893147 alignparse-0.6.3/notebooks/input_files/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3361 2019-12-06 13:24:51.000000 alignparse-0.6.3/notebooks/input_files/LASV_Josiah_OPT.gb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3356 2019-12-06 13:24:51.000000 alignparse-0.6.3/notebooks/input_files/LASV_Josiah_WT.gb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2240 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    24548 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/flu_WSN_amplicons.gb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)  1065361 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/flu_WSN_ccs.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1536 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/flu_WSN_feature_parse_specs.yaml
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    67258 2019-12-06 13:24:51.000000 alignparse-0.6.3/notebooks/input_files/lasv_example_ccs.fastq.gz
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      609 2019-11-17 02:01:22.000000 alignparse-0.6.3/notebooks/input_files/lasv_feature_parse_specs.yaml
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      806 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/lasv_pilot_report.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2690 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_amplicon.gb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      557 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_feature_parse_specs.yaml
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   383728 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_lib-1_ccs.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      588 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_lib-1_report.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   339602 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_lib-2_ccs.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      588 2019-11-16 23:28:43.000000 alignparse-0.6.3/notebooks/input_files/recA_lib-2_report.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   153393 2024-05-23 18:36:54.000000 alignparse-0.6.3/notebooks/lasv_pilot.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   130621 2024-05-23 18:36:54.000000 alignparse-0.6.3/notebooks/recA_DMS.ipynb
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.903481 alignparse-0.6.3/paper/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      424 2019-12-06 13:24:51.000000 alignparse-0.6.3/paper/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3128 2019-12-06 13:24:51.000000 alignparse-0.6.3/paper/paper.bib
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     9274 2019-12-06 13:24:51.000000 alignparse-0.6.3/paper/paper.md
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      200 2024-05-23 18:36:54.000000 alignparse-0.6.3/pytest.ini
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       38 2024-05-23 18:37:35.952591 alignparse-0.6.3/setup.cfg
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1784 2024-05-23 18:36:54.000000 alignparse-0.6.3/setup.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       46 2024-05-23 18:36:54.000000 alignparse-0.6.3/test_requirements.txt
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-05-23 18:37:35.937187 alignparse-0.6.3/tests/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      117 2019-11-16 23:28:43.000000 alignparse-0.6.3/tests/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    29231 2024-05-23 18:36:54.000000 alignparse-0.6.3/tests/check_Targets_align_and_parse.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7951 2022-03-04 14:28:16.000000 alignparse-0.6.3/tests/profile_recA.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    89729 2022-03-04 14:28:16.000000 alignparse-0.6.3/tests/test_Targets_objects.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    66513 2024-05-23 18:36:54.000000 alignparse-0.6.3/tests/test_Targets_parse_alignment.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     8037 2022-03-04 14:28:16.000000 alignparse-0.6.3/tests/test_Targets_parse_alignment_consistency.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    19325 2024-05-23 18:36:54.000000 alignparse-0.6.3/tests/test_ccs_summaries.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    14426 2022-03-04 14:28:16.000000 alignparse-0.6.3/tests/test_cs_tag_Alignment.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    10259 2022-03-04 14:28:16.000000 alignparse-0.6.3/tests/test_cs_tag_Alignment_accuracy.ipynb
```

### Comparing `alignparse-0.6.2/CHANGELOG.rst` & `alignparse-0.6.3/CHANGELOG.rst`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com>`_.
 
+0.6.3
+-----
+
+Fixed
++++++
+* Fix bug in handling ``minimap2`` errors ([see this issue](https://github.com/jbloomlab/alignparse/issues/99))
+* Pass formatting with new ``black`` version
+* Pass tests with new ``pandas`` version.
+* Fixed ``simple_mut_consensus`` for newer versions of ``pandas`` when goruping by just one variable.
+
+Changed
++++++++
+* Change code linting to ``ruff`` rather than ``flake8``.
+* Test with GitHub Actions rather than Travis CI.
+* Remove ``mybinder`` examples.
+* Test on Python 3.11 rather than 3.9.
+* Don't allow ``pysam`` version 0.22.1 as it was causing some type of OPENSSL import error.
+* Test with ``minimap2`` version 2.22
+
 0.6.2
 -----
 
 Fixed
 +++++
 * Require python 3.8 or greater.
```

### Comparing `alignparse-0.6.2/CONTRIBUTING.rst` & `alignparse-0.6.3/CONTRIBUTING.rst`

 * *Files 19% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 Note also that the `Jupyter notebooks`_ in notebooks_ are tested via nbval_.
 If you are getting errors on these notebook tests due to testing cells that output objects that can't be properly tested (such as widgets), see the *nbval-ignore-output* tag option discussed in the nbval_ docs.
 
 Formatting
 ++++++++++
 The code is formatted using `Black <https://black.readthedocs.io/en/stable/index.html>`_, which you can install using `pip install "black[jupyter]"`.
 You may also wish to install a Black extension in your editor to, for example, auto-format upon save.
-In any case, please run Black using `black .` before submitting your PR, because the Travis tests will not pass unless the files have been formatted.
+In any case, please run Black using `black .` before submitting your PR, because the tests will not pass unless the files have been formatted.
 Note that this will change files/notebooks that you may be actively editing.
 
 Versions and CHANGELOG
 ++++++++++++++++++++++
 The version is `single sourced <https://packaging.python.org/guides/single-sourcing-package-version/>`_ in `__init__.py`_.
 When modifying a tagged version (e.g., ``0.1.0``), indicate you are working on a development version by adding a ``dev`` (e.g., ``0.1.dev1``).
 See `here <https://www.python.org/dev/peps/pep-0440/>`_ for more information on version numbers.
@@ -53,23 +53,14 @@
 
 Adding dependencies
 +++++++++++++++++++++
 When you add code that uses a new package that is not in the standard python library, you should add it to the dependencies specified under the `install_requires` option in `setup.py <setup.py>`_.
 `See here <https://packaging.python.org/discussions/install-requires-vs-requirements/>`_ for information on how to do this, and how to specify minimal required versions.
 As described in the above link, you should **not** pin exact versions in `install_requires` in `setup.py <setup.py>`_ unless absolutely necessary.
 
-Notebooks on mybinder
------------------------
-The `Jupyter notebooks`_ in notebooks_ can be run interactively on mybinder_ by going to the following link:
-https://mybinder.org/v2/gh/jbloomlab/alignparse/master?filepath=notebooks
-
-In order for this to work, you need to keep the `environment.yml <environment.yml>`_ configuration file up to date with the dependencies for running these notebooks as `described here <https://mybinder.readthedocs.io/en/latest/config_files.html>`_.
-Note that unlike for the `install_requires` in `setup.py <setup.py>`_, you may want to pin exact versions here to get reproducible installations.
-Look into the `pip freeze <https://pip.pypa.io/en/stable/reference/pip_freeze/>`_ and `conda env export <https://packaging.python.org/discussions/install-requires-vs-requirements>`_ commands on how to automatically create such a configuration file.
-
 Testing
 ---------
 
 Adding tests
 ++++++++++++++
 As you add new codes, you should create tests to make sure it is working correctly.
 These can include:
@@ -83,37 +74,29 @@
 After you make changes, you should run two sets of tests.
 To run the tests, go to the top-level package directory.
 Then make sure that you have installed the packages listed in `test_requirements.txt <test_requirements.txt>`_.
 If these are not installed, install them with::
 
     pip install -r test_requirements.txt
 
-Then use flake8_ to `lint the code <https://en.wikipedia.org/wiki/Lint_%28software%29>`_ by running::
+Then use ruff_ to `lint the code <https://en.wikipedia.org/wiki/Lint_%28software%29>`_ by running::
 
-    flake8
+    ruff check .
 
-If you need to change the flake8_ configuration, edit the `.flake8 <.flake8>`_ file.
+If you need to change the ruff_ configuration, edit the `ruff.toml <ruff.toml>`_ file.
 
 Then run the tests with pytest_ by running::
 
     pytest
 
 If you need to change the pytest_ configuration, edit the `pytest.ini <pytest.ini>`_ file.
 
-Automated testing on Travis
-+++++++++++++++++++++++++++
-The aforementioned flake8_ and pytest_ tests will be run automatically by the Travis_ continuous integration system as specified in the `.travis.yml <.travis.yml>`_ file.
-Note that running the Travis_ tests requires you to register the project with Travis_.
-
-If the tests are passing, you will see this on the Travis_ badge on GitHub repo main page.
-
-Slack notifications of test results
+Automated testing with GitHub Actions
 +++++++++++++++++++++++++++++++++++++
-You can configure Travis_ to provide automatic Slack notifications of the test results.
-To do that, follow the `instructions here <https://docs.travis-ci.com/user/notifications/#configuring-slack-notifications>`_.
+The aforementioned ruff_ and pytest_ tests will be run automatically by GitHub Actions using the test in [.github/workflows/test.yml](.github/workflows/test.yml).
 
 
 Building documentation
 ------------------------
 See `docs/README.rst <docs/README.rst>`_ for information on how to build the documentation.
 
 Tagging versions and putting on PyPI
@@ -129,16 +112,15 @@
 
     git push --tags
 
 Finally, upload to PyPI_ with twine_ as `described here <https://github.com/pypa/twine>`_.
 Note that this requires you to have registered the package on PyPI_ if this is the first version of the package there.
 
 .. _pytest: https://docs.pytest.org
-.. _flake8: http://flake8.pycqa.org
-.. _Travis: https://docs.travis-ci.com
+.. _ruff: https://github.com/astral-sh/ruff
 .. _PyPI: https://pypi.org/
 .. _pip: https://pip.pypa.io
 .. _sphinx: https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html
 .. _tests: tests
 .. _docs: docs
 .. _notebooks: notebooks
 .. _`Jupyter notebooks`: https://jupyter.org/
```

### Comparing `alignparse-0.6.2/LICENSE.txt` & `alignparse-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/PKG-INFO` & `alignparse-0.6.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-Metadata-Version: 2.1
-Name: alignparse
-Version: 0.6.2
-Summary: Align sequences and then parse features.
-Home-page: https://github.com/jbloomlab/alignparse
-Download-URL: https://github.com/jbloomlab/alignparse/tarball/0.6.2
-Author: `the Bloom lab <https://research.fhcrc.org/bloom/en.html>`_
-Author-email: jbloom@fredhutch.org
-License: GPLv3
-Platform: Linux and Mac OS X.
-License-File: LICENSE.txt
-
 ===============================
 alignparse
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/alignparse.svg
         :target: https://pypi.python.org/pypi/alignparse
 
-.. image:: https://app.travis-ci.com/jbloomlab/alignparse.svg?branch=master
-        :target: https://app.travis-ci.com/github/jbloomlab/alignparse
-
-.. image:: https://mybinder.org/badge_logo.svg
-        :target: https://mybinder.org/v2/gh/jbloomlab/alignparse/master?filepath=notebooks
+.. image:: https://github.com/jbloomlab/alignparse/actions/workflows/test.yml/badge.svg
+        :target: https://github.com/jbloomlab/alignparse/actions/workflows/test.yml
 
 .. image:: https://zenodo.org/badge/194140958.svg
    :target: https://zenodo.org/badge/latestdoi/194140958
 
 .. image:: https://joss.theoj.org/papers/10.21105/joss.01915/status.svg
    :target: https://doi.org/10.21105/joss.01915
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+
 ``alignparse`` is a Python package written by `the Bloom lab <https://research.fhcrc.org/bloom/en.html>`_. 
 It is designed to align long sequencing reads (such as those from PacBio circular consensus sequencing) to targets, filter these alignments based on user-provided specifications, and parse out user-defined sequence features.
 For each read that passes the filters, information about the features (e.g. accuracy, sequence, mutations) is retained for further analyses. 
 
 See the `alignparse documentation <https://jbloomlab.github.io/alignparse>`_ for details on how to install and use ``alignparse``.
 
 Please `cite alignparse <https://jbloomlab.github.io/alignparse/acknowledgements.html>`_ if you use it in your work.
```

### Comparing `alignparse-0.6.2/alignparse/ccs.py` & `alignparse-0.6.3/alignparse/ccs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 ===
 
 Tools for inspecting output of the PacBio ``ccs`` program:
 https://github.com/PacificBiosciences/unanimity/blob/develop/doc/PBCCS.md
 
 """
 
-
 import collections
 import io
 import itertools
 import math
 import os
 import re
 import tempfile  # noqa: F401
@@ -71,27 +70,27 @@
     """
 
     def __init__(self, name, fastqfile, reportfile):
         """See main class docstring."""
         self.name = name
         self.fastqfile = fastqfile
         if not os.path.isfile(fastqfile):
-            raise IOError(f"cannot find `fastqfile` {fastqfile}")
+            raise OSError(f"cannot find `fastqfile` {fastqfile}")
 
         ccs_stats = get_ccs_stats(self.fastqfile)
         self.passes = ccs_stats.passes
         self.accuracy = ccs_stats.accuracy
         self.length = ccs_stats.length
         assert len(self.accuracy) == len(self.length)
         assert (self.passes is None) or (len(self.passes) == len(self.length))
 
         if reportfile:
             self.reportfile = reportfile
             if not os.path.isfile(reportfile):
-                raise IOError(f"cannot find `reportfile` {reportfile}")
+                raise OSError(f"cannot find `reportfile` {reportfile}")
             self.zmw_stats = report_to_stats(self.reportfile)
             zmw_stats_nccs = self.zmw_stats[
                 self.zmw_stats["status"].str.match("^Success")
             ]["number"].sum()
             if len(self.length) != zmw_stats_nccs:
                 raise ValueError(
                     "`fastqfile`, `reportfile` differ on number "
@@ -668,15 +667,15 @@
         _report_to_stats_v4,
         _report_to_stats_v3,
     ]:
         df = func(reportfile)
         if df is not None:
             return df
 
-    raise IOError(f"Cannot match report in {reportfile}")
+    raise OSError(f"Cannot match report in {reportfile}")
 
 
 def _reportfile_version_check(reportfile, pattern):
     """
     Check reportfile against known version specific patterns
 
     Parameters
```

### Comparing `alignparse-0.6.2/alignparse/consensus.py` & `alignparse-0.6.3/alignparse/consensus.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 =========
 
 Get consensus of sequences / mutations. Useful for grouping sequences
 within a barcode.
 
 """
 
-
 import collections
 import io  # noqa: F401
 import itertools
 import math
 import re
 import textwrap  # noqa: F401
 
@@ -457,29 +456,31 @@
         .assign(_n=lambda x: x.groupby(cols)[mutation_col].transform("count"))
         # only retain groups with >1 sequence
         .query("_n > 1")
         # sort mutations
         .assign(
             **{
                 mutation_col: (
-                    lambda x: x[mutation_col].map(lambda s: " ".join(sorted(s.split())))
-                    if sort_mutations
-                    else x[mutation_col]
+                    lambda x: (
+                        x[mutation_col].map(lambda s: " ".join(sorted(s.split())))
+                        if sort_mutations
+                        else x[mutation_col]
+                    )
                 )
             }
         )
         # number of unique sequences in each group
         .assign(_u=lambda x: (x.groupby(cols)[mutation_col].transform("nunique")))
         # number of groups with each combination of n and u
         .groupby(upstream_group_cols + ["_n", "_u"])
         .size()
         .rename("_ngroups")
         .reset_index()
         # get error rate
-        .groupby(upstream_group_cols)
+        .groupby(upstream_group_cols)[["_n", "_u", "_ngroups"]]
         .apply(
             lambda x: 1
             - _LnL_error_rate(
                 x, n_col="_n", u_col="_u", count_col="_ngroups"
             ).maxlik_eps()
         )
         .rename(accuracy_col)
@@ -692,15 +693,15 @@
             "so that empty mutation strings were read as `na` "
             "rather than empty strings."
         )
 
     dropped = []
     consensus = []
     for g, g_df in df.groupby(group_cols, observed=True)[mutation_col]:
-        if len(group_cols) == 1:
+        if len(group_cols) == 1 and isinstance(g, str):
             g = [g]
 
         nseqs = len(g_df)
         half_nseqs = 0.5 * nseqs
         assert nseqs > 0
 
         if nseqs < min_support:
```

### Comparing `alignparse-0.6.2/alignparse/cs_tag.py` & `alignparse-0.6.3/alignparse/cs_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 `minimap2 <https://lh3.github.io/minimap2/>`_ output.
 
 See `here <https://lh3.github.io/minimap2/minimap2.html>`_ for details on
 short ``cs`` tag format.
 
 """
 
-
 import functools
 
 import numpy
 
 import regex
 
 import alignparse.utils
```

### Comparing `alignparse-0.6.2/alignparse/minimap2.py` & `alignparse-0.6.3/alignparse/minimap2.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     >>> mapper.map_to_sam(targetfile, queryfile, samfile)
     >>> for a in pysam.AlignmentFile(samfile):
     ...     tag_names = [tup[0] for tup in a.get_tags()]
     ...     print(a.tostring())  # doctest: +NORMALIZE_WHITESPACE
     m54228_181120_212724/4194376/ccs 0 refseq 1 1 63M * 0 0
     ATGCAAAATGATGCATAGTATTAGCATAAATAGGATAGCCATAAGGTTACTGCATAAGAGTAT
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-    NM:i:4 ms:i:111 AS:i:111 nn:i:3 tp:A:P cm:i:7 s1:i:41 s2:i:0 de:f:0.0167
+    NM:i:4 ms:i:111 AS:i:111 nn:i:3 tp:A:P cm:i:7 s1:i:41 s2:i:0 de:f:0.0635
     cs:Z::6*na*na*nt:49*ga:4 rl:i:0
     >>> print(tag_names)
     ['NM', 'ms', 'AS', 'nn', 'tp', 'cm', 's1', 's2', 'de', 'cs', 'rl']
 
     Now map retaining the `np` tag in the FASTQ:
 
     >>> samfile_tags = os.path.join(tempdir.name, 'alignments_tags.sam')
@@ -164,15 +164,15 @@
     >>> mapper_tags.map_to_sam(targetfile, queryfile, samfile_tags)
     >>> for a in pysam.AlignmentFile(samfile_tags):
     ...     tag_names = [tup[0] for tup in a.get_tags()]
     ...     print(a.tostring())  # doctest: +NORMALIZE_WHITESPACE
     m54228_181120_212724/4194376/ccs 0 refseq 1 1 63M * 0 0
     ATGCAAAATGATGCATAGTATTAGCATAAATAGGATAGCCATAAGGTTACTGCATAAGAGTAT
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-    NM:i:4 ms:i:111 AS:i:111 nn:i:3 tp:A:P cm:i:7 s1:i:41 s2:i:0 de:f:0.0167
+    NM:i:4 ms:i:111 AS:i:111 nn:i:3 tp:A:P cm:i:7 s1:i:41 s2:i:0 de:f:0.0635
     cs:Z::6*na*na*nt:49*ga:4 rl:i:0 np:i:127
     >>> print(tag_names)  # doctest: +NORMALIZE_WHITESPACE
     ['NM', 'ms', 'AS', 'nn', 'tp', 'cm', 's1', 's2', 'de', 'cs', 'rl', 'np']
 
     Remove the temporary directory for the example:
 
     >>> tempdir.cleanup()
@@ -223,15 +223,15 @@
             Queries to align, typically FASTA or FASTQ (can be gzipped).
         samfile : str
             Name of created SAM file (should have suffix ``.sam``).
 
         """
         for fname, f in [("target", targetfile), ("query", queryfile)]:
             if not os.path.isfile(f):
-                raise IOError(f"cannot find `{fname}file` {f}")
+                raise OSError(f"cannot find `{fname}file` {f}")
 
         if os.path.splitext(samfile)[1] != ".sam":
             raise ValueError(f"`samfile` lacks extension '.sam': {samfile}")
 
         if not any("-a" == opt for opt in self.options):
             options = self.options + ["-a"]
 
@@ -244,15 +244,15 @@
                 untagged_samfile = os.path.join(tempdir, os.path.basename(samfile))
             else:
                 untagged_samfile = samfile
 
             # do the alignment
             with contextlib.ExitStack() as stack:
                 sam = stack.enter_context(open(untagged_samfile, "w"))
-                err = stack.enter_context(tempfile.TemporaryFile(mode="w"))
+                err = stack.enter_context(tempfile.TemporaryFile(mode="w+"))
                 try:
                     _ = subprocess.check_call(cmds, stdout=sam, stderr=err)
                 except Exception as exc:
                     if os.path.isfile(untagged_samfile):
                         os.remove(untagged_samfile)
                     exc_type = type(exc).__name__
                     err.seek(0)
```

### Comparing `alignparse-0.6.2/alignparse/targets.py` & `alignparse-0.6.3/alignparse/targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 =======
 
 Defines :class:`Targets`, which holds :class:`Target` objects that define
 alignment targets. Each :class:`Target` has some :class:`Feature` regions.
 
 """
 
-
 import contextlib
 import copy
 import itertools
 import os
 import re
 import tempfile
 
@@ -156,15 +155,15 @@
             if feature_name in self._features_dict:
                 raise ValueError(
                     f"duplicate feature {feature_name} when "
                     f"creating Target {self.name}"
                 )
             if not (allow_extra_features or (feature_name in allow_features)):
                 raise ValueError(f"feature {feature_name} not allowed feature")
-            if bio_feature.strand != 1:
+            if bio_feature.location.strand != 1:
                 raise ValueError(
                     f"feature {feature_name} of {self.name} is - "
                     "strand, but only + strand features handled"
                 )
             feature_seq = str(bio_feature.location.extract(seqrecord).seq)
             feature = Feature(
                 name=feature_name,
@@ -898,15 +897,15 @@
         # now make the alignments
         for tup in df.itertuples():
             os.makedirs(tup.subdir, exist_ok=True)
             if os.path.isfile(tup.samfile):
                 if overwrite:
                     os.remove(tup.samfile)
                 else:
-                    raise IOError(f"file {tup.samfile} already exists")
+                    raise OSError(f"file {tup.samfile} already exists")
         _ = map_func(
             self.align, df[queryfile_col], df["samfile"], itertools.repeat(mapper)
         )
         assert all(os.path.isfile(f) for f in df["samfile"])
 
         # now parse the alignments
         parse_results = map_func(
@@ -949,15 +948,15 @@
         aligned = {
             t: os.path.join(outdir, t.replace(" ", "_") + "_aligned.csv")
             for t in self.target_names
         }
         for f in list(filtered.values()) + list(aligned.values()):
             if os.path.isfile(f):
                 if not overwrite:
-                    raise IOError(f"file {f} already exists.")
+                    raise OSError(f"file {f} already exists.")
                 else:
                     os.remove(f)
 
         # collect read stats for all runs
         readstats = []
         for i, (ireadstats, _, _) in enumerate(parse_results):
             readstats.append(
@@ -1127,15 +1126,15 @@
             }
             aligned = {
                 t: os.path.join(csv_dir, t.replace(" ", "_") + "_aligned.csv")
                 for t in self.target_names
             }
             filenames = list(filtered.values()) + list(aligned.values())
             if (not overwrite_csv) and any(map(os.path.isfile, filenames)):
-                raise IOError(f"existing file with name in: {filenames}")
+                raise OSError(f"existing file with name in: {filenames}")
         else:
             filtered = {t: [] for t in self.target_names}
             aligned = {t: [] for t in self.target_names}
 
         # Iterate samfile in contextlib so can handle files if using `to_csv`.
         with contextlib.ExitStack() as stack:
             # Define callback to delete CSV files on error. See here:
```

### Comparing `alignparse-0.6.2/alignparse/utils.py` & `alignparse-0.6.3/alignparse/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 =====
 utils
 =====
 
 """
 
-
 import math
 import numbers
 import re
 
 import numpy
 
 import pandas as pd  # noqa: F401
```

### Comparing `alignparse-0.6.2/alignparse.egg-info/SOURCES.txt` & `alignparse-0.6.3/alignparse.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-.flake8
 .gitignore
-.travis.yml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
-environment.yml
 nbval_sanitize.cfg
 pytest.ini
 setup.py
 test_requirements.txt
 alignparse/__init__.py
 alignparse/ccs.py
 alignparse/consensus.py
```

### Comparing `alignparse-0.6.2/docs/Makefile` & `alignparse-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/docs/README.rst` & `alignparse-0.6.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/docs/_static/BloomLogo.jpg` & `alignparse-0.6.3/docs/_static/BloomLogo.jpg`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/docs/acknowledgements.rst` & `alignparse-0.6.3/docs/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/docs/conf.py` & `alignparse-0.6.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-#
 # alignparse documentation build configuration file.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
@@ -17,15 +15,15 @@
 """Configuration file for sphinx."""
 
 import datetime
 import os
 import re
 import sys
 
-sys.path.insert(0, "{0}/..".format(os.path.abspath(".")))
+sys.path.insert(0, "{}/..".format(os.path.abspath(".")))
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = "1.0"
```

### Comparing `alignparse-0.6.2/docs/examples.rst` & `alignparse-0.6.3/docs/examples.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,9 +12,7 @@
    :maxdepth: 1
 
    recA_DMS
    lasv_pilot
    flu_virus_seq_example
 
 The actual notebooks and input files used in these examples are `available here <https://github.com/jbloomlab/alignparse/tree/master/notebooks>`_.
-
-The above examples can also be run as interactive Jupyter notebooks on `mybinder <https://mybinder.readthedocs.io>`_ by going to the `following link <https://mybinder.org/v2/gh/jbloomlab/alignparse/master?filepath=notebooks>`_ (it may take a minute to load) and then opening the notebook you want to run.
```

### Comparing `alignparse-0.6.2/docs/index.rst` & `alignparse-0.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/docs/installation.rst` & `alignparse-0.6.3/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Installation
 --------------
 
-`alignparse <https://jbloomlab.github.io/alignparse/>`_ requires Python 3.8 or higher and is currently tested on Python 3.9.
+`alignparse <https://jbloomlab.github.io/alignparse/>`_ requires Python 3.8 or higher and is currently tested on Python 3.11.
 A Mac OS X or Linux operating system is also required.
 
 The easiest way to install `alignparse <https://jbloomlab.github.io/alignparse/>`_ is from `PyPI <https://pypi.org/>`_ using `pip <https://pip.pypa.io>`_ with::
 
     pip install alignparse
 
 Note that installing the dependency `pysam <https://pysam.readthedocs.io/en/latest/api.html>`_ may require additional packages on the host system.
```

### Comparing `alignparse-0.6.2/notebooks/input_files/LASV_Josiah_OPT.gb` & `alignparse-0.6.3/notebooks/input_files/LASV_Josiah_OPT.gb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/LASV_Josiah_WT.gb` & `alignparse-0.6.3/notebooks/input_files/LASV_Josiah_WT.gb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/README.rst` & `alignparse-0.6.3/notebooks/input_files/README.rst`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/flu_WSN_amplicons.gb` & `alignparse-0.6.3/notebooks/input_files/flu_WSN_amplicons.gb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/flu_WSN_ccs.fastq` & `alignparse-0.6.3/notebooks/input_files/flu_WSN_ccs.fastq`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/flu_WSN_feature_parse_specs.yaml` & `alignparse-0.6.3/notebooks/input_files/flu_WSN_feature_parse_specs.yaml`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/lasv_example_ccs.fastq.gz` & `alignparse-0.6.3/notebooks/input_files/lasv_example_ccs.fastq.gz`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/lasv_feature_parse_specs.yaml` & `alignparse-0.6.3/notebooks/input_files/lasv_feature_parse_specs.yaml`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/lasv_pilot_report.txt` & `alignparse-0.6.3/notebooks/input_files/lasv_pilot_report.txt`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_amplicon.gb` & `alignparse-0.6.3/notebooks/input_files/recA_amplicon.gb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_feature_parse_specs.yaml` & `alignparse-0.6.3/notebooks/input_files/recA_feature_parse_specs.yaml`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_lib-1_ccs.fastq` & `alignparse-0.6.3/notebooks/input_files/recA_lib-1_ccs.fastq`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_lib-1_report.txt` & `alignparse-0.6.3/notebooks/input_files/recA_lib-1_report.txt`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_lib-2_ccs.fastq` & `alignparse-0.6.3/notebooks/input_files/recA_lib-2_ccs.fastq`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/input_files/recA_lib-2_report.txt` & `alignparse-0.6.3/notebooks/input_files/recA_lib-2_report.txt`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/notebooks/lasv_pilot.ipynb` & `alignparse-0.6.3/notebooks/lasv_pilot.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969186027905786%*

 * *Differences: {"'cells'": "{2: {'metadata': {'execution': {'iopub.execute_input': '2024-05-23T18:06:27.680590Z', "*

 * *            "'iopub.status.busy': '2024-05-23T18:06:27.680149Z', 'iopub.status.idle': "*

 * *            "'2024-05-23T18:06:31.717771Z', 'shell.execute_reply': '2024-05-23T18:06:31.716937Z', "*

 * *            "'shell.execute_reply.started': '2024-05-23T18:06:27.680557Z'}}}, 4: {'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2024-05-23T18:06:31.720334Z', "*

 * *            "'iopub.status.busy': '2024-05- […]*

```diff
@@ -21,19 +21,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:50.285491Z",
-                    "iopub.status.busy": "2023-06-19T11:20:50.284583Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.904111Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.902769Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:50.285452Z"
+                    "iopub.execute_input": "2024-05-23T18:06:27.680590Z",
+                    "iopub.status.busy": "2024-05-23T18:06:27.680149Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.717771Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.716937Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:27.680557Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import tempfile\n",
                 "import warnings\n",
@@ -62,19 +62,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.906497Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.905958Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.910617Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.909750Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.906467Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.720334Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.719872Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.723583Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.722917Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.720306Z"
                 }
             },
             "outputs": [],
             "source": [
                 "warnings.simplefilter(\"ignore\")"
             ]
         },
@@ -86,19 +86,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.911839Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.911592Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.915465Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.914744Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.911817Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.724731Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.724436Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.728224Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.727532Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.724705Z"
                 }
             },
             "outputs": [],
             "source": [
                 "outdir = \"./output_files/\"\n",
                 "os.makedirs(outdir, exist_ok=True)"
             ]
@@ -111,19 +111,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.917566Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.917225Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.920993Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.920228Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.917541Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.729604Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.729285Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.733335Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.732450Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.729573Z"
                 }
             },
             "outputs": [],
             "source": [
                 "CBPALETTE = (\"#999999\", \"#E69F00\", \"#56B4E9\", \"#009E73\")"
             ]
         },
@@ -140,19 +140,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.922660Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.922081Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.009637Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.008073Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.922632Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.735845Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.735032Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.742332Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.741750Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.735790Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -326,19 +326,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.012195Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.011316Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.066690Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.065892Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.012158Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.743703Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.743415Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.749052Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.748095Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.743677Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -390,19 +390,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.068516Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.068082Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.106915Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.105634Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.068486Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.755591Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.755090Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.893571Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.892700Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.755546Z"
                 }
             },
             "outputs": [],
             "source": [
                 "targets = alignparse.targets.Targets(\n",
                 "    seqsfile=targetfiles,\n",
                 "    feature_parse_specs=lasv_parse_specs_file,\n",
@@ -418,19 +418,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.109138Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.108223Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.119036Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.118149Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.109062Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.895056Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.894755Z",
+                    "iopub.status.idle": "2024-05-23T18:06:31.906140Z",
+                    "shell.execute_reply": "2024-05-23T18:06:31.905413Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.895023Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -508,25 +508,25 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.120763Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.120358Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.632056Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.630842Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.120731Z"
+                    "iopub.execute_input": "2024-05-23T18:06:31.907942Z",
+                    "iopub.status.busy": "2024-05-23T18:06:31.907578Z",
+                    "iopub.status.idle": "2024-05-23T18:06:32.445595Z",
+                    "shell.execute_reply": "2024-05-23T18:06:32.444747Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:31.907912Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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o0Z4eHgwY8YMOnTowOjRo5k3bx4rVqxg4sSJJCcnU7BgQZ599lmGDRuWbjLQsGFDQkJCiI6OvuclhzeTnlvjDA4OZtOmTbz66quMGzeOxMREypUrx9KlS2nZsqWl3FNPPcXMmTP55JNPiI2NJSwsjEGDBjFs2LDbtpcnTx6WLVvGSy+9xLBhw/D396dHjx40atSIZs2a3dM9ZFThwoXJnz8/Z86cSTcpjoqKYsmSJVpyKCLykDCYbfGrPxERkX/88ccflC9fnkmTJtG3b197hyMiImIzeuZLRERs6uY7um4+xyUiIvKw0MyXiIhkieTkZC5dunTb80ePHuWnn35i1KhR5MuXj71791qe5cpNLly4gNFovO15FxcXAgICbBiRiIjkFnrmS0REssSmTZvuuo29h4cHderUYdy4cbky8YIbL6a++dLn9NSrV8+yfbyIiMitNPMlIiJZ4vLly+zcufOOZUqXLk1ISIiNIsoeGzduJCEh4bbn/f39qVy5sg0jEhGR3ELJl4iIiIiIiA3kzjUfIiIiIiIiuYySLxERERERERtQ8iUiIiIiImIDSr5ERERERERsQMmXiIiIiIiIDSj5EhERERERsQElXyIiIiIiIjag5EtERERERMQGlHyJiIiIiIjYgJIvERERERERG1DyJSIiIiIiYgNKvkRERERERGzAKTsrN5vNHDp0iD179nD27FlSUlKys7ks4+joSEBAACVLlqRkyZK4uLjYOyQREREREcnlDGaz2ZwdFZvNZpYuXcquXbvwzRNAaEQhnF1cwJAdrWUtY2oqF85Ec+7UKUJDQ+nRowdubm72DktERERERHKxbEu+tmzZwurVq6nftg3FypXDYMgFWdd/nD99hhUzZ1IkMpJOnTrZOxwREREREcnFsu2Zrz///JOIEsUpXr58rky8AIJC81Ohdi32799PcnKyvcMREREREZFcLFuSr+TkZM6cOUN4sWLZUb1NhRctSmpqKqdOnbJ3KCIiIiIikotlS/KVlJQEgLuHZ7rnn+/Th/ply913O3/9/jshDo5sWrfuvuu6HXcvLwASExOzrQ0REREREXnwZctuhzcfI7vdcsMXhg0jPi4uO5rOcrl1yaSIiIiIiOQs2brV/O1EREbao1kRERERERG7sctLlm9ddjh3yhRCHBz5c9cuurVoQWEvb6KKFee7adPSXDf2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ATeShOrVq7N+/Xry5MmDn58fP//8M97e3lbvR7l69SoJCQlcvXoVs9ls6eeAgADLe2YeVsWKFWP9+vX4+voSFBREdHQ0W7ZssQyc1Mf35m7/j92tTwMDAylSpAhLly6lVatWGI1GVqxYQZkyZaxmyy5cuIDRaCQhIYHk5GRLv99M6h50d+pnLy8v5s2bR3R0NF27dsVsNlv+P3R3d8fR0VH9nAF3+7v834TWwcEBLy8vy7tF1ccZc7d+joqKYv78+RQsWJBChQpx6NAh9u/fT+/evQE0tsvBDOabv87MwY4dO8bUqVPTHC9fvjzt2rWzfUC5zLvvvpvu8bZt21oGVDdfxPfXX39hNBqJjIykZcuWVlPTU6ZM4fjx42nqef755/Hz88uO0HO1KVOmkC9fvjQvWVYf358DBw7w448/EhMTg7+/PzVq1KBy5cqW8zdfVrtz504SExMpWLBgmpfVLlq0iN27d6ep++aDyg+zpKQkfv75Z/7++2/LMrgyZcpQr149y3/E6uPMu9v/Yxnp04SEBFasWMGBAwfSfTEtwKeffmrZNv1Wb7/9dvbcWA5zp36uX78+n332WbrX3fr3Uv18Z5kdk3366afUqFEjzUuW1cd3lpF+3rVrFxs2bODatWvkyZOH+vXrW/0STOOOnClXJF8iIiIiIiK5nd7zJSIiIiIiYgNKvkRERERERGxAyZeIiIiIiIgNKPkSERERERGxASVfIiIiIiIiNqDkS0RERERExAaUfImIiIiIiNiAki8REREREREbUPIlIiIiIiJiA0q+REREREREbEDJl4iIiIiIiA0o+RIREREREbEBJV8iIiIiIiI2oORLRERERETEBpR8iYiIiIiI2ICSLxERERERERtQ8iUiIiIiImIDSr5ERERERERsQMmXiIiIiIiIDSj5EhERERERsQElXyIiIiIiIjag5EtERERERMQGlHyJiIiIiIjYgJIvERERERERG1DyJSIiIiIiYgNKvkRERERERGxAyZeIiIiIiIgNKPkSERERERGxASVfIiIiIiIiNqDkS0RERERExAaUfImIiIiIiNiAki8REREREREbUPIlIiIiIiJiA0q+REQk15syZQoGg4Fjx45l+tr69etTpkyZrA9KRETkP5R8iYjkYDeTih07dmSofLVq1TAYDEyYMOG2Zf788086depEeHg4bm5u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",
+                        "image/png": "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o0Z4eHgwY8YMOnTowOjRo5k3bx4rVqxg4sSJJCcnU7BgQZ599lmGDRuWbjLQsGFDQkJCiI6OvuclhzeTnlvjDA4OZtOmTbz66quMGzeOxMREypUrx9KlS2nZsqWl3FNPPcXMmTP55JNPiI2NJSwsjEGDBjFs2LDbtpcnTx6WLVvGSy+9xLBhw/D396dHjx40atSIZs2a3dM9ZFThwoXJnz8/Z86cSTcpjoqKYsmSJVpyKCLykDCYbfGrPxERkX/88ccflC9fnkmTJtG3b197hyMiImIzeuZLRERs6uY7um4+xyUiIvKw0MyXiIhkieTkZC5dunTb80ePHuWnn35i1KhR5MuXj71791qe5cpNLly4gNFovO15FxcXAgICbBiRiIjkFnrmS0REssSmTZvuuo29h4cHderUYdy4cbky8YIbL6a++dLn9NSrV8+yfbyIiMitNPMlIiJZ4vLly+zcufOOZUqXLk1ISIiNIsoeGzduJCEh4bbn/f39qVy5sg0jEhGR3ELJl4iIiIiIiA3kzjUfIiIiIiIiuYySLxERERERERtQ8iUiIiIiImIDSr5ERERERERsQMmXiIiIiIiIDSj5EhERERERsQElXyIiIiIiIjag5EtERERERMQGlHyJiIiIiIjYgJIvERERERERG1DyJSIiIiIiYgNKvkRERERERGzAKTsrN5vNHDp0iD179nD27FlSUlKys7ks4+joSEBAACVLlqRkyZK4uLjYOyQREREREcnlDGaz2ZwdFZvNZpYuXcquXbvwzRNAaEQhnF1cwJAdrWUtY2oqF85Ec+7UKUJDQ+nRowdubm72DktERERERHKxbEu+tmzZwurVq6nftg3FypXDYMgFWdd/nD99hhUzZ1IkMpJOnTrZOxwREREREcnFsu2Zrz///JOIEsUpXr58rky8AIJC81Ohdi32799PcnKyvcMREREREZFcLFuSr+TkZM6cOUN4sWLZUb1NhRctSmpqKqdOnbJ3KCIiIiIikotlS/KVlJQEgLuHZ7rnn+/Th/ply913O3/9/jshDo5sWrfuvuu6HXcvLwASExOzrQ0REREREXnwZctuhzcfI7vdcsMXhg0jPi4uO5rOcrl1yaSIiIiIiOQs2brV/O1EREbao1kRERERERG7sctLlm9ddjh3yhRCHBz5c9cuurVoQWEvb6KKFee7adPSXDf2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ATeShOrVq7N+/Xry5MmDn58fP//8M97e3lbvR7l69SoJCQlcvXoVs9ls6eeAgADLe2YeVsWKFWP9+vX4+voSFBREdHQ0W7ZssQyc1Mf35m7/j92tTwMDAylSpAhLly6lVatWGI1GVqxYQZkyZaxmyy5cuIDRaCQhIYHk5GRLv99M6h50d+pnLy8v5s2bR3R0NF27dsVsNlv+P3R3d8fR0VH9nAF3+7v834TWwcEBLy8vy7tF1ccZc7d+joqKYv78+RQsWJBChQpx6NAh9u/fT+/evQE0tsvBDOabv87MwY4dO8bUqVPTHC9fvjzt2rWzfUC5zLvvvpvu8bZt21oGVDdfxPfXX39hNBqJjIykZcuWVlPTU6ZM4fjx42nqef755/Hz88uO0HO1KVOmkC9fvjQvWVYf358DBw7w448/EhMTg7+/PzVq1KBy5cqW8zdfVrtz504SExMpWLBgmpfVLlq0iN27d6ep++aDyg+zpKQkfv75Z/7++2/LMrgyZcpQr149y3/E6uPMu9v/Yxnp04SEBFasWMGBAwfSfTEtwKeffmrZNv1Wb7/9dvbcWA5zp36uX78+n332WbrX3fr3Uv18Z5kdk3366afUqFEjzUuW1cd3lpF+3rVrFxs2bODatWvkyZOH+vXrW/0STOOOnClXJF8iIiIiIiK5nd7zJSIiIiIiYgNKvkRERERERGxAyZeIiIiIiIgNKPkSERERERGxASVfIiIiIiIiNqDkS0RERERExAaUfImIiIiIiNiAki8REREREREbUPIlIiIiIiJiA0q+REREREREbEDJl4iIiIiIiA0o+RIREREREbEBJV8iIiIiIiI2oORLRERERETEBpR8iYiIiIiI2ICSLxERERERERtQ8iUiIiIiImIDSr5ERERERERsQMmXiIiIiIiIDSj5EhERERERsQElXyIiIiIiIjag5EtERERERMQGlHyJiIiIiIjYgJIvERERERERG1DyJSIiIiIiYgNKvkRERERERGxAyZeIiIiIiIgNKPkSERERERGxASVfIiIiIiIiNqDkS0RERERExAaUfImIiIiIiNiAki8REREREREbUPIlIiIiIiJiA0q+REQk15syZQoGg4Fjx45l+tr69etTpkyZrA9KRETkP5R8iYjkYDeTih07dmSofLVq1TAYDEyYMOG2Zf788086depEeHg4bm5u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",
                         "text/plain": [
                             "<Figure size 1000x600 with 2 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -547,19 +547,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.636227Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.635659Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.649119Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.648187Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.636190Z"
+                    "iopub.execute_input": "2024-05-23T18:06:32.446884Z",
+                    "iopub.status.busy": "2024-05-23T18:06:32.446568Z",
+                    "iopub.status.idle": "2024-05-23T18:06:32.459985Z",
+                    "shell.execute_reply": "2024-05-23T18:06:32.459342Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:32.446847Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -602,19 +602,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.650469Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.650152Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.663230Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.662346Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.650447Z"
+                    "iopub.execute_input": "2024-05-23T18:06:32.461260Z",
+                    "iopub.status.busy": "2024-05-23T18:06:32.460833Z",
+                    "iopub.status.idle": "2024-05-23T18:06:32.474256Z",
+                    "shell.execute_reply": "2024-05-23T18:06:32.473547Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:32.461235Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -688,19 +688,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.664739Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.664347Z",
-                    "iopub.status.idle": "2023-06-19T11:20:54.576091Z",
-                    "shell.execute_reply": "2023-06-19T11:20:54.575160Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.664714Z"
+                    "iopub.execute_input": "2024-05-23T18:06:32.475522Z",
+                    "iopub.status.busy": "2024-05-23T18:06:32.475184Z",
+                    "iopub.status.idle": "2024-05-23T18:06:33.310276Z",
+                    "shell.execute_reply": "2024-05-23T18:06:33.309033Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:32.475494Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ccs_summaries = alignparse.ccs.Summaries(pacbio_runs)"
             ]
         },
@@ -712,19 +712,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:54.578435Z",
-                    "iopub.status.busy": "2023-06-19T11:20:54.578018Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.098900Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.097926Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:54.578407Z"
+                    "iopub.execute_input": "2024-05-23T18:06:33.312544Z",
+                    "iopub.status.busy": "2024-05-23T18:06:33.312072Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.138029Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.137019Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:33.312500Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "p = ccs_summaries.plot_zmw_stats()\n",
@@ -732,19 +732,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.100524Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.100128Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.143469Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.142580Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.100501Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.139792Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.139349Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.194531Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.193912Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.139764Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -844,19 +844,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.144853Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.144479Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.864073Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.863012Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.144831Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.195919Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.195449Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.797352Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.796682Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.195892Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "for stat in [\"length\", \"passes\", \"accuracy\"]:\n",
@@ -878,32 +878,34 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.865788Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.865356Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.896448Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.895084Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.865760Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.798626Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.798266Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.809961Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.809078Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.798601Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Using `minimap2` 2.17-r941 with these options:\n",
+                        "Using `minimap2` 2.22-r1101 with these options:\n",
                         "-A2 -B4 -O12 -E2 --end-bonus=13 --secondary=no --cs\n"
                     ]
                 }
             ],
             "source": [
+                "# NBVAL_IGNORE_OUTPUT\n",
+                "\n",
                 "mapper = alignparse.minimap2.Mapper(alignparse.minimap2.OPTIONS_CODON_DMS)\n",
                 "\n",
                 "print(\n",
                 "    f\"Using `minimap2` {mapper.version} with these options:\\n\"\n",
                 "    + \" \".join(mapper.options)\n",
                 ")"
             ]
@@ -917,19 +919,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.899307Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.898620Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.915701Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.914586Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.899243Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.811699Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.811270Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.823979Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.823306Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.811661Z"
                 },
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -1001,19 +1003,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.917362Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.916958Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.026319Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.024727Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.917335Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.825383Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.825027Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.930651Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.929339Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.825354Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1037,19 +1039,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.029250Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.028686Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.038450Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.037325Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.029193Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.932964Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.932389Z",
+                    "iopub.status.idle": "2024-05-23T18:06:34.940875Z",
+                    "shell.execute_reply": "2024-05-23T18:06:34.939933Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.932907Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1079,19 +1081,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.040496Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.039993Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.240520Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.239835Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.040452Z"
+                    "iopub.execute_input": "2024-05-23T18:06:34.942818Z",
+                    "iopub.status.busy": "2024-05-23T18:06:34.942189Z",
+                    "iopub.status.idle": "2024-05-23T18:06:35.502285Z",
+                    "shell.execute_reply": "2024-05-23T18:06:35.501601Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:34.942783Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1135,19 +1137,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.241851Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.241639Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.249775Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.248984Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.241831Z"
+                    "iopub.execute_input": "2024-05-23T18:06:35.503468Z",
+                    "iopub.status.busy": "2024-05-23T18:06:35.503245Z",
+                    "iopub.status.idle": "2024-05-23T18:06:35.512662Z",
+                    "shell.execute_reply": "2024-05-23T18:06:35.511886Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:35.503446Z"
                 },
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -1228,19 +1230,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.251104Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.250631Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.389831Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.389031Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.251080Z"
+                    "iopub.execute_input": "2024-05-23T18:06:35.518503Z",
+                    "iopub.status.busy": "2024-05-23T18:06:35.518113Z",
+                    "iopub.status.idle": "2024-05-23T18:06:35.649601Z",
+                    "shell.execute_reply": "2024-05-23T18:06:35.648283Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:35.518472Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "p = (\n",
@@ -1263,19 +1265,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.391096Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.390768Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.399208Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.398481Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.391074Z"
+                    "iopub.execute_input": "2024-05-23T18:06:35.651362Z",
+                    "iopub.status.busy": "2024-05-23T18:06:35.651000Z",
+                    "iopub.status.idle": "2024-05-23T18:06:35.663816Z",
+                    "shell.execute_reply": "2024-05-23T18:06:35.662995Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:35.651338Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1368,19 +1370,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.400429Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.400175Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.752143Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.751095Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.400405Z"
+                    "iopub.execute_input": "2024-05-23T18:06:35.665706Z",
+                    "iopub.status.busy": "2024-05-23T18:06:35.665307Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.006445Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.005674Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:35.665669Z"
                 },
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
@@ -1417,19 +1419,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.753557Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.753327Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.368663Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.367899Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.753538Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.007729Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.007417Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.675127Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.674361Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.007703Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "error_rate_floor = 1e-7  # error rates < this set to this\n",
@@ -1470,19 +1472,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.369993Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.369598Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.375735Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.374989Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.369971Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.676680Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.676344Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.683034Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.682323Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.676656Z"
                 }
             },
             "outputs": [],
             "source": [
                 "retained = {targetname: [] for targetname in targets.target_names}\n",
                 "for targetname in targets.target_names:\n",
                 "    target_retained = aligned[targetname][\n",
@@ -1503,19 +1505,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.376935Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.376623Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.391413Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.390737Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.376914Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.684798Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.684431Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.702566Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.701654Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.684771Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1693,19 +1695,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.395414Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.395006Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.406411Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.405755Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.395387Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.704097Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.703709Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.717796Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.716977Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.704065Z"
                 }
             },
             "outputs": [],
             "source": [
                 "indices = {\n",
                 "    \"LASV_Josiah_WT\": [\"AGACAC\", \"GGTATG\"],\n",
                 "    \"LASV_Josiah_OPT\": [\"ACGACC\", \"CTTCAC\", \"GAGACG\"],\n",
@@ -1743,19 +1745,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 29,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.407815Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.407493Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.621266Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.620387Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.407795Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.719460Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.719131Z",
+                    "iopub.status.idle": "2024-05-23T18:06:36.988751Z",
+                    "shell.execute_reply": "2024-05-23T18:06:36.987969Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.719436Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "for target_name in targets.target_names:\n",
@@ -1786,19 +1788,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 30,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.622462Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.622186Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.650715Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.649851Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.622442Z"
+                    "iopub.execute_input": "2024-05-23T18:06:36.990634Z",
+                    "iopub.status.busy": "2024-05-23T18:06:36.990275Z",
+                    "iopub.status.idle": "2024-05-23T18:06:37.029580Z",
+                    "shell.execute_reply": "2024-05-23T18:06:37.028748Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:36.990612Z"
                 },
                 "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -2144,19 +2146,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 31,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.652289Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.651884Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.672104Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.671142Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.652255Z"
+                    "iopub.execute_input": "2024-05-23T18:06:37.030955Z",
+                    "iopub.status.busy": "2024-05-23T18:06:37.030612Z",
+                    "iopub.status.idle": "2024-05-23T18:06:37.046260Z",
+                    "shell.execute_reply": "2024-05-23T18:06:37.045472Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:37.030927Z"
                 }
             },
             "outputs": [],
             "source": [
                 "for target_idx in target_idx_retained:\n",
                 "    target_idx_retained[target_idx] = alignparse.consensus.add_mut_info_cols(\n",
                 "        target_idx_retained[target_idx],\n",
@@ -2176,19 +2178,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 32,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.673764Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.673319Z",
-                    "iopub.status.idle": "2023-06-19T11:20:58.625267Z",
-                    "shell.execute_reply": "2023-06-19T11:20:58.621631Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.673733Z"
+                    "iopub.execute_input": "2024-05-23T18:06:37.047681Z",
+                    "iopub.status.busy": "2024-05-23T18:06:37.047263Z",
+                    "iopub.status.idle": "2024-05-23T18:06:38.053149Z",
+                    "shell.execute_reply": "2024-05-23T18:06:38.051878Z",
+                    "shell.execute_reply.started": "2024-05-23T18:06:37.047655Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "mut_cols = [\"n_gene_subs\", \"n_gene_indels\"]\n",
@@ -2221,15 +2223,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.9"
         },
         "toc": {
             "nav_menu": {},
             "number_sections": false,
             "sideBar": true,
             "skip_h1_title": false,
             "toc_cell": false,
```

### Comparing `alignparse-0.6.2/notebooks/recA_DMS.ipynb` & `alignparse-0.6.3/notebooks/recA_DMS.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968838832712166%*

 * *Differences: {"'cells'": "{2: {'metadata': {'execution': {'iopub.execute_input': '2024-05-23T18:11:28.075817Z', "*

 * *            "'iopub.status.busy': '2024-05-23T18:11:28.075508Z', 'iopub.status.idle': "*

 * *            "'2024-05-23T18:11:31.029873Z', 'shell.execute_reply': '2024-05-23T18:11:31.028964Z', "*

 * *            "'shell.execute_reply.started': '2024-05-23T18:11:28.075789Z'}}}, 4: {'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2024-05-23T18:11:31.034049Z', "*

 * *            "'iopub.status.busy': '2024-05- […]*

```diff
@@ -18,19 +18,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:48.284558Z",
-                    "iopub.status.busy": "2023-06-19T11:20:48.283844Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.231785Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.230917Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:48.284513Z"
+                    "iopub.execute_input": "2024-05-23T18:11:28.075817Z",
+                    "iopub.status.busy": "2024-05-23T18:11:28.075508Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.029873Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.028964Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:28.075789Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import warnings\n",
                 "\n",
@@ -57,19 +57,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.233686Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.233269Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.238119Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.237089Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.233659Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.034049Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.033729Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.037853Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.037005Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.034021Z"
                 }
             },
             "outputs": [],
             "source": [
                 "warnings.simplefilter(\"ignore\")"
             ]
         },
@@ -81,19 +81,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.240231Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.239506Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.244708Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.243827Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.240183Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.041720Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.041385Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.045733Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.044937Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.041692Z"
                 }
             },
             "outputs": [],
             "source": [
                 "outdir = \"./output_files/\"\n",
                 "os.makedirs(outdir, exist_ok=True)"
             ]
@@ -111,19 +111,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.246597Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.245993Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.279128Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.278089Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.246558Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.050536Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.050145Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.056477Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.055658Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.050502Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -204,19 +204,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.283233Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.282543Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.313738Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.312710Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.283190Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.061598Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.061206Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.066683Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.065960Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.061567Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -266,19 +266,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.315455Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.315017Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.371635Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.370396Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.315420Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.071237Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.070654Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.103527Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.102551Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.071203Z"
                 }
             },
             "outputs": [],
             "source": [
                 "targets = alignparse.targets.Targets(\n",
                 "    seqsfile=recA_targetfile, feature_parse_specs=recA_parse_specs_file\n",
                 ")"
@@ -294,25 +294,25 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.373954Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.372930Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.611315Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.610655Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.373875Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.105478Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.105175Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.344586Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.343791Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.105447Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA1YAAAEpCAYAAACQt7NWAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjkuMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy80BEi2AAAACXBIWXMAAA9hAAAPYQGoP6dpAABZNUlEQVR4nO3dd1QUVxsG8GdZlqX3XgRpimLvHRVj793YW6yJiZqmxpZojMYYu1/svaBib1hi7y12UUFAlCoC0nZ3vj8IG1e6Cyzl+Z2z57Az99555zoh83Lv3BEJgiCAiIiIiIiIPpmWpgMgIiIiIiIq6ZhYERERERERqYmJFRERERERkZqYWBEREREREamJiRUREREREZGamFgRERERERGpiYkVERERERGRmphYERERERERqYmJFRERERERkZqYWBERUbGzfv16iEQiBAUFaTqUIpHV+fr4+MDHx0djMRERUf4wsSIiyqeMm+CMj7a2NhwcHDB48GCEhYUV+vEfPnwIkUgEXV1dvH379pPa+PgcdHV14enpiXHjxuHNmzcFG/C/fHx8VI6po6OD8uXLY+TIkQgJCSmUYxIRERUVbU0HQERUUs2aNQvly5dHcnIyLl++jPXr1+P8+fO4d+8edHV1C+24mzdvhq2tLWJjY+Hn54fhw4d/clsfnsP58+exYsUKHD58GPfu3YO+vn4BRp3O0dERc+fOBQCkpqbiwYMHWLlyJY4dO4aHDx8qjzlgwAD06dMHUqm0wGMoKY4fP67pEIiIKB+YWBERfaK2bduidu3aAIDhw4fD0tIS8+bNw/79+9GrV69COaYgCNi6dSv69euHFy9eYMuWLWolVh+fg4WFBRYuXIh9+/ahb9++BRW2komJCfr376+yrXz58hg3bhwuXLiAVq1aAQDEYjHEYnGBH78k0dHR0XQIRESUD5wKSERUQJo0aQIAePbsmXLbo0eP0KNHD5ibm0NXVxe1a9fG/v37M9V9+/Ytvv76a7i4uEAqlcLR0REDBw5EVFSUSrkLFy4gKCgIffr0QZ8+fXD27FmEhoYW2Dm0aNECAPDixQsAwIIFC9CwYUNYWFhAT08PtWrVgp+fX5Z1N2/ejLp160JfXx9mZmZo2rRpnkZdbG1tAQDa2v/9rS+7Z6yWL1+OypUrQyqVwt7eHmPHjs33dMiYmBhMmjQJVapUgaGhIYyNjdG2bVvcuXNHpdyZM2cgEomwc+dOzJw5Ew4ODjAyMkKPHj0QFxeHlJQUTJgwAdbW1jA0NMSQIUOQkpKi0oZIJMK4ceOwZcsWVKhQAbq6uqhVqxbOnj2ba5xZPWOVnJyMGTNmwNPTE7q6urCzs0O3bt1UrrnExERMnDgRTk5OkEqlqFChAhYsWABBELKMzd/fH97e3pBKpahcuTKOHj2ar/4kIqJ0HLEiIiogGUmAmZkZAOD+/fto1KgRHBwc8P3338PAwAA7d+5Ely5dsHv3bnTt2hUAkJCQgCZNmuDhw4cYOnQoatasiaioKOzfvx+hoaGwtLRUHmPLli1wc3NDnTp14O3tDX19fWzbtg2TJ08ukHPIuEG3sLAAAPz555/o1KkTPv/8c6SmpmL79u3o2bMnDh48iPbt2yvrzZw5EzNmzEDDhg0xa9Ys6Ojo4MqVKzh16hQ+++wzZTm5XK5MFtPS0vDw4UNMnz4d7u7uaNSoUY6xzZgxAzNnzoSvry9Gjx6Nx48fY8WKFbh27RouXLgAiUSSp3N8/vw5/P390bNnT5QvXx5v3rzBqlWr0KxZMzx48AD29vYq5efOnQs9PT18//33CAwMxJIlSyCRSKClpYXY2FjMmDFDORW0fPny+Omnn1Tq//3339ixYwe+/PJLSKVSLF++HG3atMHVq1fh7e2dp5gz+q5Dhw44efIk+vTpg6+++grx8fE4ceIE7t27Bzc3NwiCgE6dOuH06dMYNmwYqlevjmPHjmHy5MkICwvDH3/8odLm+fPnsWfPHowZMwZGRkZYvHgxunfvjpcvXyqvASIiyiOBiIjyZd26dQIAISAgQIiMjBRCQkIEPz8/wcrKSpBKpUJISIggCILQsmVLoUqVKkJycrKyrkKhEBo2bCh4eHgot/30008CAGHPnj2ZjqVQKJQ/p6amChYWFsKUKVOU2/r16ydUq1atQM5h+/btgoWFhaCnpyeEhoYKgiAI79+/V6mXmpoqeHt7Cy1atFBue/r0qaClpSV07dpVkMvl2cbfrFkzAUCmj5eXl/D8+fMs43vx4oUgCIIQEREh6OjoCJ999pnKMZYuXSoAENauXZvnc09OTs4U54sXLwSpVCrMmjVLue306dMCAMHb21tITU1Vbu/bt68gEomEtm3bqrTRoEEDwdnZWWVbxjlev35duS04OFjQ1dUVunbtmu35CkJ6fzVr1kz5fe3atQIAYeHChZnOKaOf/f39BQDCzz//rLK/R48egkgkEgIDA1Vi09HRUdl2584dAYCwZMmSTMcgIqKccSogEdEn8vX1hZWVFZycnNCjRw8YGBhg//79cHR0RExMDE6dOoVevXohPj4eUVFRiIqKQnR0NFq3bo2nT58qVxDcvXs3qlWrphzB+pBIJFL+fOTIEURHR6s8+9S3b1/cuXMH9+/fV/sc+vTpA0NDQ+zduxcODg4AAD09PWXZ2NhYxMXFoUmTJrh586Zyu7+/PxQKBX766Sdoaan+b+XD+AHAxcUFJ06cwIkTJ3DkyBEsWrQIcXFxaNu2LSIjI7ONMyAgAKmpqZgwYYLKMUaMGAFjY2McOnQoz+cslUqVbcjlckRHR8PQ0BAVKlRQOa8MAwcOVBkNq1evHgRBwNChQ1XK1atXDyEhIZDJZCrbGzRogFq1aim/lytXDp07d8axY8cgl8vzHPfu3bthaWmJ8ePHZ9qX0c+HDx+GWCzGl19+qbJ/4sSJEAQBR44cUdnu6+sLNzc35feqVavC2NgYz58/z3NcRESUjlMBiYg+0bJly+Dp6Ym4uDisXbsWZ8+eVa5iFxgYCEEQMG3aNEybNi3L+hEREXBwcMCzZ8/QvXv3XI+3efNmlC9fHlKpFIGBgQAANzc36OvrY8uWLZgzZ84nn4O2tjZsbGxQoUIFlcTl4MGD+Pnnn3H79m2V54c+TJiePXsGLS0tVKpUKdfjGRgYwNfXV/m9TZs2aNy4MWrXro1ff/0Vv//+e5b1goODAQAVKlRQ2a6jowNXV1fl/rxQKBT4888/sXz5crx48UIluclq+lu5cuVUvpuYmAAAnJycMm1XKBSIi4tTacfDwyNTm56ennj//j0iIyOVz5jl5tmzZ6hQoYLKs2gfCw4Ohr29PYyMjFS2e3l5Kfd/6ONzA9KnssbGxuYpJiIi+g8TKyKiT1S3bl3linpdunRB48aN0a9fPzx+/BgKhQIAMGnSJLRu3TrL+u7u7nk+1rt373DgwAEkJydneaO+detW/PLLL5lGiPJzDh87d+4cOnXqhKZNm2L58uWws7ODRCLBunXrsHXr1nwdJye1atWCiYlJnhZ0KAhz5szBtGnTMHToUMyePRvm5ubQ0tLChAkTlP9uH8pudcLstgsfLRJRnJWGcyAiKi6YWBERFQCxWIy5c+eiefPmWLp0qXKamEQiURmhyYqbmxvu3buXY5k9e/YgOTkZK1asUFnMAgAeP36MqVOn4sKFC2jcuLF6J/KB3bt3Q1dXF8eOHVN5n9S6desyxa9QKPDgwQNUr179k44ll8uRkJCQ7X5nZ2cA6efq6uqq3J6amooXL17k2scf8vPzQ/PmzbFmzRqV7W/fvs3UtwXh6dOnmbY9efIE+vr6sLKyynM7bm5uuHLlCtLS0rJdqMPZ2RkBAQGIj49XGbV69OiRcj8RERUOPmNFRFRAfHx8ULduXSxatAjGxsbw8fHBqlWrEB4enqnsh88Tde/eHXfu3MHevXszlcsYOdi8eTNcXV0xatQo9OjRQ+UzadIkGBoaYsuWLQV6PmKxGCKRSGWqXFBQEPz9/VXKdenSBVpaWpg1a1amEZ+8jHycPn0aCQkJqFatWrZlfH19oaOjg8WLF6u0uWbNGsTFxamsUJgbsVicKa5du3Ypn3kraJcuXVJ5diskJAT79u3DZ599lq93dXXv3h1RUVFYunRppn0Z59OuXTvI5fJMZf744w+IRCK0bdv2E8+CiIhywxErIqICNHnyZPTs2RPr16/HsmXL0LhxY1SpUgUjRoyAq6sr3rx5g0uXLiE0NFT53qTJkyfDz88PPXv2xNChQ1GrVi3ExMRg//79WLlyJaysrHD69OlMCxJkkEqlaN26NXbt2oXFixfnednx3LRv3x4LFy5EmzZt0K9fP0RERGDZsmVwd3fH3bt3leXc3d0xZcoUzJ49G02aNEG3bt0glUpx7do12NvbY+7cucqycXFx2Lx5MwBAJpMpl0zPWM48O1ZWVvjhhx8wc+ZMtGnTBp06dcLjx4+xfPly1KlTJ9NLh3PSoUMHzJo1C0OGDEHDhg3xzz//YMuWLSojYQXJ29sbrVu3VlluHUhfoj4/Bg4ciI0bN+Kbb77B1atX0aRJEyQmJiIgIABjxoxB586d0bFjRzRv3hxTpkxBUFAQqlWrhuPHj2Pfvn2YMGGCykIVRERUwDS1HCERUUmVsTT2tWvXMu2Ty+WCm5ub4ObmJshkMuHZs2fCwIEDBVtbW0EikQgODg5Chw4dBD8/P5V60dHRwrhx4wQHBwdBR0dHcHR0FAYNGiRERUUJv//+uwBAOHnyZLYxrV+/XgAg7Nu3T+1z+NCaNWsEDw8PQSqVChUrVhTWrVsnTJ8+Xcjqfx9r164VatSoIUilUsHMzExo1qyZcOLECeX+j5dbF4lEgrm5udCpUyfhxo0bWcb34fLjgpC+vHrFihUFiUQi2NjYCKNHjxZiY2PzdM4ZkpOThYkTJwp2dnaCnp6e0KhRI+HSpUuZljfPWG59165dWcb2cd9l9EtkZKRyGwBh7NixwubNm5X9WKNGDeH06dO5nu/H8QhC+vL3U6ZMEcqXLy9IJBLB1tZW6NGjh/Ds2TNlmfj4eOHrr78W7O3tBYlEInh4eAjz589XWfr+w9g+5uzsLAwaNCiHHiQioqyIBIFPqBIRERUGkUiEsWPHZjl9j4iIShc+Y0VERERERKQmPmNFRFSKJCQk5Li6HpD+vFJ+Fk0oKZKSkhAXF5djGXNzc+jo6BRRREREVJYwsSIiKkUWLFiQ66IIL168gIuLS9EEVIR27NiBIUOG5Fjm9OnT8PHxKZqAiIioTOEzVkREpcjz58/x/PnzHMs0btwYurq6RRRR0QkPD8f9+/dzLFOrVi2YmZkVUURERFSWMLEiIiIiIiJSExevICIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUhMTKyIiIiIiIjUxsSIiIiIiIlITEysiIiIiIiI1MbEiIiIiIiJSExMrIiIiIiIiNTGxIiIiIiIiUpO2pgMgIiIiIqK8UygUePnyJcLCwpCWlqbpcDRGT08Prq6usLKy0nQoAJhYERERERGVGMHBwfDz80NCQgJ0dCSQSnU0HZJGCIKApKRkyOUK2Nvbo0+fPjAyMtJoTCJBEASNRkBERERERLl6/fo11q5dC3s7S7RoURcODjYQiUSaDktjZDIZnj0LxZGj5yGV6mLEiJHQ0dFcoslnrIiIiIiISoBr165BX0+Kvn3bwtHRtkwnVQCgra2NChVc0K9fO0RFRePJkycajYeJFRERERFRCfD48WNUquwGiUSi6VCKFWsrc9jZWeHx48cajYOJFRERERFRMadQKJCYmAhLC1NNh1IsWVqY4t27dxqNgYkVEREREVExp1AoAABa4qxv34cM/QpVq/kUYUQF5+3bOIi17bB+w45PbkMs1oJcLi/AqPKPiRUREREREZGamFgREREREVG2kpKSNB1CicDEioiIiIiolDhy5CSqVvOBvoEL6tT9DJcv31Du27hpJ5o27QRLKy9YWFZEixbdcPXqLZX6M2cugLGJG65evYVGjTpA38AFy5evBwA8fPgE3XsMhaWVFwyNyqNGzZbYtn2vsm5ycjImTpwOR6fq0DdwQc1avtjrfzhTjH+t3gxXtzowNCqPVq16IjDwRZbnsn7DDlSv0QL6Bi5wKlcDU6fO1fh0v5wwsSIiIiIiKgXCwyMwbvwPmDhxDLZvXwWpjhRt2/VFREQUACA4KBT9B/TEju3/w+ZNy+BUzgE+zbviyZNnKu2kpqah/4Ax+Pzz7jh0cAtatWqGp0+fo1HjjggMfIFFi2bDf+8GDB7UGyEvw5T1+g8Yi//9tQmTJ43Bnt1r4eXliZ49h2P/gWPKMgcPnsCoUZPh49MIu/3WokWLxujdZ2Smc/njj5UYOXIiPmvlg33+G/Dt5LFYsnQNpk79tZB6T33amg6AiIiIiIjUFxMTix3b/4cWLRoDAJo1bQBnl1pYtGgV5syZgmnTvlGWVSgUaNWqGa5du4UNG3bgl19+VO5LS0vD7Nnfo3evzspt/QeMgY6OBOfO7oexsREAwNe3qXL/3bsPsHfvYSxfPg9fjBwIAGjTpgWCg0Iwe/bv6NSxNQBgzpxFaNK4HtauWQQAaN26OZKTU/DzL38o24qPT8CMmQswedIYZVytWjWDREeCSZNmYNKk0bCwMC/IrisQHLEiIiIiIioFTEyMlUlVxveWLZsop/s9fPgE3boPgZ19FUh0HCDVdcLjx8/w5OnzTG21b+er8v3UqfPo3r2DMqn62PnzVwAAPXt0VNneq1cn3Lp1D4mJ7yGXy3Hj5l106dJWpUz37h1Uvl+8eA0JCYno0aMjZDKZ8uPbsimSkpJx796jPPZI0eKIFRERERFRKWBlZZFpm42NFR49eor4+AS0adsXVlbmWLBgBpzLOUJXV4qRX0xCcnKKSh19fT0YGhqobIuOjoW9nU22x46NfQuJRAJzczOV7dY2VhAEIX1JdbEYMpkMVtaWmWL8UFR0DACgdp3PsjxWSOirbOPQJCZWRERERESlQGRkdKZtb95Ews7WBpcuXUdo6Cvs37cR1apVVu6Pi3sHBwc7lToikShTOxYWZngV/ibbY5ubmyEtLQ2xsW9hZmaq3B7xJhIikQimpibQ1ZVCW1sbkf8+8/VhjCpt/Vvfz28NnBztMx2rfPly2cahSZwKSERERERUCsTFvcOpU+dVvp88eQ5169ZAUnIyAEBHR6Lcf/HiNQQFheSp7ZYtm2D37oOIj0/Icn+jRnUBALv8Dqhs9/M7gBo1vGFgoA+xWIyaNarA3/+ISpnduw+qfG/QoDb09fUQFhqO2rWrZ/oUx+erAI5YERERERGVCubmZhgx8htMnz4JpqYm+G3eUgiCgK++Sl91z9DQAOPH/4hvvx2HsFevMXPm/EyjVdn5adpEHDoUgKbNOmPSpDGws7XBw4dP8P59EiZPHouqVSuha9d2mDRpBpKTkuHp6YYtW3fj4qXr2LtnvbKdH378Cl27DsbQYRPQu1dn3Lx5F5u3+Kkcy9TUBDNnfIvvvv8ZoaHhaNasAcRiMZ6/CMb+/cfgt2s19PX1C6zfCgpHrIiIiIiISgE7O2ss/nMOfvttKXr3HonklGQcObwNNjZWsLGxwo7t/0NEZBS6dhuCxYv/worlv8HdzSVPbXt4uOL8uf1wdnbCuHE/oHOXgVi7bhvKOTsqy2zauBTDh32Oeb8tRdduQ3Dv3iPs3PkXOnb871mpTh1bY/nyeTh16hy6dR+KEyf+xratqzId75tvRmHNmj9w5swF9Ow1HL37jMTq1ZtRp3Z16OjoqN1XhUEkCIKg6SCIiIiIiCh7MpkMv/zyCzp3bo6qVTw1HU6xc+DAGURGJWD48OEai4EjVkRERERERGpiYkVEREREVFJwrlmWikO3MLEiIiIiIirmxGIxtLS0kJKSqulQiqWUlFSNP3vFxIqIiIiIqJgTiUSws7PDi6AwTYdS7MjlcgQHh8PBwUGjcTCxIiIiIiIqASpXroynT1/ixYtQTYdSrFy4eBtJScmoVKmSRuPgqoBERERERCWATCbD9u3bERQUBA+PcnAt7whdPSlEmg5MAxSCgIT493j8OAgvQ8Lh4+ODZs2aaTQmJlZERERERCWETCbDlStXcP/+fYSHh2s6HI3S0tKCq6srqlWrBm9vb02Hw8SKiIiIiKgkUigUSEtL09jxe/fujR07dmjk2CKRCBKJBCJR8Rmv09Z0AERERERElH9aWlqQSqUaO75CodDo8YsbLl5BRERERESkJiZWREREREREauJUQCIiIiKiMuTt27cIDAxEYmIi1Fluwc7ODmfOnCm4wDRALBbDwsIC7u7uar9gmItXEBERERGVAampqdi1axcCAwPTn8/S04OW6NMnsMnkcmiLxQUYYdGTyWRISU6CRCJB8+bN0aBBg09uiyNWRERERESlnCAI2Lp1K16Fh6NZuy5w8agIHS48AQB4FxuDf65fxvHjxyGRSFC7du1PaofPWBERERERlXKvXr1CcHAwmnfoBk/vakyqPmBsZo6Gvm3hWrEyLl669MnTI5lYERERERGVco8ePYKunj6cXD00HUqxJBKJ4OldDbExMYiKivqkNphYERERERGVcvHx8TAxM4eWFm//s2NqYQUAePfu3SfVZ88SEREREZVyCoUCWtksNHF0vz/Wr1pexBFlLSQ4CA76Ihzc65evehfPnoGDvgh3blxXbpv1wyQ0r1UZntZGqGBjjHaN62Dfru3ZtiH+t38UCsUnxc7FK4iIiIiIyrCjB/1x9+Z1DP5ijKZDgbWtHfafuQRXd8981atSvSb2n7kEj4peym2JCQnoN2QE3D0rQiQS4dBeP4wZ1BcKhQJde/cr6NCZWBERERERUcFISkqCnp7eJ9eXSqWoVbd+vusZGRtnqjdvyUqV7z6tWuPJowfYuXl9oSRWnApIRERERFRGTRg5GLs2b8DjB/fhoC+Cg74IE0YOBgBcv3IJPdu2gLulASrammDs4H6IiohQ1s2Ytrdj03pMHjMClR0t0KFpXQCAg74Iy36fh1+nT0FVZ2t42Zni5ynfQhAEnDt9Eq3qVYeHlSF6tWuJsNCQTG1+OBWwXkUXTPl6HNavXIa6FZxR0dYEQ3t1QXRkpLJMVlMBs2JmboG01NSC6LpMOGJFRERERFRGTfh+GqIjI/HsySMsWbcFAGBhaZWeVLX2QYvW7bBi4w68f5+I32ZOxZBenXHgzCWVNn796Qe0bNMey9dvU3k+ad3KpWjQ1AeLV2/CrWtXsODn6ZDL5Th36gTGfzsFOhIdTJv0JSaNHoZtB47nGOfxQ/vx4tlT/PLHMsRER2Hmd19j6sTxWLEx+2emgPT3d8nlciQmJODE4QM4e/I4Fq/d/Im9lTMmVkREREREZZSLqxssrKwQFhKsMpVu4qihqFqzNlZv3wORSAQA8KpcBS1qe+Pk0cNo2aadsmzlqtWxYMXqTG3b2tljyZpNANKn4R0/tB9/LfkDp2/cVz4L9fpVGKZOHI+4t29hYmqabZyCIGDdrv2Q/vv+rdDgICyZPyd9UY4cVjo8d/ok+nZoBQDQ1tbGzwuXokPXHnnsnfzhVEAiIiIiIlJKev8e1y5dQIduPSGXyyGTySCTyeDq4Ql7RyfcuXFNpXzLNu2zbKdJi1Yq3109PGFjZ6+ywISrR/oiFeFhoTnG1KBJM2VSBQAeXpWQlpamMjUxKzXr1MPhc9ew/VAAho+bgGkTx2Pb+jU51vlUHLEiIiIiIiKlt7GxkMvlmPHt15jx7deZ9r/64JkoALC0scmynY9HoCQ6OlluA4CU5OQcYzI2Ua2nI/m3XkrO9QyNjFCtVm0AQJPmLSGTyTDz+2/Qa8Bg5fLqBYWJFRERERERKZmYmkIkEmH85B/RpmOXTPvNLS1VvmdMFSwJqtaohdVLFyE6MhLWtrYF2jYTKyIiIiKiMkxHoqMyYqRvYIBa9Rog8PFDVJvxswYjK3hXL56HkbFxpuSwIDCxIiIiIiIqw9wremH7xrXw37kN5d08YG5pialz5qN32xYYNaA3OvfoAxMzM4SHheLsqRPoPWAIGjb10XTYOXrwz13MmfodOnTrCUdnF7xPSEDAkYPYun41fpg1F9raBZ8GMbEiIiIiIirD+g4ahtvXr2LqxPGIjY5Gz/6DsOh/67E34DwW/Dwd34wagtTUVNg5OKKxT0u4uLprOuRcWVnbwNjUFH/MnYXIN69hZGICd8+KWLN9L1p37FwoxxQJgiAUSstERERERFQs7NmzB1Fv36FD38GaDqXYep8Qjy3LF6Jfv37w8PDId30ut05ERERERKQmJlZERERERGUB56nlSN15fEysiIiIiIhKOYlEgtTUnN/5VNal/vtOLJ1/362VX0ysiIiIiIhKOXt7e8RERiApMVHToRRbYcHPoaWlBWtr60+qz8SKiIiIiKiU8/LyAgBcPRsArl2XWUL8O9y7fhmurm7Q09P7pDa4KiARERERURlw584d+Pv7w8LaFuUreMHIxAxaWmV3nEUAIJelITI8DM8fPYCOjgSDBw2CmZnZJ7XHxIqIiIiIqIx49uwZbty4icDAp0hLS9N0OMWCsYkJKnl5oX79+jAxMfnkdphYERERERGVMYIgIC0tTa1pgb1798aOHTvUiqMg2lCHWCyGtrZ2gbRVMK0QEREREVGJIRKJPnn1uwwKhQJSqVTjbRQXZXdSJRERERERUQHJdcRKEAQkJSVBLpcXRTyUDZFIBF1d3QIbqiQiIiKi4k0mkyE5ObnYruInkUgQHx+v8TYKm5aWFvT09HJd6CPbZ6xiYmJw4cIFPHr0EO/fJxVKkJQ/IpEIruXLo1bt2solM4mIiIiodHn06BGuX7+OFy9eQKFQaDocQvpLgz09PdGgQQPY29tnWSbLxCo6OhobNqwHBAFVKrjBwc4aEm1xYcdLOVAoBLx9F48HT17g5avXaNu2LerWravpsIiIiIioAN24cQMHDx6Eg509KrpXgKmxcZleEr04kMnliIyOwoPHDxGfmIDPP/8czs7OmcplmVht2bwZMdGRGNKrIwwN9IskYMobQRBw9MwlXL19H9988w2MjIw0HRIRERERFYDExET8/vvvqFa5Clr7+EIkEmk6JPpAWloaduzbjcTk9xg/fnymf59M6W9SUhKev3iBejW8mVQVQyKRCD4NakJLSwsPHz7UdDhEREREVEAePXoEAGhSrxGTqmJIIpGgYZ36iI2NxevXrzPtz5RYRUREQKFQwMXRrkgCpPzT09WFrZVFlv+gRERERFQyhYeHw9LCEgb6HNworpwdnQAgb4lVxhuYpVL11rX/FC5V6mHcpCmF0rb/waNY/tf6fNebMfd3XLxyreAD+sDg0RMgMnHI9DkacDrbOlIdCd+WTURERFSKyGQySNV8t9Sn8qxeGRO+nVgobe8/dACr1vyV73qz583BpauXCyGi/yxcsgj1fBrBprwjzJ1sUKtxPaz4a1W2KzGKxWKIxWKkpqZm2pft2t2aGHzcu3kNzExNCqVt/0NHcf3WXYwZMThf9Wb+uhCGBgZoWK9OocSVwdXFGVtWL1HZ5uXpkUMNDg8TERERUcHYuXErTE1NC6Xt/YcP4ubtW/hi2Ih81fvlt7kwNDBAg7r1CyUuAHgbF4ceXbqhslclSKW6OH32DL75YTLexb/Dd99MzrKOKJv78GLxUqSkpCTo6emhRjVvTYeiMXp6uqhfp5amwyAiIiKiMiTjPrx61WqaDkUjZk2drvK9pU9zhISFYtP2LdkmVtnJ89qN67fsgLZ5ObyJiFTZHhMTCx1LF6xauwmXrl5Hpz6DYV+hJgzs3FG9cSts2u6nUv7MuYsQmTjg0LEA9BgwAsaOFdBz0BcAMk8FzE97J06dRb9hY2Hk4Aln77r4bdFyZZnBoydgw9ZduP/wsXKa3eDRE3I9Z5GJAwBg8rTZynpnzl0EAPy+ZCXq+LSDiVNFWLtVRYdeA/Ek8FmmNlat3QRn77rQt3VDq859cOvOPYhMHLB+y45cj09EREREtHHrZhhYm+JNRITK9pjYGBjZmuOv9Wtx+doVdP+8F8pX8oC5kw3qNmuILTu2qZT/+/w56FoY4cjxo+g7uD+snO3Rb+gAAJmnAuanvYDTpzBw5FBYlrODR7VK+H3xH8oyw8d+gc3bt+LBo4fQtTCCroURho/9Itdz1rVIX/n6h+lTlfX+Pn8OALBo2WI0atkM1i4OcKpQHl379sDTwKeZ2vhr/Vp4VKsEM0drtOvWCbfv3oGuhRE2bt2c47EtzMyRmpr/R27yPGLVtUNbjPr6B+zyP4hxI4cot+/efxgA0LNLBxw/dRaN6tXBqKEDoCuV4sKVaxg2bhIUCgUG9eul0t7Ir75D/17dsHfYQIjFWb8jK/hlWJ7bG/X19xjQpzv2bl4N/0PH8N30X1DV2wttfJtj2uQJiIyKxqMnz5TT7awsLHI950sB+9HAtxPGfzEU/Xp2AQBUquAJAAh9FY5xIwfD2ckR7+ITsHLtJjRs1RlPbpyDubkZAGD/4eMY9fX3GD6wH3p0bo/b/9xHr8FZX0iBz4Ng4lQRSUnJqFKpIqZ9OwFdOrTJNUYiIiIiKt06d+iI8ZMmYM++vRg94r97yb0H9gEAunfugoDTp9Cgbn2MGDwMUqkuLl29jFFfjYVCocCAvp+rtDf26y/Rt2dv7Ni4Ndv78JchIXlub/ykCejXqw92bNyKA4cPYsrMn1Clsjc+a9kKP0z6DlHRUXj89CnWr1wNALC0tMz1nP8+ehLN2rTEmBGj0Lt7TwCAV4WKAICwV68wavhIlHMqh/j4d/hr/Vr4tPXFP1dvwdzMHABw8MghjJ/4FYYMGIRunbrgzj938fmwQdkeTyaTISkpCecvXcCWHdsw5dvvc43xY3lOrExMjNGuVQts8/NXSay2+fnjsxZNYW5uhj49Oiu3C4KApo3qIzQsHKvWbc6UCHVq2wrzZuW8UEV+2uveqR1m/JCeZbf0aYJDx07Cz/8Q2vg2h5urC6wsLRAcEpav6XYZZcs5OmSq98fcmcqf5XI5WjVvAmv3avDbdwgjh/QHAPw8/0+0aNoIfy2ZDwBo7euDNFkapv08X6WtGlW9UadmdVSu6Im3ce+wYs1GdP18GHZtWIUeXTrkOV4iIiIiKn1MjE3Qxvcz7NizSyWx2rnbD77NW8DczBy9uvVQbhcEAU0aNkLYqzCs2bA2UyLUvk07/DJjdo7HzE97XTt2wrTvfgQAtGjmgyMnjmHPfn981rIV3Mq7wtLCEi9DQlCvTt08n3NGWSdHx0z15v/yq/JnuVyOlj4t4FTBFXv2+2P4oKEAgF9/nw+fJs2wYtFSAECrFr5IS5Nh5tzM5/3s+TNUrlNd+f37id/iy9Hj8hxrhnw9Y9W3R2f0HjIaL0PCUM7JAeGv3+DvC5excdWfAIDY2LeYPvd37Dt8DGGvXkMulwMALP4dwflQ+9Ytcz1eftr7rEVT5c8ikQheFTwQ+io8P6eXL5ev3cC0n+fj5p1/EBP7Vrn9SeBzAOn/yLfu3sOCn6ep1OvcrnWmxOqr0cNVvndq9xkatuqEn+YsYGJFREREROjVvSf6DxuEl6EhKOfohPDXr3Hu4nmsWf4/AEDs21jM/nUODhw5hFfhrz64bzbP1Fbbz1rnerz8tNfS57/7epFIhIqeFRD26tUnnWdeXLl2FTPn/ozbd28jJjZWuT3wWSCA9Pvw2//cwa+zflGp17Fd+ywTK0cHR1wI+BsJiYm4cPkiFvy5EFpaWvjp+/ytVp7nZ6wAoEMbXxgY6GP77vRhx517D0BXV4ou7dOnrA0e8zW2+flj0vhROL53K66dPoyh/fsgOSUlU1s2Vla5Hi8/7ZmaqK4mqKMjybJcQXgZEobPuvaDXC7HqkXzcOG4P66dPgxrK0vlMSOjoiGTyWBlqTrl0Noq96FPLS0tdO/UHg8fP0VSUlKhnAMRERERlRztPmsDA30D7NqTvt7A7n17oKuri07t0v8IP2LsKOzcswtfj/0SB/324ULA3xj0+YAs74etraxzPV5+2st0Hy6RIDkl+VNOM1cvQ0PQoUcXyOVyLF24GKePnMCFgL9hbWWF5OSM+/AoyGQyWFqo3ndbWWadf0ilUtSqURPNGjfBj5O+w6yp0zFv4Xy8fvMmX7Hla8RKT08PXdq3xvbd+/DthDHYvnsfOrZpBQMDfSQnJ+Pg0QAsnDMd478YqqyjWK3Isq3c3iad3/aK0tGA00hISMSezath+u/y8DKZTGXkysrSAtra2oiMilapGxEZVZShEhEREVEpoKenh47tOmDX3t2Y+OXX2LXHD+1bt4WBgQGSk5Nx+PhR/PbzXIwZOUpZR7Hm0+/D89NeUTp+8gQSEhOwY+MWmJqYAsi4D/9v5MrK0hLa2tqIila9746MUl2ELzs1qlWHXC5H8Mtg2NrY5Dm2fI1YAUDfHl1w6+49HAs4g8vXbqJvjy4AgJSUVCgUCuhIJMqy8fEJ2H/4eH4PUSjt6Uh0lFlsfkiyyLiTkpMhEokg+SC2nXsPQCaTKb+LxWLUqOqNfYeOqdT1P3Q012MqFArs8j+Iyl4VoKenl++YiYiIiKj06d29B27fvYMTpwJw5fo15XNQKakp/943//dy4fj4eBw6eviTjlPQ7eno6HzSTDKJRJLp/j054z5c+7/7cD//PZnuw6tXqYYDhw+p1N1/+GCejnvx8iWIRCK4OLvkK958v8eqVfOmsDA3w9BxE2FqYoK2rZoDSF/cok7N6vh10TLlaM2vfyyFibExIqLyP0pT0O15VXDH2s3bsc3PHx6u5WFpYQ4XZ6c81dt36DiaNKgHA319VPBwQ4umjQAAQ8Z8jS+G9Mf9R0/w+9JVmYZBp07+Cp37DsGI8ZPRs0sH3Lp7Dxu2pg/famml57TBL0MxaPQE9O3eGe6uLoh9G4cVazbi+q072L0p/2+oJiIiIqLSqaVPC1iYm+OL8WNgamKK1r6fAUhf3KJ2jVqY/+dCWFpaQlssxoI/F8LY2CTPozQfKuj2KnpWwIYtm7Bj9y64u7rBwsICLuWc81Tv4JFDaNSgIQz09eHp7gGfJs0AACPHj8awQUPx8NFDLFq+RDl6leH7iZPRo38fjJ4wDt06d8Wdu3eweftWAP/dh8e9i0Pn3t3Rr2cfuJZ3hUyWhrMXzmHpqhUYPmgobKxznzL5oXyPWEkkEvTo3B6vwl+je6d20NH5L5Pdunop3Mu7YNDoCfjyu2no0bkDBvbtkUNrOSvI9oYN6IueXTpg/OSpqNO8HWb8+nue6i1bMAcKhQJte/RHnebtcOP2XVSp7IX1K/7Ajdv/oEPvwdjm5w+/Df+DiYmRSt1O7T7DioVzcezUGXTuNxRHAk5jxcK5AAATY2MAgJGhAUyMjfDzgj/RrudADBn7DRSCAkf8NqNrx7afdK5EREREVPpIJBJ07dQFr16Ho0vHTir34Rv+twZu5V0xfOwX+OaHb9G1Uxd83rvvJx+rINsb/PlAdOvcFd98PwmNfJvh53lz8lRv0W+/QyEo0Ll3NzTybYabd27Du1Jl/LV0JW7euY1u/Xpi555d2LZuE4z/vbfO0KFteyxZsAgnTp1Ez/59cOzkCSyen/5+rYz7cF2pLjzc3PHniqXoOaAPho4egXMXLmDJgkVY9FvecoUPiQRBED7cEBgYiC1btuDr4X1hbGSY7wYpZ2s2bsPw8ZPw4u7lPI2YZWej32EYmJihe/fuBRgdEREREWmKv78/oiOj0L97H02HUiqt27wBo78ah0e37uVpxCw7C5b/Cd9WvqhXr57K9nxPBaS8i4mJxcx5f6BF00YwMjTAtZt38Mvvi9G5fWu1kioiIiIiIspeTGwMfvntV/g0aQpDQyPcuHUD8xYuQMe27dVKqnJSphOrDx9y+5hIJMr2TdR5JZFI8OxFELbu2ou3ce9gZWmBAb27Y97M/K2JT0RERERUmhT6fbi2BM+DnmPH7p14GxcHKwtL9OvVB79Mn6VWuzkps4lVUHAIyletn+3+Zo0b4MwhP7WOYWRkiIM7N6rVBhERERFRaRL0MhgVa3hnu79Jo8Y4sf+IWscwMjLC3m3q3cvnV6bEKmNde4VCyFS4NLG3s8G109kvGWlkZFCE0eSfQlDk+g4CIiIiIio5RCIRBIXm3xVV2Oxt7XAh4O9s9xsZFt91HgRBgEJQKFcW/FCmxMrAID2hePsuHqYfrXJXmujo6KB2zWqaDuOTCIKAt+8SYOtQTtOhEBEREVEB0dfXR1x8PARBKNV/QNfR0UGtGjU1HcYnSUhMhEKhgL6+fqZ9mVItGxsbGBkZ4f6T50USHOXfqzeRiHsXDw8PD02HQkREREQFxMPDAwmJCQgND9N0KJSNR4GPoaWlBVdX10z7MiVWIpEINWvWxPW7D3H55j2k5fBgGRUtQRAQ9joSuw6dhLm5GVxcXDQdEhEREREVkHLlysHS0hL7jx1G2OtX+OitSKRBCoUCj54+xt8Xz6NSpUrQ09PLVCbTe6yA9Bv4w4cP4/r165BItGFrZQFtsTZK8oikQpH1XMiSQqFQIPZdAuLexcPc3AwDBw6CiYmJpsMiIiIiogIUHx+PDRs2IDo6GsZGRjAxNoG4mN7DKhQCtLRyTxByKpfXNjRJJpcjOiYGSclJcHd3R+/evaGtnXkNwCwTqwzR0dF48OABoqOjc1wSsSQ4d+4cmjRpoukwPpmWlhb09fXh4eEBFxcXtZegJCIiIqLiSaFQICgoCE+ePMH79++hKKYLWuT1/jqnciXhHl0sFsPExAReXl6wtbXN9vm3HBOr0qRTp07Yv3+/psMgIiIiIioV8np/nVO50nSPXjzHFYmIiIiIiEoQJlZERERERERqyvzUFRERERERqe3t27cIDAxEYmJiqVrhT0tLC6ampnzm/yNMrIiIiIiIClBKSgp2+e3Cs8Bn0NLSglRPr0SvTv0xuVyG5PdJqFa9Gk6cOAFfX99S/ULjvCoTidX79+8hl8s1HQYRERERlXKCIGDr1q14/eYNfLp0gHNFD+hIpZoOq8AlvovHo5u3cfHvCxCLxWjRokWW5WJiYkrVaF1OykRi1aB+PQQHB2s6DCIiIiIq5cLCwvDy5Uu07tsD5TzdNR1OoTEwNkItnyaQpclw9epVNG3aNNO7neLj42FhYQEPDw8NRVm0Ss+YZA7u/nMPce/iNR0GEREREZVyjx49gp6BPhzdXTUdSpHwqOaNlJQUBAUFZdqXlJQEAHj9+nURR6UZZSKxIiIiIiIqCvHx8TCxMC9Vz1TlxNTSAgDw7t27bMuUlUdyysa/OBERERFREVAoFNAqQ6vlaWlpQSQSQaFQZFuGiRUREREREZGamFgRERERERF9IOO5qfyQyWSFEEnxU6YSq7Lyj0pERERExc/j+w8woF1nVLawh5u+GZpUqILlv/0OAJgweDhaeNfEqSPH0MK7Jlx1TdCmVgPcuHxFpY1dGzejS+PmqGxuh0pmtujh0wq3rl7LdKynDx9heLfeqGxuBzd9M/hWqwP/bTuU+wVBwMoFf6CxpzfKS43RwLUi/vfHYpU2fp8xGx6GFrh19Ro6NmgGV10TbFi2shB6pnQoE8utZ3j//j2MjY01HQYRERERlUGDO3aDpY0Nfl+zEkYmxggKfIbw0DDl/jfhr/HjmC/xzYypMDUzw9JfF+Dz1h1x/uk9WFpbAwBCg4LRY+DncHZzRVpqGvy37UD3pr44cfc63DzTlzV//jQQnRo0g72TI2Yt/h1WtjZ4fO8Bwl6GKI/101cTsXX1Onw55TvUqFcHNy5expzvpkBXTw8DR41QlktLTcW4foMw4usv8f2cmTCzsCii3ip5ylRilZiYyMSKiIiIiIpcTFQUXr4Iwsw/f8dnHdsDABo191Ep8zYmBqt2bUHjFs0BAPWbNUEdJ3f89cdi/DD3ZwDA1z9NUZZXKBRo2qolbl+9jp3rN+KHObMBAAtnzIZERwf+F07D6N9736a+LZX1gp49w7qlK/DryiXoP3K4cn/S+yT8MfMX9B85TLmqYVpaGr79ZSY69+5Z8J1SypSpqYCJiYmaDoGIiIiIyiAzCws4OpfDrz9Mw84Nm/AqNDRTGWMTE2VSlfG9iW8L3Lzy31S/pw8fYVjXXqhmUw5OYn04Swzx7PETPH8SqCxz/uQZtO/RVZlUfexcwCkAQLvuXSGTyZSfxr7NEfH6NV6FhKiU923fVq1zLyvKVGKVlpam6RCIiIiIqAwSiUTYevwQ3L0qYsrYCajj5I62tRvi8tlzyjLmVpaZ6lnaWCMiPP0Fuwnx8ej7WXuEBr/E9IXzsPfcSRy+dgGVqlVFSnKysk5sdDRs7O2yjSUmKhqCIKCKpQOcJYbKT99W6SNpr0L+S/r09PVhYGio9vmXBWVqKqC+vr6mQyAiIiKiMsrN0wP/27UVaWlpuH7xEn798ScM7tgdN8KeAwBiIqMy1Yl6EwFrO1sAwI1LlxEeGoYNB/eicrWqyjLxcXGwc3RQfjezsMCbV+HZxmFqbg6RSIS9509BR0cnc5wVPJU/i0Si/J9oGVWmRqwMDAw0HQIRERERlXESiQQNmjXF2O8nI/7dO7z+Nwl6FxeH86dOK8u9i4vDuYBTqFmvDgAgOSl9VOrDZOjaxUsICQpWab+Jb3Mc8tuLhPj4LI/fuGX6dMPY6BhUq10r08fQyKjgTrYM4YgVEREREVEhe3D3H8ya+B069e4BZzdXxMe9w9K58+Hk4gwXN1cA6SNJk4aNwsSZ02Biaoqlvy6AIAgYPmE8AKBm/bowMDTEj2O/wrjvJ+F12CssmD4btg4OKsf6evpUBBw8gi6NW2DMt9/A2s4WTx88QtL79xjz7US4eXpg8NhR+GrAUIya/DVq1KsDWZoMz588xcXTf2Ot/64i75/SoEwlVnp6epoOgYiIiIjKIGtbG1jZ2mDp3Pl4HfYKRiYmqNukERZvXgexWAwAsLGzxY/zfsHPk39A8LPn8KxcCVuOHYCVjQ0AwMrGBqt2bcXsSd9jaOeeKO/pgXmrlmH5vAUqx3L1cMe+i2cw94dp+HHMV5DJZHD19MDY7ycpy8xevBBuFTyxedVqLJo1B/qGhnCr4IkOPbsVXaeUMiJBEARNB1HYMuaGloFTJSIiIiIN2r17N2IS49F+YN981ZsweDjuXr+JU/duFlJkhWf1rHlo164dateurbI9IiICNjY20NHRQUpKSpZ1O3XqhP379xdFmIWuTD1jRURERERERausrHPAxIqIiIiIqCCVoVlSeZkRVlYSqzL1jBURERERUWGSSCRIzWbaW04WrV9dCNEUPllaGgRByHLZ9gxlZQE5jlgRERERERUQe3t7RL+OQFLie02HUiTCngcBSD/v7FhbWxdRNJpVJhKrZcuWYdWqVZoOg4iIiIhKOS8vLwDAtZNnSv3CaSnJybh19gKsra1haWmZab+FhQVGjhyJhQsXaiC6olcmVgUkIiIiIioqt2/fxr59+2BpawOXShVgZGoKLa3SM54hl8kQ/SYCT+/eA+QKDBw4EHZ2dp/UVmlaFZDPWBERERERFaDq1avD0NAQN2/exJ1zl5CWlqbpkAqcgYEBQoKCMX36dFhZWWk6nGKBiRURERERUQFzd3eHu7s7BEFA2r8LPBS23r17Y8eOHYV+HLFYDG1tbXTq1IlJ1QeYWBERERERFRKRSJTjinkFSaFQQCqVFsmxKLPSM9mTiIiIiIhIQ5hYERERERERqYmJFRERERERkZqYWBEREREREampWC9eERYWhqSkJE2HUaxJpVI4OTnlqawgCAgODoZMJivkqIiIiIjKDmdnZ0gkkjyVjYiIwLt37woljsTERAQGBuaprL6+Puzt7fNUVqFQ4MWLF8qVDc3NzWFubp5l2fycn7GxcZ7KlRhCMQaAnzx8hgwZIqSkpOTan1u3btV4rPzwww8//PDDDz+l7eNdtZoQHByc671YdHS0oK2trfF4Mz7fffedIJfLc417wYIFKvV0daXCtWvXhI4dO6qUi4yMFMRicZ6Pr6WlJVSqVElQKBS5xlASFOsRKwBYPgqwNtF0FMXXo1Bg1uYNeBb4BLv3+MPS0jLbsrGxsdASi9F09q4ijJCIiIio9JIlJeDOX1NRq3Yd7N/njwYNGmRbNiEhIX3mUK+mgIttEUaZhcBXmPfbb3jw8CG2btkCQ0PDbIvGxsbC2koPa5ZVBABMn/MCvXv3gKenl0q5hIQEyOVyoOkQwMY91xAUz6/jwY29GDZsGFauXFlky9IXlmKfWNV2AxyzzxXKvIYVgSrOCgxbehl169TEgYNHULly5WzLi0RasK7aqAgjJCIiIirdzCvWwuU5Q9HMxwdr16xB//79c67gZAVUzNujHIWmohPgaIlDfx1B/YYNcfjgQZQrVy7b4nq6YjRpaAYAWLtMF03b3EBKcioEQYBIJFItbO0KOFXJPQanKoCVMzZsWoYnTwPhv3dPjoMExV2pWrziyE1g/SlNR5EuJAqwHwIcvJa/ehcfpde78+K/bd1/Td/28edpePr+Oh7A4Wly6MpfoUH9ujh06FDBnQgRERER5UjXxBJNft4Fx6bdMGDAAPzwww9QKBSaDit31d2g+KEPHr0OQY3atXDp0qU8VXNx1sPi+Z4IexWO//3vf+rFUKkFFD1+xuXb91Czdh3cv39fvfY0qFQlVsduAhuKSWJlbQIcmAo08sq97IeqOKfX8/joWcI6HunbP/w4fZDQO1oC+36Qo4FHEjp27IiFCxcqHzAkIiIiosIllkhR+6tFqDZ0BubNm4eu3bojISFB02HlztES8il98dZcD019mmHTpk15qtalgzWGDXTAV199ibt376oXg70X5H3m41WSCHXr1y+xgwSlKrEqSEmp6tWXSoBaboBZ9tNVs2Skl15PX6q63UQ/ffuHH92PFp8x1APWjhMwpq2AiRMnYtiwYUhNVfNEiIiIiChPRCIRKnQbjUY/bcLREwFo2KgxXr58qemwcmesD8XE7pDVrYCBAwfmecTtl5/c4eGmi169CiCJNLaGvNevSLKtXGIHCUpNYjVhNbDzAvA47L+pchNWp++7Hgj0nAe4fQFUGAOMWQlEfbAKZMa0vR3ngUnrgMrjgPaz0vfZDwGWHgJ+3Q1U+RKoOAaYvRMQBODcA8D3J8B9FNDrNyAsOnObH04FrDsJ+HETsO4kUGdSeixDFgPRH8SS1VTA/NDSAqb0BP4cDmzZvAGtfFsgKirq0xojIioEz45sxMEhtbC7uwv+ntoTsc/+wc4ONngRsF1Z5kXAdhwb5wO/ruVwYGA1/LNxDhRyucr+nR1sEPvsH5yd3he7u7vg8Ij6CDq5M9PxXl07gYBv2mB3N2fs61cJN5Z9C1lyYpGcKxGVTfZ1WqH5bwcRFBGL2nXq5nmKnUZpi4EhnwG9muHXefPQtVu3XJMlXV0x1q3wQmhIMMaOHaN+DDp6EDr+AKF2txI5SFB6EqtOQMuqgLPVf1PlJnRKT6p6zAOM9IGVo4HfBqUnLUMWZ25jrl96wrRsFDCt93/b151MT5qWjABGtgZWHAFm7QBmbAPGt0/f/uw1MHFd7nEevw0cvwXM6Q/M6gdcfgxM2ZJ7vUuP0xPD8iOAbr+m18tJz0bArskKPLiTvqhFSZ6vSkSlR9iVo7ixbDJsajRDox/Xwbp6U1z6dYRKmcd7V+L64m9gW7M5Gv+0CRV6jMPTA6txb9OcTO1dWTAmva2pG2DqVgVXF32JdyFPlPtDzh/AhdkDYeLihYZT1qHqkGkIvXQI1/78utDPlYjKNhMXLzT//QhEVi7wad4cW7bk4YZP00QioE1tYHxnHDx+FPUbNsx1xM3DzQAL53pg48ZN2L17dwHEoAU0GQS0mYANmzajeYuWiIyMVL/dIlDsVwXMKxdrwMIICI1OnyaX4Zu1QFUXYM249GsFALwcgebTgJN3gJbV/itbuRzw+9DMbduaAUtGpv/sUyU9OfrfceDMz/89CxUeC0zdAsS9T5+2lx1BANZ/lT5VEEgf2VpyEFAo0kebslK/AtCjIeBqC7yOBVYeBXrPB3Z/D9TOYSXLjEUtBi1OX9Sid59+2RcmIioCD7f/AeuqjVHny4UAANtazSHI0nBv8zwAQNr7BNzf+hsqdB+LqoOmpJep0Qxa2jq4s2Y6KnQbC6nxfy+ldO8wFO7thwAALL1qI/zaCYReOIhKfb6BIAi4s3YmnJp0Rp0v/1DW0TW3wbkZ/VCpzzcwca5YVKdORGVQxqIWN5d9i/79+2PkyJGaDilvMha1WLIPNWrXQtvPWiOnSXm9u9vi7MVYTJs2peBiqNQCClM7XDkwFzVq1cYev12oW7duwbVfCErNiFVW3qcA154CHesAcgUgk6d/XG0Be3Pg9kfT7VpWzbqdppVUv7vaALamqgtMuP77KoLwmJxjalDhv6QKADztgTQ5EBWffZ3JXYG+TYF6nkDneukJlY0psGh/zscC/lvUop7be6xZvRpyuSz3SkREhUAhlyP2+T3Y12utst2+fhvlz9EPr0GWlAinxp2gkMuUH5vqTSFPSUJc8COVujY1fJQ/a+sawMDaCe+j0pdMjQ97hvcRIZnasvJuAJFIC7GBdwrtXImIMmQsalF16HT1V9ArSv8uahFjLMGWLVuQlpbzlLzfZnvC3lYLYjEAeVrBxGDvBXnfBQhLFFCvfvbvBysuSs2IVVbi3qcnVNO3pX8+9uqjJMgqmxcRG380AqWjnfU2AEjJ5Tr6uJ4kj/U+pC9NH2k7dD1v5Q31gEldgLP3AZmiZD0ESESlR8q7aAhyGaQmFirbdU0sVcoAwImvfLNsIynqlcp3HQNjle9a2hIo0lIAAKnv0n/JX/hlSJZtvY8My0f0RESfTiQSwbV1f7w4vhXxoU81HU7eGesDnRsCC3Of4megL0bn9tZYuDQYeP+2AGOwBup2B44uKrg2C0mpTqxM9NOn/33ZHmhTM/N+cyPV76LMRUqFw9eB8au1YGNri7DwCE2HQ0RllNTYAiKxNlLiolW2J8f9t8COjlH6yycb/rgO+lYfvXcCgIFN9i+v/JiOkSkAoMaoubCokPl/Anrmtnlui4hIHfGvXuDS7AFQxL3WdCj5c+YuRFtOwbFcOYiEnKdlXbkehz9X/Ps8lpFVwRxfEICru4ALm9GlS9eCabMQlarESqKtOvKjL01/3uppOPBdec3FVdDepwABd4DquZyTIACLDwLz9gA9e3RFw0aNMWnyt0UTJBHRR7TEYpi5euPVlaPw7PzfcwZhl44qf7aoWBtiqR6Sol/BsWE7tY5n5OgBPUt7JL4OhkeHLB6gJSIqAhF3z+Py3GFwsLXG6v370bx5c02HlDu5AthxBgi4hdFjxsDY2BjbtizNtnhsbBqGjXmIGjWq4/r1WwUTQ1oKcGIp8OhvTJ8+HdOnTy+YdgtRqUqsPOyA7eeAvZfTn4MyNwKm9UpfCv2L5UCXeoCJQfpzUGfvA72bAA2L+XPLV54Ay48AbWumvxD4zdv0xSsi44D/5bCqZVJq+tLxey9DeTGuWLGiyOImIsqKV5+vcWH2IFxb/A2cGndC7PN/EHxqBwBAJNKCjqEJvD//DnfXzcb7qHBYV2kIkZYYCa+D8erKUTT8YQ20dXNYIegDIpEI1YfPxOX5oyFLfg/7Or4Q6+rjfUQowq8FoMqgH2Hk4JZ7Q0REn+jZkY24tfIH+Pj4wG/XTsTH5/BQfXHxPhmiVYchevASS5Ytw5gxYzB16tRsiwuCgDETHyExSYJFi5agcePG6seQGAvxgTkQRwdj044d6NWrl/ptFoFSlVj1bQrcepG+Ol9sAtCrEbBoOOD/I7DAH/h6DZAqB+zNgMaV0lcSLO6sTYA0Wfp7tGIT0kfharsD8wYBNVyzrhMRBwxdIsaDUDF27NhUYi5GIir9HOq1Qc0xv+HRrj/x8sxumHvWRM0xv+HstF6QGKTPz67QbTT0LGzxxH8lAg+ugZZYGwZ2LrCv0wpaEp18Hc+pcSdIDEzwcMciXD7jBwDQt3aCba0WkJoW0FQVIqKPKOQy3Fk9HU8PrMaYMWOwaNEiSCSS4p9YvYmFeMl+6CemYs/Ro/D1zfp51w+tXBOKI8cjsW/fPjg4OKgfQ8RziA/8Ags9bRw6fw61a9dWv80iIhKK8SuNRSIRrs5PX9mO8uafYGDIEjEEiTn27T+EOnXqKPctX74cX341Ad39QzUYIRGRqufHt+D64m/Qfs21fD1DRURUHKUmxOHK/C8QcfsslixZgtGjRyv3vXz5Es7OzsDE7kBlF80FmZWHLyFeeQjOtvY4cvAQPD09lbumTp2KzRv/xJ1Lqsud37rzDp91uYnRo8fhzz//RFBQEMqXLw/0mA2Uq/bxEXL39CK0ji1ClcqVcOjA/oJJ1IpQqRqxKusOXwe+XK0Fr8re2Lf/UIm7GImo9EuJj8WDrQtgXa0xtPUMEfP0Nh7uWAT7+m2YVBFRiadcpOJdJI7mccSnWPh3kYqmPs2we5cfzMzMcq0S906GIWMeolq1apg/f756x/9gkYpuPXtiw/r10NfP27Tv4oSJVSnw8SIV6zdsLJEXIxGVflpiCRJeB+Hl33uRmhgHqYkFnFv0RNXB0zQdGhGRWj5cpOJwwBWVEZ9i66NFKjKmLOZGEARM+O4xYmJFCDi5Czo6+ZumrSKLRSpEopK5VjcTqxIuq0UqSurFSESln0TfEE2mb9F0GEREBerjRSryMuKjcVksUpFX67e8wt4Db7Bz5064uamxCFAJXaQiO8U+sfpmHaCnRhJc2gVFaCEkWjvPi1TIZWk4P2tAEURGREREVPqlJSUg8p+LKotU5GrvReBkAS1L/onEr2Kgn6LI8yIVEVFJ6DPkLgDg9NlYjBo1Cj179sy68IXNwM0DuccQ+Qzm+hIcOndWZV2AkqpYL17Ru3dvJCUlaTqMYk1HRwffffddni7GBw8eYOrUqZDJZEUQGREREVHZ0LlzZwwbNizXcmlpaRg5ciSio6NzLVvYDAwMMHPmzDxNWbx48SLmzZuHjLTB0dERCxcuhK6urkq5tLQ0jBgxAjExOb9MOIOZmRnmzJlTatYFKNaJFRERERERUUmgpekAiIiIiIiISjomVkRERERERGpiYkVERERERKSmYp1YyWQynDlzhostFDD2a+Fh3xYO9mvhYd8WHvZt4WC/Fh72beFgv5YdxTqxksvl+PvvvyGXyzUdSqnCfi087NvCwX4tPOzbwsO+LRzs18LDvi0c7Neyo1gnVkRERERERCUBEysiIiIiIiI1MbEiIiIiIiJSU7FOrMRiMZo1awaxWKzpUEoV9mvhYd8WDvZr4WHfFh72beFgvxYe9m3hYL+WHSJBEARNB0FERERERFSSFesRKyIiIiIiopKAiRUREREREZGamFgRERERERGpiYkVERERERGRmrQ1HUBWgoODcfHiRbx69QoJCQno3bs3KlasqOmwir3c+s3f3x937txRqePm5ob+/fsrv589exZPnz7F69evIRaL8f333xdZ/MXVtWvXcP36dbx9+xYAYG1tjaZNm8LDwwMAIJPJcOzYMdy/fx8ymQzu7u5o164dDA0NlW0cOXIEISEhiIiIgKWlJUaNGqWJUynWzp8/j5MnT6JevXpo06YNAGD9+vUIDg5WKVerVi106NBB+Z19m7V3794hICAAgYGBSEtLg7m5OTp37gx7e3sAgCAIOHPmDG7evInk5GQ4OTmhffv2sLCwULbB3weZLVq0CHFxcZm2165dG+3bt+c1q4aUlBScPn0ajx49QmJiImxtbdGmTRs4ODgA4DWbV7ndC+SlH7O6zlu2bInGjRsDSP//3sGDBxEeHo7IyEh4enqiT58+RXOCGpJTv8rlcpw6dQqBgYGIjY2FVCqFq6srfH19YWRkpGwjKSkJR44cwePHjyESieDl5YW2bdtCR0cHQNns19KmWCZWqampsLGxQfXq1bFz505Nh1Ni5KXf3N3d0blzZ+X3j5f+lMvlqFSpEhwdHXHr1q1CjbekMDY2hq+vL8zNzQEAt2/fxvbt2/HFF1/A2toaR48exdOnT9GzZ09IpVIcOXIEO3fuxNChQ1XaqV69OsLCwvDmzRtNnEaxFhYWhhs3bsDGxibTvpo1a6J58+bK7xKJJFMZ9q2qpKQkrF27FuXLl8fnn38OfX19xMTEQFdXV1nmwoULuHLlCrp06QIzMzOcPn0amzdvxtixY6Gtnf6/Bv4+yGzEiBH4cDHdiIgIbNq0CZUrV1Zu4zX7aQ4cOICIiAh07doVRkZGuHv3LjZt2oQxY8bA2NiY12we5XYvkJd+BAAfHx/UqlVL+T3j5h8AFAoFtLW1UbduXTx8+LBwT6iYyKlf09LS8Pr1azRt2hQ2NjZITk7G0aNHsW3bNowcOVJZbs+ePYiPj8eAAQOgUCiwb98+HDhwAN27dwdQNvu1tCmWUwE9PDzQokULeHl5aTqUEiUv/SYWi2FoaKj86Onpqexv3rw5GjRokOUNbllVoUIFeHh4wMLCAhYWFmjZsiV0dHQQGhqK5ORk3Lp1C61bt0b58uVhb2+Pzp07IyQkBKGhoco22rZti7p168LMzEyDZ1I8paamYs+ePejYsaPKjX8GiUSics1KpVKV/ezbzC5cuAATExN07twZDg4OMDMzg5ubm/KPA4Ig4MqVK2jatCkqVqwIGxsbdOnSBfHx8Xj06JGyHf4+yMzAwEDlenzy5AnMzMzg7OysLMNrNv/S0tLw4MED+Pr6wtnZGebm5vDx8YG5uTmuX7/OazYfcroXyGs/AoBUKlW5jj9MrHR0dNChQwfUqlVLZXZGaZZTv+rq6mLAgAGoXLkyLC0t4ejoiLZt2yI8PFw58hcZGYnAwEB06tQJjo6OKFeuHNq2bYt79+4hPj4eQNns19KmWI5YUeEJCgrC/PnzoaenBxcXF7Ro0QL6+vqaDqvEUCgUePDgAdLS0uDk5ITw8HAoFAq4uroqy1haWsLExAQhISFwdHTUYLQlw+HDh+Hh4QFXV1ecPXs20/5//vkHd+/ehaGhITw9PdGsWbMsRwDoP48fP4abmxt27dqFoKAgGBsbo3bt2sq/Pr99+xYJCQkq162uri4cHR0REhICb29vTYVeosjlcty9excNGjSASCRSbuc1m38KhQKCIKiMmACAtrY2Xr58yWu2gOSnH8+fP4+zZ8/CxMQE3t7eaNCgAbS0iuXf44ullJQUAFD+wTA0NBS6urrK6dgA4OrqCpFIhNDQUA4mlBJMrMoQd3d3eHl5wdTUFLGxsTh58iS2bNmCYcOG8ZdlLt68eYM1a9ZAJpNBR0cHvXv3hpWVlXIe/8cjLQYGBkhISNBQtCXHvXv3EB4ejhEjRmS5v0qVKjAxMYGRkRHevHmDgIAAREdHo3fv3kUcackSGxuL69evo0GDBmjcuDFevXqFo0ePQiwWo3r16spr08DAQKWegYEBEhMTNRFyifTo0SMkJyejevXqym28Zj+NVCqFo6Mjzp49CysrKxgYGODevXsIDQ2Fubk5r9kCktd+rFevHuzs7KCnp4eQkBCcPHkSCQkJaN26dZHGW1LJZDIEBASgSpUqyhHrhISETP2upaUFPT093i+UIkysypAP/xJlY2MDGxsbLF68GEFBQSp/vaLMMh4wT05OxoMHD+Dv74/BgwdrOqwSLS4uDkePHsWAAQMy/ZU6w4fz+21sbGBkZISNGzciJiZGOa2NMhMEAfb29mjZsiUAwM7ODhEREbhx44ZKEkDquXXrFjw8PFQeTuc1++m6du2K/fv3Y+HChRCJRLCzs4O3tzfCw8M1HVqZ06BBA+XPNjY2EIvFOHjwIFq2bJnt72tKJ5fLsWvXLgiCgPbt22s6HCpi/K+jDDMzM1M+1M7EKmdisVh5U2Rvb49Xr17h8uXL8Pb2hlwuR3JyssqoVWJiIudH5yI8PByJiYlYtWqVcpsgCAgODsbVq1cxderUTCOpGauD8SY1Z0ZGRrCyslLZZmlpqXwYOuPaTExMVEkKEhMTy/SzKfnx9u1bPH/+HL169cqxHK/ZvDM3N8fgwYORmpqKlJQUGBkZwc/PD2ZmZrxmC8in9qODgwMUCgXevn0LS0vLQo+zpJLL5fDz80NcXBwGDhyo8nyloaFhptFVhUKBpKQk3i+UIkysyrB3797h/fv3Kr9cKW8EQYBcLoednR20tLTw/PlzVKpUCQAQFRWFuLg4ODk5aTjK4q18+fIYPXq0yrZ9+/bB0tISjRo1ynJ66uvXrwGA12wunJycEB0drbItOjoaJiYmAABTU1MYGhri+fPnsLW1BZD+PEBoaChq165d5PGWRLdv34aBgQE8PT1zLMdrNv90dHSgo6ODpKQkBAYGolWrVrxmC8in9uPr168hEokyTWWj/2QkVdHR0Rg0aFCm59cdHR2RnJyMV69eKZ+zevHiBQRB4PPYpUixTKxSU1MRExOj/B4bG4vXr19DT09PeWNAmeXUb3p6ejhz5gwqVaoEQ0NDxMTEICAgAObm5nBzc1PWiYuLQ1JSEuLi4iAIgvKmwNzcXGVFoLIkICAAHh4eMDExQUpKCv755x8EBQWhf//+0NXVRY0aNXD8+HHo6ekpl1t3dHRU+UUZExOD1NRUJCQkQCaTKfvVysoq05L3ZYVUKoW1tbXKNolEAj09PVhbWyMmJgb//PMPPDw8oK+vjzdv3uDYsWNwdnZW+csq+zaz+vXrY+3atTh37hwqV66MsLAw3Lx5U/kuJZFIhHr16uHcuXOwsLCAqakpTp8+DSMjI5X33fD3QdYEQcDt27dRrVo1lT8A8JpVT2BgIADAwsICMTExOHHiBCwtLVG9enVes/mQ2z1Ubv0YEhKCsLAwuLi4QCqVIiQkBMeOHUPVqlVVVhKOjIyEXC5HUlISUlNTlX2dkbCVNjn1q6GhIXbt2oXw8HD07dsXgiAon5vS09ODWCyGlZUV3N3dceDAAXTo0AFyuRyHDx+Gt7e3yh9eylq/ljYi4cMXchQTQUFB2LBhQ6bt1apVQ5cuXYo+oBIip35r3749duzYgfDwcCQnJ8PIyAhubm5o3ry5yhB0Vi8RBoBBgwbBxcWlMMMvtvbt24cXL14gISEBUqkUNjY2aNSokTIhzXhB8L179yCXy+Hm5ob27dur9GtWLw0FgK+++gqmpqZFdSrF3vr165UvBY2Li8PevXsRERGB1NRUmJiYoGLFimjatKnK9Ar2bdaePHmCkydPIjo6GmZmZqhfv77K8z8ZLwm9ceMGkpOTUa5cuUwvCeXvg6w9e/YMmzdvxrhx41T6i9eseu7fv4+TJ0/i3bt30NPTg5eXF1q0aKGcZs1rNm9yu4fKrR/Dw8Nx6NAhREVFQS6Xw9TUFFWrVkWDBg1Unq/K7mXZ06dPL7yT06Cc+tXHxwd//vlnlvU+vPaSkpJw+PBhPHnyJMsXBANlr19Lm2KZWBEREREREZUkXGObiIiIiIhITUysiIiIiIiI1MTEioiIiIiISE1MrIiIiIiIiNTExIqIiIiIiEhNTKyIiIiIiIjUxMSKiIiIiIhITUysiIiIiIiI1MTEioiIiIiISE1MrIiIiIiIiNTExIqIiIiIiEhNTKyIiIiIiIjU9H8ls5aDi0j55QAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<Figure size 1000x300 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -330,19 +330,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.612604Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.612245Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.619284Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.618702Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.612582Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.346013Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.345645Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.356143Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.355441Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.345984Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -436,19 +436,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.620356Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.620051Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.633477Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.632973Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.620336Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.357522Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.357148Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.372207Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.371567Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.357494Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -534,19 +534,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.634461Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.634174Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.638935Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.638433Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.634441Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.373886Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.373526Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.379847Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.379051Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.373860Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0    recA_lib-1\n",
@@ -564,19 +564,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.640014Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.639659Z",
-                    "iopub.status.idle": "2023-06-19T11:20:52.643836Z",
-                    "shell.execute_reply": "2023-06-19T11:20:52.643142Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.639993Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.381209Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.380881Z",
+                    "iopub.status.idle": "2024-05-23T18:11:31.386391Z",
+                    "shell.execute_reply": "2024-05-23T18:11:31.385577Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.381181Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "('recA_lib-1', 'recA_lib-2')"
@@ -592,19 +592,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:52.644935Z",
-                    "iopub.status.busy": "2023-06-19T11:20:52.644652Z",
-                    "iopub.status.idle": "2023-06-19T11:20:53.460491Z",
-                    "shell.execute_reply": "2023-06-19T11:20:53.459638Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:52.644913Z"
+                    "iopub.execute_input": "2024-05-23T18:11:31.387769Z",
+                    "iopub.status.busy": "2024-05-23T18:11:31.387418Z",
+                    "iopub.status.idle": "2024-05-23T18:11:32.165947Z",
+                    "shell.execute_reply": "2024-05-23T18:11:32.164411Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:31.387737Z"
                 }
             },
             "outputs": [],
             "source": [
                 "ccs_summaries = alignparse.ccs.Summaries(pacbio_runs)"
             ]
         },
@@ -618,19 +618,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:53.462103Z",
-                    "iopub.status.busy": "2023-06-19T11:20:53.461793Z",
-                    "iopub.status.idle": "2023-06-19T11:20:54.097665Z",
-                    "shell.execute_reply": "2023-06-19T11:20:54.096988Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:53.462080Z"
+                    "iopub.execute_input": "2024-05-23T18:11:32.168569Z",
+                    "iopub.status.busy": "2024-05-23T18:11:32.168007Z",
+                    "iopub.status.idle": "2024-05-23T18:11:32.783337Z",
+                    "shell.execute_reply": "2024-05-23T18:11:32.782402Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:32.168515Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "p = ccs_summaries.plot_zmw_stats()\n",
                 "p = p + theme(panel_grid_major_x=element_blank())  # no vertical grid lines\n",
@@ -645,19 +645,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:54.101249Z",
-                    "iopub.status.busy": "2023-06-19T11:20:54.100841Z",
-                    "iopub.status.idle": "2023-06-19T11:20:54.141382Z",
-                    "shell.execute_reply": "2023-06-19T11:20:54.140660Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:54.101228Z"
+                    "iopub.execute_input": "2024-05-23T18:11:32.784919Z",
+                    "iopub.status.busy": "2024-05-23T18:11:32.784530Z",
+                    "iopub.status.idle": "2024-05-23T18:11:32.831505Z",
+                    "shell.execute_reply": "2024-05-23T18:11:32.830894Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:32.784893Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -705,24 +705,24 @@
                             "      <td>Failed -- Draft generation error</td>\n",
                             "      <td>3</td>\n",
                             "      <td>0.018072</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>recA_lib-1</td>\n",
-                            "      <td>Failed -- Min coverage violation</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>0.006024</td>\n",
+                            "      <td>Failed -- CCS below minimum RQ</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>0.012048</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>recA_lib-1</td>\n",
-                            "      <td>Failed -- CCS below minimum RQ</td>\n",
-                            "      <td>2</td>\n",
-                            "      <td>0.012048</td>\n",
+                            "      <td>Failed -- Min coverage violation</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>0.006024</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>recA_lib-1</td>\n",
                             "      <td>Failed -- Other reason</td>\n",
                             "      <td>2</td>\n",
                             "      <td>0.012048</td>\n",
@@ -747,22 +747,22 @@
                             "      <td>Failed -- Draft generation error</td>\n",
                             "      <td>4</td>\n",
                             "      <td>0.025641</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9</th>\n",
                             "      <td>recA_lib-2</td>\n",
-                            "      <td>Failed -- Min coverage violation</td>\n",
+                            "      <td>Failed -- CCS below minimum RQ</td>\n",
                             "      <td>2</td>\n",
                             "      <td>0.012821</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10</th>\n",
                             "      <td>recA_lib-2</td>\n",
-                            "      <td>Failed -- CCS below minimum RQ</td>\n",
+                            "      <td>Failed -- Min coverage violation</td>\n",
                             "      <td>2</td>\n",
                             "      <td>0.012821</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>11</th>\n",
                             "      <td>recA_lib-2</td>\n",
                             "      <td>Failed -- Other reason</td>\n",
@@ -774,22 +774,22 @@
                             "</div>"
                         ],
                         "text/plain": [
                             "          name                            status  number  fraction\n",
                             "0   recA_lib-1          Success -- CCS generated     139  0.837349\n",
                             "1   recA_lib-1     Failed -- Lacking full passes      19  0.114458\n",
                             "2   recA_lib-1  Failed -- Draft generation error       3  0.018072\n",
-                            "3   recA_lib-1  Failed -- Min coverage violation       1  0.006024\n",
-                            "4   recA_lib-1    Failed -- CCS below minimum RQ       2  0.012048\n",
+                            "3   recA_lib-1    Failed -- CCS below minimum RQ       2  0.012048\n",
+                            "4   recA_lib-1  Failed -- Min coverage violation       1  0.006024\n",
                             "5   recA_lib-1            Failed -- Other reason       2  0.012048\n",
                             "6   recA_lib-2          Success -- CCS generated     124  0.794872\n",
                             "7   recA_lib-2     Failed -- Lacking full passes      22  0.141026\n",
                             "8   recA_lib-2  Failed -- Draft generation error       4  0.025641\n",
-                            "9   recA_lib-2  Failed -- Min coverage violation       2  0.012821\n",
-                            "10  recA_lib-2    Failed -- CCS below minimum RQ       2  0.012821\n",
+                            "9   recA_lib-2    Failed -- CCS below minimum RQ       2  0.012821\n",
+                            "10  recA_lib-2  Failed -- Min coverage violation       2  0.012821\n",
                             "11  recA_lib-2            Failed -- Other reason       2  0.012821"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -806,19 +806,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:54.142561Z",
-                    "iopub.status.busy": "2023-06-19T11:20:54.142233Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.156677Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.153817Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:54.142542Z"
+                    "iopub.execute_input": "2024-05-23T18:11:32.833209Z",
+                    "iopub.status.busy": "2024-05-23T18:11:32.832843Z",
+                    "iopub.status.idle": "2024-05-23T18:11:33.710580Z",
+                    "shell.execute_reply": "2024-05-23T18:11:33.708786Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:32.833184Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "for stat in [\"length\", \"passes\", \"accuracy\"]:\n",
                 "    if ccs_summaries.has_stat(stat):\n",
@@ -837,19 +837,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.161866Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.160326Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.177054Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.176233Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.161815Z"
+                    "iopub.execute_input": "2024-05-23T18:11:33.713769Z",
+                    "iopub.status.busy": "2024-05-23T18:11:33.713146Z",
+                    "iopub.status.idle": "2024-05-23T18:11:33.726873Z",
+                    "shell.execute_reply": "2024-05-23T18:11:33.726189Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:33.713708Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -934,32 +934,34 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 17,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.178915Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.178366Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.249383Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.248646Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.178882Z"
+                    "iopub.execute_input": "2024-05-23T18:11:33.728152Z",
+                    "iopub.status.busy": "2024-05-23T18:11:33.727822Z",
+                    "iopub.status.idle": "2024-05-23T18:11:33.741144Z",
+                    "shell.execute_reply": "2024-05-23T18:11:33.739902Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:33.728127Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Using `minimap2` 2.17-r941 with these options:\n",
+                        "Using `minimap2` 2.22-r1101 with these options:\n",
                         "-A2 -B4 -O12 -E2 --end-bonus=13 --secondary=no --cs\n"
                     ]
                 }
             ],
             "source": [
+                "# NBVAL_IGNORE_OUTPUT\n",
+                "\n",
                 "mapper = alignparse.minimap2.Mapper(alignparse.minimap2.OPTIONS_CODON_DMS)\n",
                 "\n",
                 "print(\n",
                 "    f\"Using `minimap2` {mapper.version} with these options:\\n\"\n",
                 "    + \" \".join(mapper.options)\n",
                 ")"
             ]
@@ -975,19 +977,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.250789Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.250476Z",
-                    "iopub.status.idle": "2023-06-19T11:20:55.254255Z",
-                    "shell.execute_reply": "2023-06-19T11:20:55.253730Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.250762Z"
+                    "iopub.execute_input": "2024-05-23T18:11:33.743528Z",
+                    "iopub.status.busy": "2024-05-23T18:11:33.742927Z",
+                    "iopub.status.idle": "2024-05-23T18:11:33.748800Z",
+                    "shell.execute_reply": "2024-05-23T18:11:33.747687Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:33.743471Z"
                 }
             },
             "outputs": [],
             "source": [
                 "align_and_parse_outdir = os.path.join(outdir, \"RecA_align_and_parse\")"
             ]
         },
@@ -1000,19 +1002,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:55.255360Z",
-                    "iopub.status.busy": "2023-06-19T11:20:55.255053Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.397627Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.396660Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:55.255338Z"
+                    "iopub.execute_input": "2024-05-23T18:11:33.758115Z",
+                    "iopub.status.busy": "2024-05-23T18:11:33.757696Z",
+                    "iopub.status.idle": "2024-05-23T18:11:34.912577Z",
+                    "shell.execute_reply": "2024-05-23T18:11:34.911220Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:33.758084Z"
                 }
             },
             "outputs": [],
             "source": [
                 "readstats, aligned, filtered = targets.align_and_parse(\n",
                 "    df=pacbio_runs,\n",
                 "    mapper=mapper,\n",
@@ -1036,19 +1038,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.399269Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.398888Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.408800Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.407917Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.399243Z"
+                    "iopub.execute_input": "2024-05-23T18:11:34.914587Z",
+                    "iopub.status.busy": "2024-05-23T18:11:34.914153Z",
+                    "iopub.status.idle": "2024-05-23T18:11:34.928149Z",
+                    "shell.execute_reply": "2024-05-23T18:11:34.926907Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:34.914551Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1076,63 +1078,63 @@
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>lib-1</td>\n",
                             "      <td>recA_lib-1</td>\n",
-                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
-                            "      <td>123</td>\n",
+                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
+                            "      <td>16</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>lib-1</td>\n",
                             "      <td>recA_lib-1</td>\n",
-                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
-                            "      <td>16</td>\n",
+                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
+                            "      <td>123</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>lib-1</td>\n",
                             "      <td>recA_lib-1</td>\n",
                             "      <td>unmapped</td>\n",
                             "      <td>0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>lib-2</td>\n",
                             "      <td>recA_lib-2</td>\n",
-                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
-                            "      <td>112</td>\n",
+                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
+                            "      <td>12</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>lib-2</td>\n",
                             "      <td>recA_lib-2</td>\n",
-                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
-                            "      <td>12</td>\n",
+                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
+                            "      <td>112</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>lib-2</td>\n",
                             "      <td>recA_lib-2</td>\n",
                             "      <td>unmapped</td>\n",
                             "      <td>0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  library        name                       category  count\n",
-                            "0   lib-1  recA_lib-1   aligned RecA_PacBio_amplicon    123\n",
-                            "1   lib-1  recA_lib-1  filtered RecA_PacBio_amplicon     16\n",
+                            "0   lib-1  recA_lib-1  filtered RecA_PacBio_amplicon     16\n",
+                            "1   lib-1  recA_lib-1   aligned RecA_PacBio_amplicon    123\n",
                             "2   lib-1  recA_lib-1                       unmapped      0\n",
-                            "3   lib-2  recA_lib-2   aligned RecA_PacBio_amplicon    112\n",
-                            "4   lib-2  recA_lib-2  filtered RecA_PacBio_amplicon     12\n",
+                            "3   lib-2  recA_lib-2  filtered RecA_PacBio_amplicon     12\n",
+                            "4   lib-2  recA_lib-2   aligned RecA_PacBio_amplicon    112\n",
                             "5   lib-2  recA_lib-2                       unmapped      0"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -1151,19 +1153,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.410643Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.410182Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.595923Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.594703Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.410610Z"
+                    "iopub.execute_input": "2024-05-23T18:11:34.930535Z",
+                    "iopub.status.busy": "2024-05-23T18:11:34.930006Z",
+                    "iopub.status.idle": "2024-05-23T18:11:35.264328Z",
+                    "shell.execute_reply": "2024-05-23T18:11:35.263529Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:34.930489Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "p = (\n",
                 "    ggplot(readstats, aes(\"category\", \"count\"))\n",
@@ -1186,19 +1188,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.598115Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.597532Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.616767Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.615730Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.598078Z"
+                    "iopub.execute_input": "2024-05-23T18:11:35.265625Z",
+                    "iopub.status.busy": "2024-05-23T18:11:35.265382Z",
+                    "iopub.status.idle": "2024-05-23T18:11:35.281505Z",
+                    "shell.execute_reply": "2024-05-23T18:11:35.280841Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:35.265601Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1364,19 +1366,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.618607Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.618249Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.638904Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.637860Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.618575Z"
+                    "iopub.execute_input": "2024-05-23T18:11:35.283682Z",
+                    "iopub.status.busy": "2024-05-23T18:11:35.283290Z",
+                    "iopub.status.idle": "2024-05-23T18:11:35.301722Z",
+                    "shell.execute_reply": "2024-05-23T18:11:35.301041Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:35.283648Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -1518,19 +1520,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.641187Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.640487Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.653028Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.652188Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.641148Z"
+                    "iopub.execute_input": "2024-05-23T18:11:35.303428Z",
+                    "iopub.status.busy": "2024-05-23T18:11:35.303081Z",
+                    "iopub.status.idle": "2024-05-23T18:11:35.314734Z",
+                    "shell.execute_reply": "2024-05-23T18:11:35.313849Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:35.303401Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1640,19 +1642,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 25,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.655208Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.654529Z",
-                    "iopub.status.idle": "2023-06-19T11:20:56.928828Z",
-                    "shell.execute_reply": "2023-06-19T11:20:56.927933Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.655171Z"
+                    "iopub.execute_input": "2024-05-23T18:11:35.316220Z",
+                    "iopub.status.busy": "2024-05-23T18:11:35.315831Z",
+                    "iopub.status.idle": "2024-05-23T18:11:35.601375Z",
+                    "shell.execute_reply": "2024-05-23T18:11:35.600487Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:35.316191Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "for targetname in targets.target_names:\n",
                 "    target_filtered = filtered[targetname]\n",
@@ -1682,19 +1684,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 26,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:56.930158Z",
-                    "iopub.status.busy": "2023-06-19T11:20:56.929827Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.969865Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.968374Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:56.930137Z"
+                    "iopub.execute_input": "2024-05-23T18:11:35.602845Z",
+                    "iopub.status.busy": "2024-05-23T18:11:35.602604Z",
+                    "iopub.status.idle": "2024-05-23T18:11:36.764052Z",
+                    "shell.execute_reply": "2024-05-23T18:11:36.762178Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:35.602821Z"
                 }
             },
             "outputs": [],
             "source": [
                 "readstats_csv, aligned_csv, filtered_csv = targets.align_and_parse(\n",
                 "    df=pacbio_runs,\n",
                 "    mapper=mapper,\n",
@@ -1716,19 +1718,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 27,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.972247Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.971776Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.977829Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.976939Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.972201Z"
+                    "iopub.execute_input": "2024-05-23T18:11:36.766619Z",
+                    "iopub.status.busy": "2024-05-23T18:11:36.766143Z",
+                    "iopub.status.idle": "2024-05-23T18:11:36.772286Z",
+                    "shell.execute_reply": "2024-05-23T18:11:36.771445Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:36.766576Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1752,19 +1754,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 28,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.979682Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.979156Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.986705Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.986081Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.979642Z"
+                    "iopub.execute_input": "2024-05-23T18:11:36.773975Z",
+                    "iopub.status.busy": "2024-05-23T18:11:36.773582Z",
+                    "iopub.status.idle": "2024-05-23T18:11:36.783794Z",
+                    "shell.execute_reply": "2024-05-23T18:11:36.782976Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:36.773942Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -1804,19 +1806,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 29,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.987892Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.987505Z",
-                    "iopub.status.idle": "2023-06-19T11:20:57.995637Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.994953Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.987872Z"
+                    "iopub.execute_input": "2024-05-23T18:11:36.785813Z",
+                    "iopub.status.busy": "2024-05-23T18:11:36.785440Z",
+                    "iopub.status.idle": "2024-05-23T18:11:36.795202Z",
+                    "shell.execute_reply": "2024-05-23T18:11:36.794178Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:36.785784Z"
                 }
             },
             "outputs": [],
             "source": [
                 "error_rate_floor = 1e-7  # error rates < this set to this\n",
                 "\n",
                 "aligned_df = aligned_df.assign(\n",
@@ -1836,19 +1838,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 30,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:57.996892Z",
-                    "iopub.status.busy": "2023-06-19T11:20:57.996561Z",
-                    "iopub.status.idle": "2023-06-19T11:20:58.000047Z",
-                    "shell.execute_reply": "2023-06-19T11:20:57.999410Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:57.996868Z"
+                    "iopub.execute_input": "2024-05-23T18:11:36.796919Z",
+                    "iopub.status.busy": "2024-05-23T18:11:36.796481Z",
+                    "iopub.status.idle": "2024-05-23T18:11:36.801126Z",
+                    "shell.execute_reply": "2024-05-23T18:11:36.800184Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:36.796885Z"
                 }
             },
             "outputs": [],
             "source": [
                 "error_cutoff = 1e-4"
             ]
         },
@@ -1860,19 +1862,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 31,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:58.001290Z",
-                    "iopub.status.busy": "2023-06-19T11:20:58.000923Z",
-                    "iopub.status.idle": "2023-06-19T11:20:58.855372Z",
-                    "shell.execute_reply": "2023-06-19T11:20:58.854669Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:58.001268Z"
+                    "iopub.execute_input": "2024-05-23T18:11:36.802650Z",
+                    "iopub.status.busy": "2024-05-23T18:11:36.802265Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.481052Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.480057Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:36.802623Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "p = (\n",
                 "    ggplot(\n",
@@ -1905,19 +1907,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 32,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:58.856501Z",
-                    "iopub.status.busy": "2023-06-19T11:20:58.856174Z",
-                    "iopub.status.idle": "2023-06-19T11:20:58.861063Z",
-                    "shell.execute_reply": "2023-06-19T11:20:58.860469Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:58.856482Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.482622Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.482385Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.490347Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.489475Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.482599Z"
                 }
             },
             "outputs": [],
             "source": [
                 "aligned_df = aligned_df.assign(\n",
                 "    retained=lambda x: (\n",
                 "        (x[\"gene_error\"] <= error_cutoff) & (x[\"barcode_error\"] <= error_cutoff)\n",
@@ -1933,19 +1935,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 33,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:58.862039Z",
-                    "iopub.status.busy": "2023-06-19T11:20:58.861779Z",
-                    "iopub.status.idle": "2023-06-19T11:20:58.870482Z",
-                    "shell.execute_reply": "2023-06-19T11:20:58.869940Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:58.862022Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.491699Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.491372Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.506206Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.505526Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.491672Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2031,19 +2033,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 34,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:58.871461Z",
-                    "iopub.status.busy": "2023-06-19T11:20:58.871207Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.059627Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.058758Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:58.871443Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.507551Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.507294Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.715403Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.714647Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.507523Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "max_CCSs = 8  # in plot, group barcodes with >= this many CCSs\n",
                 "\n",
@@ -2092,19 +2094,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 35,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.061097Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.060686Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.073012Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.072233Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.061068Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.716641Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.716421Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.729476Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.728770Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.716619Z"
                 }
             },
             "outputs": [],
             "source": [
                 "aligned_df = alignparse.consensus.add_mut_info_cols(\n",
                 "    aligned_df, mutation_col=\"gene_mutations\", n_indel_col=\"n_indels\"\n",
                 ")\n",
@@ -2120,19 +2122,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 36,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.074379Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.074026Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.084362Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.083693Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.074349Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.730691Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.730441Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.745522Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.744859Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.730664Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2219,19 +2221,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 37,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.085431Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.085174Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.125964Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.125406Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.085413Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.746925Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.746665Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.805058Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.804203Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.746899Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2296,19 +2298,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 38,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.127281Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.126946Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.187402Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.185907Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.127262Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.806962Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.806552Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.851233Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.850716Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.806931Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2386,19 +2388,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 39,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.190142Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.189544Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.213990Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.213208Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.190095Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.852673Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.852375Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.868972Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.868212Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.852657Z"
                 }
             },
             "outputs": [],
             "source": [
                 "consensus, dropped = alignparse.consensus.simple_mutconsensus(\n",
                 "    aligned_df.query(\"retained\"),\n",
                 "    group_cols=(\"library\", \"barcode\"),\n",
@@ -2415,19 +2417,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 40,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.215326Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.215005Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.223405Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.222750Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.215304Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.870088Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.869798Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.877165Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.876328Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.870071Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2532,19 +2534,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 41,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.227916Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.227540Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.240656Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.239971Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.227894Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.878326Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.878068Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.889259Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.888548Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.878308Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2673,19 +2675,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 42,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.241802Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.241520Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.248716Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.248074Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.241781Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.890523Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.890255Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.897393Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.896717Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.890505Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2770,19 +2772,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 43,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:59.249809Z",
-                    "iopub.status.busy": "2023-06-19T11:20:59.249541Z",
-                    "iopub.status.idle": "2023-06-19T11:20:59.258597Z",
-                    "shell.execute_reply": "2023-06-19T11:20:59.257867Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:59.249788Z"
+                    "iopub.execute_input": "2024-05-23T18:11:37.898482Z",
+                    "iopub.status.busy": "2024-05-23T18:11:37.898192Z",
+                    "iopub.status.idle": "2024-05-23T18:11:37.906206Z",
+                    "shell.execute_reply": "2024-05-23T18:11:37.905304Z",
+                    "shell.execute_reply.started": "2024-05-23T18:11:37.898465Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -2851,15 +2853,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.9"
         },
         "toc": {
             "nav_menu": {},
             "number_sections": false,
             "sideBar": true,
             "skip_h1_title": false,
             "toc_cell": false,
```

### Comparing `alignparse-0.6.2/paper/paper.bib` & `alignparse-0.6.3/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/paper/paper.md` & `alignparse-0.6.3/paper/paper.md`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/setup.py` & `alignparse-0.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Setup script for ``alignparse``."""
 
-
 import re
 import sys
 
 from setuptools import setup
 
 
 if not (sys.version_info[0] == 3 and sys.version_info[1] >= 8):
@@ -48,15 +47,15 @@
         "dna_features_viewer>=1.0.0",
         "matplotlib>=3.0.0",
         "numpy>=1.17",
         "packaging",
         "pandas>=0.25.1",
         "pathos>=0.2.4",
         "plotnine>=0.6",
-        "pysam>=0.14",
+        "pysam!=0.22.1",
         "regex>=2.5.33",
         "scipy>=1.2",
         "pyyaml>=5.1.1",
     ],
     platforms="Linux and Mac OS X.",
     packages=["alignparse"],
     package_dir={"alignparse": "alignparse"},
```

### Comparing `alignparse-0.6.2/tests/check_Targets_align_and_parse.ipynb` & `alignparse-0.6.3/tests/check_Targets_align_and_parse.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996986604165714%*

 * *Differences: {"'cells'": "{3: {'metadata': {'execution': {'iopub.execute_input': '2024-05-23T17:54:10.494438Z', "*

 * *            "'iopub.status.busy': '2024-05-23T17:54:10.494020Z', 'iopub.status.idle': "*

 * *            "'2024-05-23T17:54:13.342417Z', 'shell.execute_reply': '2024-05-23T17:54:13.341573Z', "*

 * *            "'shell.execute_reply.started': '2024-05-23T17:54:10.494410Z'}}}, 5: {'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2024-05-23T17:54:13.352773Z', "*

 * *            "'iopub.status.busy': '2024-05- […]*

```diff
@@ -27,19 +27,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:02.971425Z",
-                    "iopub.status.busy": "2023-06-19T11:21:02.970985Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.797828Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.796912Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:02.971393Z"
+                    "iopub.execute_input": "2024-05-23T17:54:10.494438Z",
+                    "iopub.status.busy": "2024-05-23T17:54:10.494020Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.342417Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.341573Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:10.494410Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import warnings\n",
                 "\n",
@@ -58,19 +58,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.799605Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.799231Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.803204Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.802484Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.799581Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.352773Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.352427Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.356546Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.355785Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.352741Z"
                 }
             },
             "outputs": [],
             "source": [
                 "warnings.simplefilter(\"ignore\")"
             ]
         },
@@ -82,19 +82,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.804308Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.804103Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.810754Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.810089Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.804289Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.367746Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.367234Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.374750Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.373968Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.367692Z"
                 }
             },
             "outputs": [],
             "source": [
                 "outdir_base = \"_temp_check_Targets_align_and_parse\"\n",
                 "outdir_separate = os.path.join(outdir_base, \"separate/\")\n",
                 "outdir_together = os.path.join(outdir_base, \"together/\")\n",
@@ -110,19 +110,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.812573Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.812274Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.835599Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.834752Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.812552Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.384538Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.384133Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.418318Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.417504Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.384501Z"
                 }
             },
             "outputs": [],
             "source": [
                 "recA_targetfile = \"../notebooks/input_files/recA_amplicon.gb\"\n",
                 "recA_parse_specs_file = \"../notebooks/input_files/recA_feature_parse_specs.yaml\"\n",
                 "targets = alignparse.targets.Targets(\n",
@@ -138,19 +138,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.836939Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.836571Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.851368Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.850729Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.836915Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.427051Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.426718Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.444375Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.443634Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.427021Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -231,19 +231,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.852646Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.852256Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.872919Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.871635Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.852620Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.453312Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.452997Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.473952Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.472489Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.453285Z"
                 }
             },
             "outputs": [],
             "source": [
                 "mapper = alignparse.minimap2.Mapper(alignparse.minimap2.OPTIONS_CODON_DMS)"
             ]
         },
@@ -256,19 +256,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.874901Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.874505Z",
-                    "iopub.status.idle": "2023-06-19T11:21:04.888264Z",
-                    "shell.execute_reply": "2023-06-19T11:21:04.887624Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.874859Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.488191Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.487797Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.500845Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.499925Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.488148Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -349,19 +349,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:04.889519Z",
-                    "iopub.status.busy": "2023-06-19T11:21:04.889217Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.235111Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.233345Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:04.889498Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.502251Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.501894Z",
+                    "iopub.status.idle": "2024-05-23T17:54:13.625547Z",
+                    "shell.execute_reply": "2024-05-23T17:54:13.624037Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.502222Z"
                 }
             },
             "outputs": [],
             "source": [
                 "for tup in pacbio_runs.itertuples(index=False):\n",
                 "    targets.align(queryfile=tup.fastq, alignmentfile=tup.alignments, mapper=mapper)"
             ]
@@ -374,19 +374,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.237830Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.237332Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.440566Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.439888Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.237799Z"
+                    "iopub.execute_input": "2024-05-23T17:54:13.627878Z",
+                    "iopub.status.busy": "2024-05-23T17:54:13.627296Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.043959Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.043043Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:13.627830Z"
                 }
             },
             "outputs": [],
             "source": [
                 "readstats = []\n",
                 "aligned = {targetname: [] for targetname in targets.target_names}\n",
                 "filtered = {targetname: [] for targetname in targets.target_names}\n",
@@ -417,19 +417,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.442767Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.442453Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.449578Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.449026Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.442746Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.046079Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.045664Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.055106Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.054255Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.046051Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -454,59 +454,59 @@
                             "      <th>count</th>\n",
                             "      <th>name</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
-                            "      <td>123</td>\n",
+                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
+                            "      <td>16</td>\n",
                             "      <td>recA_lib-1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
-                            "      <td>16</td>\n",
+                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
+                            "      <td>123</td>\n",
                             "      <td>recA_lib-1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>unmapped</td>\n",
                             "      <td>0</td>\n",
                             "      <td>recA_lib-1</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
-                            "      <td>112</td>\n",
+                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
+                            "      <td>12</td>\n",
                             "      <td>recA_lib-2</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
-                            "      <td>12</td>\n",
+                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
+                            "      <td>112</td>\n",
                             "      <td>recA_lib-2</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>unmapped</td>\n",
                             "      <td>0</td>\n",
                             "      <td>recA_lib-2</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                        category  count        name\n",
-                            "0   aligned RecA_PacBio_amplicon    123  recA_lib-1\n",
-                            "1  filtered RecA_PacBio_amplicon     16  recA_lib-1\n",
+                            "0  filtered RecA_PacBio_amplicon     16  recA_lib-1\n",
+                            "1   aligned RecA_PacBio_amplicon    123  recA_lib-1\n",
                             "2                       unmapped      0  recA_lib-1\n",
-                            "3   aligned RecA_PacBio_amplicon    112  recA_lib-2\n",
-                            "4  filtered RecA_PacBio_amplicon     12  recA_lib-2\n",
+                            "3  filtered RecA_PacBio_amplicon     12  recA_lib-2\n",
+                            "4   aligned RecA_PacBio_amplicon    112  recA_lib-2\n",
                             "5                       unmapped      0  recA_lib-2"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -524,19 +524,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.450623Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.450332Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.459162Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.458560Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.450604Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.056565Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.056191Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.067495Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.065916Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.056537Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -624,19 +624,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.460307Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.459974Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.471662Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.471008Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.460286Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.069938Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.069357Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.086836Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.085795Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.069886Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -787,19 +787,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.472938Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.472576Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.833393Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.832298Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.472914Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.088408Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.088016Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.476031Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.474522Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.088379Z"
                 }
             },
             "outputs": [],
             "source": [
                 "readstats2, aligned2, filtered2 = targets.align_and_parse(\n",
                 "    df=pacbio_runs,\n",
                 "    mapper=mapper,\n",
@@ -819,55 +819,55 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.835091Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.834802Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.841545Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.840713Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.835061Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.478338Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.477850Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.485247Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.484325Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.478298Z"
                 }
             },
             "outputs": [],
             "source": [
                 "pd.testing.assert_frame_equal(readstats, readstats2, check_like=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.842893Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.842536Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.858587Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.857931Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.842869Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.486800Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.486410Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.496855Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.495906Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.486769Z"
                 }
             },
             "outputs": [],
             "source": [
                 "pd.testing.assert_frame_equal(\n",
                 "    aligned[targets.target_names[0]], aligned2[targets.target_names[0]], check_like=True\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:05.859825Z",
-                    "iopub.status.busy": "2023-06-19T11:21:05.859508Z",
-                    "iopub.status.idle": "2023-06-19T11:21:05.865321Z",
-                    "shell.execute_reply": "2023-06-19T11:21:05.864661Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:05.859805Z"
+                    "iopub.execute_input": "2024-05-23T17:54:14.498370Z",
+                    "iopub.status.busy": "2024-05-23T17:54:14.498013Z",
+                    "iopub.status.idle": "2024-05-23T17:54:14.504543Z",
+                    "shell.execute_reply": "2024-05-23T17:54:14.503585Z",
+                    "shell.execute_reply.started": "2024-05-23T17:54:14.498340Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "pd.testing.assert_frame_equal(\n",
                 "    filtered[targets.target_names[0]],\n",
@@ -889,15 +889,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.9"
         },
         "toc": {
             "nav_menu": {},
             "number_sections": false,
             "sideBar": true,
             "skip_h1_title": false,
             "toc_cell": true,
```

### Comparing `alignparse-0.6.2/tests/profile_recA.ipynb` & `alignparse-0.6.3/tests/profile_recA.ipynb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/tests/test_Targets_objects.ipynb` & `alignparse-0.6.3/tests/test_Targets_objects.ipynb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/tests/test_Targets_parse_alignment.ipynb` & `alignparse-0.6.3/tests/test_Targets_parse_alignment.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997044509556622%*

 * *Differences: {"'cells'": "{2: {'metadata': {'execution': {'iopub.execute_input': '2024-05-23T17:58:14.441391Z', "*

 * *            "'iopub.status.busy': '2024-05-23T17:58:14.440974Z', 'iopub.status.idle': "*

 * *            "'2024-05-23T17:58:16.962091Z', 'shell.execute_reply': '2024-05-23T17:58:16.961075Z', "*

 * *            "'shell.execute_reply.started': '2024-05-23T17:58:14.441347Z'}}}, 4: {'metadata': "*

 * *            "{'execution': {'iopub.execute_input': '2024-05-23T17:58:16.967482Z', "*

 * *            "'iopub.status.busy': '2024-05- […]*

```diff
@@ -16,19 +16,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:20:58.554169Z",
-                    "iopub.status.busy": "2023-06-19T11:20:58.553602Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.254606Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.252878Z",
-                    "shell.execute_reply.started": "2023-06-19T11:20:58.554136Z"
+                    "iopub.execute_input": "2024-05-23T17:58:14.441391Z",
+                    "iopub.status.busy": "2024-05-23T17:58:14.440974Z",
+                    "iopub.status.idle": "2024-05-23T17:58:16.962091Z",
+                    "shell.execute_reply": "2024-05-23T17:58:16.961075Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:14.441347Z"
                 }
             },
             "outputs": [],
             "source": [
                 "import contextlib\n",
                 "import os\n",
                 "import random\n",
@@ -54,33 +54,33 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.258981Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.258199Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.637247Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.636141Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.258944Z"
+                    "iopub.execute_input": "2024-05-23T17:58:16.967482Z",
+                    "iopub.status.busy": "2024-05-23T17:58:16.966907Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.243007Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.242160Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:16.967449Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "There is just one target: ['RecA_PacBio_amplicon']\n",
                         "It has the following features: ['termini5', 'gene', 'spacer', 'barcode', 'termini3', 'variant_tag5', 'variant_tag3']\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 500x300 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -117,19 +117,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.639016Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.638603Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.644576Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.643674Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.638982Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.247685Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.247252Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.254329Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.252852Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.247651Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -158,19 +158,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.646139Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.645832Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.669152Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.667773Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.646112Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.260487Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.259673Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.289276Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.287970Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.260435Z"
                 }
             },
             "outputs": [],
             "source": [
                 "random.seed(1)  # for reproducible output\n",
                 "nts = \"ACGT\"  # valid nucleotides\n",
                 "\n",
@@ -293,19 +293,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.672086Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.671726Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.795929Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.794850Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.672055Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.294786Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.294305Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.348780Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.347963Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.294739Z"
                 }
             },
             "outputs": [],
             "source": [
                 "# NBVAL_IGNORE_OUTPUT\n",
                 "\n",
                 "mapper = alignparse.minimap2.Mapper(alignparse.minimap2.OPTIONS_CODON_DMS)\n",
@@ -338,19 +338,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.797660Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.797272Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.803000Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.802335Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.797636Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.352587Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.352361Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.358553Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.357934Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.352560Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
@@ -373,19 +373,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.804140Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.803835Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.809117Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.808410Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.804118Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.360137Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.359770Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.366284Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.365344Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.360107Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
@@ -409,19 +409,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.810314Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.809987Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.815657Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.814957Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.810288Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.367808Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.367401Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.374405Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.373584Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.367771Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
@@ -445,19 +445,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.816929Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.816593Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.835793Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.835122Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.816903Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.375870Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.375501Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.398309Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.397565Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.375834Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -758,19 +758,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.836956Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.836625Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.843257Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.842714Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.836936Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.399525Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.399195Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.407311Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.406413Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.399501Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -794,35 +794,35 @@
                             "      <th>category</th>\n",
                             "      <th>count</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
+                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
                             "      <td>3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>filtered RecA_PacBio_amplicon</td>\n",
+                            "      <td>aligned RecA_PacBio_amplicon</td>\n",
                             "      <td>3</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>unmapped</td>\n",
                             "      <td>2</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                        category  count\n",
-                            "0   aligned RecA_PacBio_amplicon      3\n",
-                            "1  filtered RecA_PacBio_amplicon      3\n",
+                            "0  filtered RecA_PacBio_amplicon      3\n",
+                            "1   aligned RecA_PacBio_amplicon      3\n",
                             "2                       unmapped      2"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -839,19 +839,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.844361Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.844083Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.849798Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.849128Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.844343Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.409252Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.408685Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.418257Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.417434Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.409200Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "True"
@@ -874,19 +874,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 12,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.850980Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.850648Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.857999Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.857364Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.850958Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.419529Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.419212Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.427824Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.427006Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.419501Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -960,19 +960,19 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {
                 "execution": {
-                    "iopub.execute_input": "2023-06-19T11:21:00.859111Z",
-                    "iopub.status.busy": "2023-06-19T11:21:00.858821Z",
-                    "iopub.status.idle": "2023-06-19T11:21:00.868052Z",
-                    "shell.execute_reply": "2023-06-19T11:21:00.867379Z",
-                    "shell.execute_reply.started": "2023-06-19T11:21:00.859090Z"
+                    "iopub.execute_input": "2024-05-23T17:58:17.429167Z",
+                    "iopub.status.busy": "2024-05-23T17:58:17.428835Z",
+                    "iopub.status.idle": "2024-05-23T17:58:17.440004Z",
+                    "shell.execute_reply": "2024-05-23T17:58:17.439366Z",
+                    "shell.execute_reply.started": "2024-05-23T17:58:17.429138Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -1077,15 +1077,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.9"
         },
         "toc": {
             "nav_menu": {},
             "number_sections": false,
             "sideBar": true,
             "skip_h1_title": false,
             "toc_cell": false,
```

### Comparing `alignparse-0.6.2/tests/test_Targets_parse_alignment_consistency.ipynb` & `alignparse-0.6.3/tests/test_Targets_parse_alignment_consistency.ipynb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/tests/test_cs_tag_Alignment.ipynb` & `alignparse-0.6.3/tests/test_cs_tag_Alignment.ipynb`

 * *Files identical despite different names*

### Comparing `alignparse-0.6.2/tests/test_cs_tag_Alignment_accuracy.ipynb` & `alignparse-0.6.3/tests/test_cs_tag_Alignment_accuracy.ipynb`

 * *Files identical despite different names*

