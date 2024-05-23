# Comparing `tmp/LaoNLP-1.1.3.tar.gz` & `tmp/laonlp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LaoNLP-1.1.3.tar", last modified: Tue Oct 17 15:10:02 2023, max compression
+gzip compressed data, was "laonlp-1.2.0.tar", last modified: Thu May 23 15:32:29 2024, max compression
```

## Comparing `LaoNLP-1.1.3.tar` & `laonlp-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.200996 LaoNLP-1.1.3/LaoNLP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-17 15:10:02.000000 LaoNLP-1.1.3/LaoNLP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.200996 LaoNLP-1.1.3/laonlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/LICENSE-lao-eng-dictionary
--rw-r--r--   0 runner    (1001) docker     (127)   205310 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/Lao-Dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (127)  2857765 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/lao-eng-dictionary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/lao-wannaphong.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/lao_words.py
--rw-r--r--   0 runner    (1001) docker     (127)   409234 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/lo_spellcheck_dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/mopt_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)  3743688 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/ptagger_SeqLabeling_corpus.json
--rw-r--r--   0 runner    (1001) docker     (127)  5077288 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/ptagger_Yunshan-Cup_corpus.json
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/stopwords_lao.txt
--rw-r--r--   0 runner    (1001) docker     (127)   270905 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/corpus/wiktionary-20210720.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/tag/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/tag/pos_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/tokenize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/translate/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/translate/mopt_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/transliterate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/util/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/util/lao.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/laonlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/laonlp/word_vector/word2vec.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 15:10:02.212996 LaoNLP-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2023-10-17 15:09:48.000000 LaoNLP-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 15:32:22.000000 laonlp-1.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/LaoNLP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 15:32:29.000000 laonlp-1.2.0/LaoNLP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-23 15:32:29.561584 laonlp-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 15:32:22.000000 laonlp-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.541584 laonlp-1.2.0/laonlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.557584 laonlp-1.2.0/laonlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/LICENSE-lao-eng-dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)   205310 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/Lao-Dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2857765 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/lao-eng-dictionary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/lao-wannaphong.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/lao_words.py
+-rw-r--r--   0 runner    (1001) docker     (127)   409234 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/lo_spellcheck_dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/mopt_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3743688 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/ptagger_SeqLabeling_corpus.json
+-rw-r--r--   0 runner    (1001) docker     (127)  5077288 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/ptagger_Yunshan-Cup_corpus.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/stopwords_lao.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   270905 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/corpus/wiktionary-20210720.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.557584 laonlp-1.2.0/laonlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/tag/pos_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.557584 laonlp-1.2.0/laonlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/tokenize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.557584 laonlp-1.2.0/laonlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/translate/mopt_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/laonlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/transliterate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/laonlp/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/util/lao.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/laonlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-23 15:32:22.000000 laonlp-1.2.0/laonlp/word_vector/word2vec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:32:29.561584 laonlp-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-23 15:32:22.000000 laonlp-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:32:29.561584 laonlp-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-23 15:32:22.000000 laonlp-1.2.0/tests/test_word_vector.py
```

### Comparing `LaoNLP-1.1.3/LICENSE` & `laonlp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/LaoNLP.egg-info/PKG-INFO` & `laonlp-1.2.0/LaoNLP.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LaoNLP
-Version: 1.1.3
+Version: 1.2.0
 Summary: Lao Natural Language Processing library
 Home-page: https://github.com/wannaphong/laonlp
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://github.com/wannaphong/LaoNLP/wiki
 Project-URL: Source, https://github.com/wannaphong/LaoNLP
@@ -16,17 +16,24 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: word_vector
-Provides-Extra: full
 License-File: LICENSE
+Requires-Dist: pythainlp>=3.0.0
+Provides-Extra: word-vector
+Requires-Dist: scipy<1.11.0; extra == "word-vector"
+Requires-Dist: gensim; extra == "word-vector"
+Requires-Dist: huggingface-hub; extra == "word-vector"
+Provides-Extra: full
+Requires-Dist: scipy<1.11.0; extra == "full"
+Requires-Dist: gensim; extra == "full"
+Requires-Dist: huggingface-hub; extra == "full"
 
 # LaoNLP
 [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&link=https://github.com/sponsors/wannaphong/)](https://github.com/sponsors/wannaphong/)
 [![Downloads](https://pepy.tech/badge/laonlp)](https://pepy.tech/project/laonlp)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6833407.svg)](https://doi.org/10.5281/zenodo.6833407)
 [![Coverage Status](https://coveralls.io/repos/github/wannaphong/LaoNLP/badge.svg?branch=master)](https://coveralls.io/github/wannaphong/LaoNLP?branch=master)
 
@@ -87,15 +94,15 @@
   url          = {https://doi.org/10.5281/zenodo.6833407}
 }
 ```
 
 ## License
 
 ```
-   Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+   Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/LaoNLP.egg-info/SOURCES.txt` & `laonlp-1.2.0/LaoNLP.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -27,8 +27,15 @@
 laonlp/translate/__init__.py
 laonlp/translate/mopt_dict.py
 laonlp/transliterate/__init__.py
 laonlp/util/__init__.py
 laonlp/util/digitconv.py
 laonlp/util/lao.py
 laonlp/word_vector/__init__.py
-laonlp/word_vector/word2vec.py
+laonlp/word_vector/word2vec.py
+tests/test_corpus.py
+tests/test_tag.py
+tests/test_tokenize.py
+tests/test_translate.py
+tests/test_transliterate.py
+tests/test_util.py
+tests/test_word_vector.py
```

### Comparing `LaoNLP-1.1.3/PKG-INFO` & `laonlp-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LaoNLP
-Version: 1.1.3
+Version: 1.2.0
 Summary: Lao Natural Language Processing library
 Home-page: https://github.com/wannaphong/laonlp
 Author: Wannaphong
 Author-email: wannaphong@yahoo.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://github.com/wannaphong/LaoNLP/wiki
 Project-URL: Source, https://github.com/wannaphong/LaoNLP
@@ -16,17 +16,24 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: word_vector
-Provides-Extra: full
 License-File: LICENSE
+Requires-Dist: pythainlp>=3.0.0
+Provides-Extra: word-vector
+Requires-Dist: scipy<1.11.0; extra == "word-vector"
+Requires-Dist: gensim; extra == "word-vector"
+Requires-Dist: huggingface-hub; extra == "word-vector"
+Provides-Extra: full
+Requires-Dist: scipy<1.11.0; extra == "full"
+Requires-Dist: gensim; extra == "full"
+Requires-Dist: huggingface-hub; extra == "full"
 
 # LaoNLP
 [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&link=https://github.com/sponsors/wannaphong/)](https://github.com/sponsors/wannaphong/)
 [![Downloads](https://pepy.tech/badge/laonlp)](https://pepy.tech/project/laonlp)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6833407.svg)](https://doi.org/10.5281/zenodo.6833407)
 [![Coverage Status](https://coveralls.io/repos/github/wannaphong/LaoNLP/badge.svg?branch=master)](https://coveralls.io/github/wannaphong/LaoNLP?branch=master)
 
@@ -87,15 +94,15 @@
   url          = {https://doi.org/10.5281/zenodo.6833407}
 }
 ```
 
 ## License
 
 ```
-   Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+   Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/README.md` & `laonlp-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
   url          = {https://doi.org/10.5281/zenodo.6833407}
 }
 ```
 
 ## License
 
 ```
-   Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+   Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/__init__.py` & `laonlp-1.2.0/laonlp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/corpus/LICENSE-lao-eng-dictionary` & `laonlp-1.2.0/laonlp/corpus/LICENSE-lao-eng-dictionary`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/Lao-Dictionary.txt` & `laonlp-1.2.0/laonlp/corpus/Lao-Dictionary.txt`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/__init__.py` & `laonlp-1.2.0/laonlp/corpus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/corpus/core.py` & `laonlp-1.2.0/laonlp/corpus/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/corpus/lao-eng-dictionary.csv` & `laonlp-1.2.0/laonlp/corpus/lao-eng-dictionary.csv`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/lao_words.py` & `laonlp-1.2.0/laonlp/corpus/lao_words.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/corpus/lo_spellcheck_dict.txt` & `laonlp-1.2.0/laonlp/corpus/lo_spellcheck_dict.txt`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/mopt_dict.py` & `laonlp-1.2.0/laonlp/corpus/mopt_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/corpus/ptagger_SeqLabeling_corpus.json` & `laonlp-1.2.0/laonlp/corpus/ptagger_SeqLabeling_corpus.json`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/ptagger_Yunshan-Cup_corpus.json` & `laonlp-1.2.0/laonlp/corpus/ptagger_Yunshan-Cup_corpus.json`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/stopwords_lao.txt` & `laonlp-1.2.0/laonlp/corpus/stopwords_lao.txt`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/corpus/wiktionary-20210720.txt` & `laonlp-1.2.0/laonlp/corpus/wiktionary-20210720.txt`

 * *Files identical despite different names*

### Comparing `LaoNLP-1.1.3/laonlp/tag/__init__.py` & `laonlp-1.2.0/laonlp/tag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/tag/pos_tag.py` & `laonlp-1.2.0/laonlp/tag/pos_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/tokenize/__init__.py` & `laonlp-1.2.0/laonlp/tokenize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/translate/__init__.py` & `laonlp-1.2.0/laonlp/translate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/translate/mopt_dict.py` & `laonlp-1.2.0/laonlp/translate/mopt_dict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/transliterate/__init__.py` & `laonlp-1.2.0/laonlp/transliterate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/util/__init__.py` & `laonlp-1.2.0/laonlp/util/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -13,16 +13,18 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 __all__ = [
     "lao_digit_to_arabic_digit",
     "arabic_digit_to_lao_digit",
+    "num_to_laoword",
     "remove_tone_mark",
 ]
 from laonlp.util.digitconv import (
     lao_digit_to_arabic_digit,
     arabic_digit_to_lao_digit,
+    num_to_laoword,
 )
 from laonlp.util.lao import (
     remove_tone_mark
 )
```

### Comparing `LaoNLP-1.1.3/laonlp/util/lao.py` & `laonlp-1.2.0/laonlp/util/lao.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/word_vector/__init__.py` & `laonlp-1.2.0/laonlp/word_vector/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/laonlp/word_vector/word2vec.py` & `laonlp-1.2.0/laonlp/word_vector/word2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `LaoNLP-1.1.3/setup.py` & `laonlp-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright 2020 - 2023 Wannaphong Phatthiyaphaibun
+Copyright 2020 - 2024 Wannaphong Phatthiyaphaibun
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -19,24 +19,25 @@
 with open("README.md", "r", encoding="utf-8-sig") as f:
     readme = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8-sig") as f:
     requirements = [i.strip() for i in f.readlines()]
 
 extras = {
-    "word_vector": ["gensim", "huggingface-hub"],
+    "word_vector": ["scipy<1.11.0", "gensim", "huggingface-hub"],
     "full": [
+        "scipy<1.11.0",
         "gensim",
         "huggingface-hub"
     ]
 }
 
 setup(
     name="LaoNLP",
-    version="1.1.3",
+    version="1.2.0",
     description="Lao Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Wannaphong",
     author_email="wannaphong@yahoo.com",
     url="https://github.com/wannaphong/laonlp",
     packages=find_packages(exclude=["tests"]),
```

