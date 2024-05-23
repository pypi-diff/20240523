# Comparing `tmp/mkdocs_ai_summary-0.2.0.tar.gz` & `tmp/mkdocs_ai_summary-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ai_summary-0.2.0.tar", last modified: Wed May 22 20:25:11 2024, max compression
+gzip compressed data, was "mkdocs_ai_summary-0.2.1.tar", last modified: Wed May 22 20:52:45 2024, max compression
```

## Comparing `mkdocs_ai_summary-0.2.0.tar` & `mkdocs_ai_summary-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/tongyi_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:52:45.607371 mkdocs_ai_summary-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-22 20:52:45.607371 mkdocs_ai_summary-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:52:45.603371 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/tongyi_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:52:45.603371 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 20:52:45.000000 mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-22 20:52:37.000000 mkdocs_ai_summary-0.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:52:45.607371 mkdocs_ai_summary-0.2.1/setup.cfg
```

### Comparing `mkdocs_ai_summary-0.2.0/LICENSE` & `mkdocs_ai_summary-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.0/PKG-INFO` & `mkdocs_ai_summary-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.0
+Version: 0.2.1
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 # mkdocs-ai-summary
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
 
 Generage an **ai-summary** for the page:
-![](assets/2024-05-23-04-11-20.png)
+![](assets/2024-05-23-04-35-01.png)
 
 Minimal demo: [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
 
 ## Installation
 
@@ -64,25 +64,27 @@
 ```
 or
 ```
 pip install mkdocs-ai-summary[tongyi]
 ```
 > ⚠️⚠️⚠️⚠️
 > 
-> Only support [tongyi ai](https://tongyi.aliyun.com/) and [ChatGPT](https://chat.openai.com/) for now.
+> Only support [ChatGPT](https://chat.openai.com/) and [tongyi ai](https://tongyi.aliyun.com/) for now.
 >  
 >  To use **ChatGPT(default)**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export OPENAI_API_KEY='sk-xxxxxxx'
 >  ```
->
+> [how to get an OPENAI_API_KEY?](https://platform.openai.com/docs/quickstart)
+> 
 >  To use **tongyi ai**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export DASHSCOPE_API_KEY='sk-xxxxxxx'
 >  ```
+> [how to get an DASHSCOPE_API_KEY?](https://dashscope.console.aliyun.com/)
 
 [optional] Then you can include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom  ai summary admonition style**) in the config file as below:
 
 ## Configuration
 
 A demo for `mkdocs.yml`:
```

### Comparing `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/chatgpt_api.py` & `mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/chatgpt_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import json
+import logging
 from hashlib import md5
 from openai import OpenAI
 
 
 def ask(prompt, model="gpt-3.5-turbo"):
     client = OpenAI()
     completion = client.chat.completions.create(
@@ -17,15 +18,21 @@
         ],
     )
 
     return completion.choices[0].message.content
 
 
 def get_summary_chatgpt(
-    page, prompt, markdown, cache=True, cache_dir="./", model="gpt-3.5-turbo"
+    page,
+    prompt,
+    markdown,
+    cache=True,
+    cache_dir="./",
+    model="gpt-3.5-turbo",
+    logger=logging.Logger(""),
 ):
     question = prompt + markdown
     if cache:
         content_md5 = md5(markdown.encode("utf-8")).hexdigest()
         cache_file = f"{cache_dir}_ai_summary_cache2.json"
         if os.path.exists(cache_file):
             with open(cache_file, "r+") as f:
@@ -33,14 +40,15 @@
         else:
             cache_dict = {}
 
         # asked before
         if page in cache_dict:
             if content_md5 == cache_dict[page]["content_md5"]:
                 ai_summary = cache_dict[page]["ai_summary"]
+                logger.info("Using cache.")
             # asked before, but content changed
             else:
                 ai_summary = ask(question, model=model)
         # do not aksed before
         else:
             ai_summary = ask(question, model=model)
             cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
```

### Comparing `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/plugin.py` & `mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                 try:
                     summary = get_summary_tongyi(
                         page=str(page.title),
                         prompt=self.config["prompt"],
                         markdown=markdown_to_summary,
                         cache=self.config["cache"],
                         cache_dir=self.config["cache_dir"],
+                        logger=logger,
                     )
                 except AiSummaryError as e:
                     logger.warning("Ask AI Error", repr(e))
                     return markdown
                 except Exception as e:
                     logger.warning(repr(e))
                     return markdown
@@ -78,14 +79,15 @@
                     summary = get_summary_chatgpt(
                         page=str(page.title),
                         prompt=self.config["prompt"],
                         markdown=markdown_to_summary,
                         cache=self.config["cache"],
                         cache_dir=self.config["cache_dir"],
                         model=self.config["model"],
+                        logger=logger,
                     )
                 except Exception as e:
                     logger.warning(repr(e))
                     return markdown
             case _:
                 e = repr(ConfigurationError("unrecongnized api config."))
                 logger.warning(repr(e))
```

### Comparing `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/tongyi_api.py` & `mkdocs_ai_summary-0.2.1/mkdocs_ai_summary/tongyi_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import json
 import random
 from hashlib import md5
 from http import HTTPStatus
 from dashscope import Generation
+import logging
 
 MAX_LENGTH = 6000
 
 
 class AiSummaryError(Exception):
 
     def __init__(self, *args: object) -> None:
@@ -35,37 +36,39 @@
                 response.status_code,
                 response.code,
                 response.message,
             )
         )
 
 
-def get_summary_tongyi(page, prompt, markdown, cache=True, cache_dir="./"):
+def get_summary_tongyi(
+    page, prompt, markdown, cache=True, cache_dir="./", logger=logging.Logger("")
+):
     question = (prompt + markdown)[: MAX_LENGTH - 10]
     if cache:
         content_md5 = md5(markdown.encode("utf-8")).hexdigest()
         cache_file = f"{cache_dir}_ai_summary_cache.json"
         if os.path.exists(cache_file):
             with open(cache_file, "r+") as f:
                 cache_dict = json.load(f)
         else:
             cache_dict = {}
 
         # asked before
         if page in cache_dict:
             if content_md5 == cache_dict[page]["content_md5"]:
                 ai_summary = cache_dict[page]["ai_summary"]
+                logger.info("Using cache.")
             # asked before, but content changed
             else:
                 ai_summary = ask(question)
         # do not aksed before
         else:
             ai_summary = ask(question)
             cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
             with open(f"{cache_dir}/_ai_summary_cache.json", "w+") as f:
                 cache_dict = json.dump(cache_dict, f)
     else:
         ai_summary = ask(question)
     return f"""!!! tongyiai-summary "AI Summary powered by [通义千问](https://tongyi.aliyun.com/)"
     {ai_summary}
 """
-
```

### Comparing `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/PKG-INFO` & `mkdocs_ai_summary-0.2.1/mkdocs_ai_summary.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.0
+Version: 0.2.1
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,15 +46,15 @@
 # mkdocs-ai-summary
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
 
 Generage an **ai-summary** for the page:
-![](assets/2024-05-23-04-11-20.png)
+![](assets/2024-05-23-04-35-01.png)
 
 Minimal demo: [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
 
 ## Installation
 
@@ -64,25 +64,27 @@
 ```
 or
 ```
 pip install mkdocs-ai-summary[tongyi]
 ```
 > ⚠️⚠️⚠️⚠️
 > 
-> Only support [tongyi ai](https://tongyi.aliyun.com/) and [ChatGPT](https://chat.openai.com/) for now.
+> Only support [ChatGPT](https://chat.openai.com/) and [tongyi ai](https://tongyi.aliyun.com/) for now.
 >  
 >  To use **ChatGPT(default)**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export OPENAI_API_KEY='sk-xxxxxxx'
 >  ```
->
+> [how to get an OPENAI_API_KEY?](https://platform.openai.com/docs/quickstart)
+> 
 >  To use **tongyi ai**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export DASHSCOPE_API_KEY='sk-xxxxxxx'
 >  ```
+> [how to get an DASHSCOPE_API_KEY?](https://dashscope.console.aliyun.com/)
 
 [optional] Then you can include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom  ai summary admonition style**) in the config file as below:
 
 ## Configuration
 
 A demo for `mkdocs.yml`:
```

### Comparing `mkdocs_ai_summary-0.2.0/pyproject.toml` & `mkdocs_ai_summary-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [project]
 name = "mkdocs-ai-summary"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.10"
 dependencies = [
     "mkdocs>=1.5.3",
 ]
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
```

### Comparing `mkdocs_ai_summary-0.2.0/readme.md` & `mkdocs_ai_summary-0.2.1/readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # mkdocs-ai-summary
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
 
 Generage an **ai-summary** for the page:
-![](assets/2024-05-23-04-11-20.png)
+![](assets/2024-05-23-04-35-01.png)
 
 Minimal demo: [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
 
 ## Installation
 
@@ -19,25 +19,27 @@
 ```
 or
 ```
 pip install mkdocs-ai-summary[tongyi]
 ```
 > ⚠️⚠️⚠️⚠️
 > 
-> Only support [tongyi ai](https://tongyi.aliyun.com/) and [ChatGPT](https://chat.openai.com/) for now.
+> Only support [ChatGPT](https://chat.openai.com/) and [tongyi ai](https://tongyi.aliyun.com/) for now.
 >  
 >  To use **ChatGPT(default)**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export OPENAI_API_KEY='sk-xxxxxxx'
 >  ```
->
+> [how to get an OPENAI_API_KEY?](https://platform.openai.com/docs/quickstart)
+> 
 >  To use **tongyi ai**, you should set a Environmental Variable for **api key**:
 >  ```bash
 >  export DASHSCOPE_API_KEY='sk-xxxxxxx'
 >  ```
+> [how to get an DASHSCOPE_API_KEY?](https://dashscope.console.aliyun.com/)
 
 [optional] Then you can include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom  ai summary admonition style**) in the config file as below:
 
 ## Configuration
 
 A demo for `mkdocs.yml`:
```

