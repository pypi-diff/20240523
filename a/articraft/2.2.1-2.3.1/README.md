# Comparing `tmp/articraft-2.2.1.tar.gz` & `tmp/articraft-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articraft-2.2.1.tar", last modified: Thu May 23 04:18:37 2024, max compression
+gzip compressed data, was "articraft-2.3.1.tar", last modified: Thu May 23 04:19:09 2024, max compression
```

## Comparing `articraft-2.2.1.tar` & `articraft-2.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:18:37.932195 articraft-2.2.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.2.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.2.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-05-23 04:18:37.931536 articraft-2.2.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2677 2024-05-23 04:18:19.000000 articraft-2.2.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:18:37.928506 articraft-2.2.1/articraft/
--rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-23 04:18:31.000000 articraft-2.2.1/articraft/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.2.1/articraft/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.2.1/articraft/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.2.1/articraft/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:18:37.930863 articraft-2.2.1/articraft.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-05-23 04:18:37.000000 articraft-2.2.1/articraft.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-23 04:18:37.000000 articraft-2.2.1/articraft.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 04:18:37.000000 articraft-2.2.1/articraft.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-23 04:18:37.000000 articraft-2.2.1/articraft.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-23 04:18:37.000000 articraft-2.2.1/articraft.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.2.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.2.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 04:18:37.932300 articraft-2.2.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.2.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:19:09.430220 articraft-2.3.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-11 05:01:32.000000 articraft-2.3.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 06:03:51.000000 articraft-2.3.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     3605 2024-05-23 04:19:09.429785 articraft-2.3.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2691 2024-05-23 04:19:00.000000 articraft-2.3.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:19:09.426938 articraft-2.3.1/articraft/
+-rw-r--r--   0 kamangir   (502) staff       (20)      100 2024-05-23 04:19:03.000000 articraft-2.3.1/articraft/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      252 2024-05-23 04:15:46.000000 articraft-2.3.1/articraft/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2024-05-23 04:15:48.000000 articraft-2.3.1/articraft/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-11 05:01:32.000000 articraft-2.3.1/articraft/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:19:09.429256 articraft-2.3.1/articraft.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     3605 2024-05-23 04:19:09.000000 articraft-2.3.1/articraft.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      316 2024-05-23 04:19:09.000000 articraft-2.3.1/articraft.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 04:19:09.000000 articraft-2.3.1/articraft.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-23 04:19:09.000000 articraft-2.3.1/articraft.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-23 04:19:09.000000 articraft-2.3.1/articraft.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 06:03:51.000000 articraft-2.3.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-21 06:04:42.000000 articraft-2.3.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 04:19:09.430309 articraft-2.3.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      223 2024-05-23 04:15:33.000000 articraft-2.3.1/setup.py
```

### Comparing `articraft-2.2.1/LICENSE` & `articraft-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `articraft-2.2.1/PKG-INFO` & `articraft-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.2.1
+Version: 2.3.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -25,15 +25,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
-# 🎨 `aiart`
+# 🎨 `aiart` (`articraft`)
 
 🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](https://raw.githubusercontent.com/kamangir/aiart/main/APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
```

### Comparing `articraft-2.2.1/README.md` & `articraft-2.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 🎨 `aiart`
+# 🎨 `aiart` (`articraft`)
 
 🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](./APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
```

### Comparing `articraft-2.2.1/articraft.egg-info/PKG-INFO` & `articraft-2.3.1/articraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articraft
-Version: 2.2.1
+Version: 2.3.1
 Summary: 🎨 tools for ai artists.
 Home-page: https://github.com/kamangir/aiart
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -25,15 +25,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: pylint
 Requires-Dist: pytest
 Requires-Dist: python-dotenv[cli]
 Requires-Dist: requests
 Requires-Dist: tqdm
 
-# 🎨 `aiart`
+# 🎨 `aiart` (`articraft`)
 
 🎨 `aiart` is an interface to [OpenAI](https://github.com/kamangir/openai_cli), [DALL-E](https://github.com/kamangir/openai_cli/blob/main/.abcli/DALLE.sh), and [Stable Diffusion](https://github.com/kamangir/blue-stability). AiArt can ingest [text and poetry](https://github.com/kamangir/aiart/blob/main/aiart/html/functions.py) from [allpoetry.com](https://allpoetry.com/), [medium](https://medium.com/), and [poetryfoundation.org](https://www.poetryfoundation.org/).
 
 🔷 [APIs](https://raw.githubusercontent.com/kamangir/aiart/main/APIs.yaml) 🔷
 
 ```bash
 abcli_quote <message>
```

