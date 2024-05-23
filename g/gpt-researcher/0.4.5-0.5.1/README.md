# Comparing `tmp/gpt-researcher-0.4.5.tar.gz` & `tmp/gpt-researcher-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.4.5.tar", last modified: Tue May 14 16:20:13 2024, max compression
+gzip compressed data, was "gpt-researcher-0.5.1.tar", last modified: Thu May 23 13:07:56 2024, max compression
```

## Comparing `gpt-researcher-0.4.5.tar` & `gpt-researcher-0.5.1.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.753459 gpt-researcher-0.4.5/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    11555 2024-05-14 16:20:13.752350 gpt-researcher-0.4.5/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    10832 2024-05-14 15:51:21.000000 gpt-researcher-0.4.5/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.700639 gpt-researcher-0.4.5/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.701296 gpt-researcher-0.4.5/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.702616 gpt-researcher-0.4.5/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.704206 gpt-researcher-0.4.5/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.4.5/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.4.5/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.704837 gpt-researcher-0.4.5/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.4.5/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.710084 gpt-researcher-0.4.5/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.4.5/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2108 2024-05-14 16:19:40.000000 gpt-researcher-0.4.5/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.712207 gpt-researcher-0.4.5/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.4.5/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.4.5/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.4.5/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.713109 gpt-researcher-0.4.5/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.714374 gpt-researcher-0.4.5/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.715564 gpt-researcher-0.4.5/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.717245 gpt-researcher-0.4.5/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.4.5/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.721017 gpt-researcher-0.4.5/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.4.5/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     9331 2024-05-10 05:37:26.000000 gpt-researcher-0.4.5/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.4.5/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.4.5/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.722627 gpt-researcher-0.4.5/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.4.5/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.4.5/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.723471 gpt-researcher-0.4.5/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.725081 gpt-researcher-0.4.5/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.726700 gpt-researcher-0.4.5/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.728747 gpt-researcher-0.4.5/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.730793 gpt-researcher-0.4.5/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.732170 gpt-researcher-0.4.5/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.734070 gpt-researcher-0.4.5/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.736139 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.737702 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.739297 gpt-researcher-0.4.5/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.741035 gpt-researcher-0.4.5/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.742320 gpt-researcher-0.4.5/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.744245 gpt-researcher-0.4.5/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.745985 gpt-researcher-0.4.5/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.747584 gpt-researcher-0.4.5/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.4.5/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.751081 gpt-researcher-0.4.5/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.4.5/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.4.5/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-14 16:20:13.708770 gpt-researcher-0.4.5/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    11555 2024-05-14 16:20:13.000000 gpt-researcher-0.4.5/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-14 16:20:13.000000 gpt-researcher-0.4.5/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-14 16:20:13.000000 gpt-researcher-0.4.5/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-14 16:20:13.000000 gpt-researcher-0.4.5/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-14 16:20:13.000000 gpt-researcher-0.4.5/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.4.5/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-14 16:20:13.753803 gpt-researcher-0.4.5/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-14 16:19:14.000000 gpt-researcher-0.4.5/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.210263 gpt-researcher-0.5.1/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:07:56.209420 gpt-researcher-0.5.1/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    12159 2024-05-23 11:18:14.000000 gpt-researcher-0.5.1/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.143611 gpt-researcher-0.5.1/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.144427 gpt-researcher-0.5.1/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.146011 gpt-researcher-0.5.1/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.147425 gpt-researcher-0.5.1/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.1/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.148609 gpt-researcher-0.5.1/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.153520 gpt-researcher-0.5.1/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.158984 gpt-researcher-0.5.1/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.1/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.160966 gpt-researcher-0.5.1/gpt_researcher/document/
+-rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/document/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/document/document.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.162286 gpt-researcher-0.5.1/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.164500 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.166120 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.167658 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.172222 gpt-researcher-0.5.1/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.1/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    14872 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.174605 gpt-researcher-0.5.1/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.5.1/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.175727 gpt-researcher-0.5.1/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      500 2024-05-23 13:00:48.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.177210 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.179434 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.181403 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.183486 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.185478 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.187304 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.189154 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2028 2024-05-23 13:06:48.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.190703 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1152 2024-05-23 13:04:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/yahoo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.192795 gpt-researcher-0.5.1/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.194812 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.196899 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.198929 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.200888 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.203013 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.207885 gpt-researcher-0.5.1/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.151890 gpt-researcher-0.5.1/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2781 2024-05-23 13:07:56.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      393 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-23 13:07:56.210489 gpt-researcher-0.5.1/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-23 13:07:51.000000 gpt-researcher-0.5.1/setup.py
```

### Comparing `gpt-researcher-0.4.5/LICENSE` & `gpt-researcher-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/PKG-INFO` & `gpt-researcher-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.4.5
+Version: 0.5.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔎 GPT Researcher
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.gg/MN9M86kb)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
 -  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
 -  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
@@ -60,30 +61,30 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Tutorials
- - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
+ - [How it Works](https://docs.gptr.dev/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
-- 📝 Generate research, outlines, resources and lessons reports
+- 📝 Generate research, outlines, resources and lessons reports with local documents and web sources
 - 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
-Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
+Please see [here](https://docs.gptr.dev/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
@@ -125,48 +126,70 @@
 uvicorn main:app --reload
 ```
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
-**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
+**To learn how to get started with [Docker](https://docs.gptr.dev/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.gptr.dev/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.gptr.dev/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.gptr.dev/docs/gpt-researcher/getting-started) page.**
 
 ### Run as PIP package
 ```bash
 pip install gpt-researcher
 ```
 
 ```python
+...
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
 research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
+...
 ```
 
-**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.gptr.dev/docs/gpt-researcher/pip-package) page.**
+
+## 📄 Research on Local Documents
+
+You can instruct the GPT Researcher to run research tasks based on your local documents. Currently supported file formats are: PDF, plain text, CSV, Excel, Markdown, PowerPoint, and Word documents.
+
+Step 1: Add the env variable `DOC_PATH` pointing to the folder where your documents are located.
+
+```bash
+export DOC_PATH="./my-docs"
+```
+
+Step 2: 
+ - If you're running the frontend app on localhost:8000, simply select "My Documents" from the the "Report Source" Dropdown Options.
+ - If you're running GPT Researcher with the [PIP package](https://docs.tavily.com/docs/gpt-researcher/pip-package), pass the `report_source` argument as "documents" when you instantiate the `GPTResearcher` class [code sample here](https://docs.tavily.com/docs/gpt-researcher/tailored-research).
+
+### One-Click Deployment
+
+[![Deploy to RepoCloud](https://d16t0pc4846x52.cloudfront.net/deploylobe.svg)](https://repocloud.io/details/?app_id=274)
 
 ## 👪 Multi-Agent Assistant
 As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
 
 By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
 
 An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
 
-Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.gptr.dev/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
-
+<a href="https://github.com/assafelovic/gpt-researcher/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=assafelovic/gpt-researcher" />
+</a>
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
```

### Comparing `gpt-researcher-0.4.5/README.md` & `gpt-researcher-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # 🔎 GPT Researcher
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.gg/MN9M86kb)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
 -  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
 -  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
@@ -42,30 +43,30 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Tutorials
- - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
+ - [How it Works](https://docs.gptr.dev/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
-- 📝 Generate research, outlines, resources and lessons reports
+- 📝 Generate research, outlines, resources and lessons reports with local documents and web sources
 - 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
-Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
+Please see [here](https://docs.gptr.dev/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
@@ -107,48 +108,70 @@
 uvicorn main:app --reload
 ```
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
-**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
+**To learn how to get started with [Docker](https://docs.gptr.dev/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.gptr.dev/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.gptr.dev/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.gptr.dev/docs/gpt-researcher/getting-started) page.**
 
 ### Run as PIP package
 ```bash
 pip install gpt-researcher
 ```
 
 ```python
+...
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
 research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
+...
 ```
 
-**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.gptr.dev/docs/gpt-researcher/pip-package) page.**
+
+## 📄 Research on Local Documents
+
+You can instruct the GPT Researcher to run research tasks based on your local documents. Currently supported file formats are: PDF, plain text, CSV, Excel, Markdown, PowerPoint, and Word documents.
+
+Step 1: Add the env variable `DOC_PATH` pointing to the folder where your documents are located.
+
+```bash
+export DOC_PATH="./my-docs"
+```
+
+Step 2: 
+ - If you're running the frontend app on localhost:8000, simply select "My Documents" from the the "Report Source" Dropdown Options.
+ - If you're running GPT Researcher with the [PIP package](https://docs.tavily.com/docs/gpt-researcher/pip-package), pass the `report_source` argument as "documents" when you instantiate the `GPTResearcher` class [code sample here](https://docs.tavily.com/docs/gpt-researcher/tailored-research).
+
+### One-Click Deployment
+
+[![Deploy to RepoCloud](https://d16t0pc4846x52.cloudfront.net/deploylobe.svg)](https://repocloud.io/details/?app_id=274)
 
 ## 👪 Multi-Agent Assistant
 As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
 
 By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
 
 An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
 
-Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.gptr.dev/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
-
+<a href="https://github.com/assafelovic/gpt-researcher/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=assafelovic/gpt-researcher" />
+</a>
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
```

### Comparing `gpt-researcher-0.4.5/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.5.1/backend/report_type/basic_report/basic_report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from gpt_researcher.master.agent import GPTResearcher
 from fastapi import WebSocket
 
 class BasicReport():
-    def __init__(self, query: str, report_type: str, source_urls, config_path: str, websocket: WebSocket):
+    def __init__(self, query: str, report_type: str, report_source:str, source_urls, config_path: str, websocket: WebSocket):
         self.query = query
         self.report_type = report_type
+        self.report_source = report_source
         self.source_urls = source_urls
         self.config_path = config_path
         self.websocket = websocket
         
     async def run(self):
         # Initialize researcher
-        researcher = GPTResearcher(self.query, self.report_type, self.source_urls, self.config_path, self.websocket)
+        researcher = GPTResearcher(self.query, self.report_type, self.report_source, self.source_urls, self.config_path, self.websocket)
         
         # Run research
         await researcher.conduct_research()
         
         # and generate report        
         report = await researcher.write_report()
```

### Comparing `gpt-researcher-0.4.5/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.5.1/backend/report_type/detailed_report/detailed_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 from gpt_researcher.master.agent import GPTResearcher
 from gpt_researcher.master.functions import (add_source_urls, extract_headers,
                                              table_of_contents)
 
 
 class DetailedReport():
-    def __init__(self, query: str, source_urls, config_path: str, websocket: WebSocket, subtopics=[]):
+    def __init__(self, query: str, report_type: str, report_source: str, source_urls, config_path: str, websocket: WebSocket, subtopics=[]):
         self.query = query
+        self.report_type = report_type
+        self.report_source = report_source
         self.source_urls = source_urls
         self.config_path = config_path
         self.websocket = websocket
         self.subtopics = subtopics
         
         # A parent task assistant. Adding research_report as default
-        self.main_task_assistant = GPTResearcher(self.query, "research_report", self.source_urls, self.config_path, self.websocket)
-
+        self.main_task_assistant = GPTResearcher(self.query, "research_report", self.report_source, self.source_urls, self.config_path, self.websocket)
         self.existing_headers = []
         # This is a global variable to store the entire context accumulated at any point through searching and scraping
         self.global_context = []
     
         # This is a global variable to store the entire url list accumulated at any point through searching and scraping
         if self.source_urls:
             self.global_urls = set(self.source_urls)
```

### Comparing `gpt-researcher-0.4.5/backend/server.py` & `gpt-researcher-0.5.1/backend/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         while True:
             data = await websocket.receive_text()
             if data.startswith("start"):
                 json_data = json.loads(data[6:])
                 task = json_data.get("task")
                 report_type = json_data.get("report_type")
                 filename = f"task_{int(time.time())}_{task}"
+                report_source = json_data.get("report_source")
                 if task and report_type:
-                    report = await manager.start_streaming(task, report_type, websocket)
+                    report = await manager.start_streaming(task, report_type, report_source, websocket)
                     # Saving report as pdf
                     pdf_path = await write_md_to_pdf(report, filename)
                     # Saving report as docx
                     docx_path = await write_md_to_word(report, filename)
                     # Returning the path of saved report files
                     md_path = await write_text_to_md(report, filename)
                     await websocket.send_json({"type": "path", "output": {"pdf": pdf_path, "docx": docx_path, "md": md_path}})
```

### Comparing `gpt-researcher-0.4.5/backend/utils.py` & `gpt-researcher-0.5.1/backend/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,81 @@
 import aiofiles
 import urllib
-import uuid
-from md2pdf.core import md2pdf
 import mistune
-from docx import Document
-from htmldocx import HtmlToDocx
+
 
 async def write_to_file(filename: str, text: str) -> None:
     """Asynchronously write text to a file in UTF-8 encoding.
 
     Args:
         filename (str): The filename to write to.
         text (str): The text to write.
     """
     # Convert text to UTF-8, replacing any problematic characters
     text_utf8 = text.encode('utf-8', errors='replace').decode('utf-8')
 
     async with aiofiles.open(filename, "w", encoding='utf-8') as file:
         await file.write(text_utf8)
 
+
 async def write_text_to_md(text: str, filename: str = "") -> str:
     """Writes text to a Markdown file and returns the file path.
 
     Args:
         text (str): Text to write to the Markdown file.
 
     Returns:
         str: The file path of the generated Markdown file.
     """
-    file_path = f"outputs/{filename}.md"
+    file_path = f"outputs/{filename[:60]}.md"
     await write_to_file(file_path, text)
     return file_path
 
+
 async def write_md_to_pdf(text: str, filename: str = "") -> str:
     """Converts Markdown text to a PDF file and returns the file path.
 
     Args:
         text (str): Markdown text to convert.
 
     Returns:
         str: The encoded file path of the generated PDF.
     """
-    file_path = f"outputs/{filename}.pdf"
+    file_path = f"outputs/{filename[:60]}.pdf"
 
     try:
+        from md2pdf.core import md2pdf
         md2pdf(file_path,
                md_content=text,
                #md_file_path=f"{file_path}.md",
                css_file_path="./frontend/pdf_styles.css",
                base_url=None)
         print(f"Report written to {file_path}.pdf")
     except Exception as e:
         print(f"Error in converting Markdown to PDF: {e}")
         return ""
 
     encoded_file_path = urllib.parse.quote(file_path)
     return encoded_file_path
 
+
 async def write_md_to_word(text: str, filename: str = "") -> str:
     """Converts Markdown text to a DOCX file and returns the file path.
 
     Args:
         text (str): Markdown text to convert.
 
     Returns:
         str: The encoded file path of the generated DOCX.
     """
-    file_path = f"outputs/{filename}.docx"
+    file_path = f"outputs/{filename[:60]}.docx"
 
     try:
+        from docx import Document
+        from htmldocx import HtmlToDocx
         # Convert report markdown to HTML
         html = mistune.html(text)
         # Create a document object
         doc = Document()
         # Convert the html generated from the report to document format
         HtmlToDocx().add_html_to_document(html, doc)
```

### Comparing `gpt-researcher-0.4.5/backend/websocket_manager.py` & `gpt-researcher-0.5.1/backend/websocket_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,31 +48,32 @@
         if websocket in self.active_connections:
             self.active_connections.remove(websocket)
             self.sender_tasks[websocket].cancel()
             await self.message_queues[websocket].put(None)
             del self.sender_tasks[websocket]
             del self.message_queues[websocket]
 
-    async def start_streaming(self, task, report_type, websocket):
+    async def start_streaming(self, task, report_type, report_source, websocket):
         """Start streaming the output."""
-        report = await run_agent(task, report_type, websocket)
+        report = await run_agent(task, report_type, report_source, websocket)
         return report
 
 
-async def run_agent(task, report_type, websocket):
+async def run_agent(task, report_type, report_source, websocket):
     """Run the agent."""
     # measure time
     start_time = datetime.datetime.now()
     # add customized JSON config file path here
     config_path = ""
     # Instead of running the agent directly run it through the different report type classes
     if report_type == ReportType.DetailedReport.value:
-        researcher = DetailedReport(query=task, source_urls=None, config_path=config_path, websocket=websocket)
+        researcher = DetailedReport(query=task, report_type=report_type, report_source=report_source,
+                                    source_urls=None, config_path=config_path, websocket=websocket)
     else:
-        researcher = BasicReport(query=task, report_type=report_type,
+        researcher = BasicReport(query=task, report_type=report_type, report_source=report_source,
                                  source_urls=None, config_path=config_path, websocket=websocket)
 
     report = await researcher.run()
     # measure time
     end_time = datetime.datetime.now()
     await websocket.send_json({"type": "logs", "output": f"\nTotal run time: {end_time - start_time}\n"})
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/context/compression.py` & `gpt-researcher-0.5.1/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/context/retriever.py` & `gpt-researcher-0.5.1/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/openai.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         llm = ChatOpenAI(
             model=self.model,
             temperature=self.temperature,
             max_tokens=self.max_tokens,
             api_key=self.api_key
         )
         if self.base_url:
-            llm.base_url = self.base_url
+            llm.openai_api_base = self.base_url
 
         return llm
 
     async def get_chat_response(self, messages, stream, websocket=None):
         if not stream:
             # Getting output from the model chain using ainvoke for asynchronous invoking
             output = await self.llm.ainvoke(messages)
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/master/agent.py` & `gpt-researcher-0.5.1/gpt_researcher/master/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import asyncio
 import time
 
 from gpt_researcher.config import Config
 from gpt_researcher.context.compression import ContextCompressor
+from gpt_researcher.document import DocumentLoader
 from gpt_researcher.master.functions import *
 from gpt_researcher.memory import Memory
-from gpt_researcher.utils.enum import ReportType
+from gpt_researcher.utils.enum import ReportSource, ReportType
 
 
 class GPTResearcher:
     """
     GPT Researcher
     """
 
     def __init__(
         self,
         query: str,
         report_type: str = ReportType.ResearchReport.value,
+        report_source=ReportSource.Web.value,
         source_urls=None,
         config_path=None,
         websocket=None,
         agent=None,
         role=None,
         parent_query: str = "",
         subtopics: list = [],
         visited_urls: set = set(),
         verbose: bool = True,
+        context=[]
     ):
         """
         Initialize the GPT Researcher class.
         Args:
             query: str,
             report_type: str
             source_urls
@@ -42,18 +45,19 @@
             visited_urls: set
         """
         self.query = query
         self.agent = agent
         self.role = role
         self.report_type = report_type
         self.report_prompt = get_prompt_by_report_type(self.report_type)  # this validates the report type
+        self.report_source = report_source
         self.websocket = websocket
         self.cfg = Config(config_path)
         self.retriever = get_retriever(self.cfg.retriever)
-        self.context = []
+        self.context = context
         self.source_urls = source_urls
         self.memory = Memory(self.cfg.embedding_provider)
         self.visited_urls = visited_urls
         self.verbose = verbose
 
         # Only relevant for DETAILED REPORTS
         # --------------------------------------
@@ -76,51 +80,62 @@
             self.agent, self.role = await choose_agent(self.query, self.cfg, self.parent_query)
 
         if self.verbose:
             await stream_output("logs", self.agent, self.websocket)
 
         # If specified, the researcher will use the given urls as the context for the research.
         if self.source_urls:
-            self.context = await self.get_context_by_urls(self.source_urls)
+            context = await self.get_context_by_urls(self.source_urls)
+            
+        elif self.report_source == ReportSource.Local.value:
+            document_data = await DocumentLoader(self.cfg.doc_path).load()
+            context = await self.get_context_by_search(self.query, document_data)
+        
         else:
-            self.context = await self.get_context_by_search(self.query)
+            context = await self.get_context_by_search(self.query)
 
+        # Extending the global context (This is useful instead of setting the context directly above to avoid over-writing input context)
+        self.context.extend(context)
+        
         time.sleep(2)
 
         return self.context
 
     async def write_report(self, existing_headers: list = []):
         """
         Writes the report based on research conducted
 
         Returns:
             str: The report
         """
+
         if self.verbose:
             await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
 
         if self.report_type == "custom_report":
             self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
         elif self.report_type == "subtopic_report":
             report = await generate_report(
                 query=self.query,
                 context=self.context,
                 agent_role_prompt=self.role,
                 report_type=self.report_type,
+                report_source=self.report_source,
                 websocket=self.websocket,
                 cfg=self.cfg,
                 main_topic=self.parent_query,
                 existing_headers=existing_headers
             )
         else:
             report = await generate_report(
                 query=self.query,
                 context=self.context,
                 agent_role_prompt=self.role,
                 report_type=self.report_type,
+                report_source=self.report_source,
                 websocket=self.websocket,
                 cfg=self.cfg
             )
 
         return report
 
     async def get_context_by_urls(self, urls):
@@ -131,15 +146,15 @@
         if self.verbose:
             await stream_output("logs",
                             f"🧠 I will conduct my research based on the following urls: {new_search_urls}...",
                             self.websocket)
         scraped_sites = scrape_urls(new_search_urls, self.cfg)
         return await self.get_similar_content_by_query(self.query, scraped_sites)
 
-    async def get_context_by_search(self, query):
+    async def get_context_by_search(self, query, scraped_data: list = []):
         """
            Generates the context for the research task by searching the query and scraping the results
         Returns:
             context: List of context
         """
         context = []
         # Generate Sub-Queries including original query
@@ -151,31 +166,34 @@
 
         if self.verbose:
             await stream_output("logs",
                                 f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
                                 self.websocket)
 
         # Using asyncio.gather to process the sub_queries asynchronously
-        context = await asyncio.gather(*[self.process_sub_query(sub_query) for sub_query in sub_queries])
+        context = await asyncio.gather(*[self.process_sub_query(sub_query, scraped_data) for sub_query in sub_queries])
         return context
 
-    async def process_sub_query(self, sub_query: str):
+    async def process_sub_query(self, sub_query: str, scraped_data: list = []):
         """Takes in a sub query and scrapes urls based on it and gathers context.
 
         Args:
             sub_query (str): The sub-query generated from the original query
+            scraped_data (list): Scraped data passed in
 
         Returns:
             str: The context gathered from search
         """
         if self.verbose:
             await stream_output("logs", f"\n🔎 Running research for '{sub_query}'...", self.websocket)
 
-        scraped_sites = await self.scrape_sites_by_query(sub_query)
-        content = await self.get_similar_content_by_query(sub_query, scraped_sites)
+        if not scraped_data:
+            scraped_data = await self.scrape_data_by_query(sub_query)
+
+        content = await self.get_similar_content_by_query(sub_query, scraped_data)
 
         if content and self.verbose:
             await stream_output("logs", f"📃 {content}", self.websocket)
         elif self.verbose:
             await stream_output("logs", f"🤷 No content found for '{sub_query}'...", self.websocket)
         return content
 
@@ -191,15 +209,15 @@
                 self.visited_urls.add(url)
                 new_urls.append(url)
                 if self.verbose:
                     await stream_output("logs", f"✅ Added source url to research: {url}\n", self.websocket)
 
         return new_urls
 
-    async def scrape_sites_by_query(self, sub_query):
+    async def scrape_data_by_query(self, sub_query):
         """
         Runs a sub-query
         Args:
             sub_query:
 
         Returns:
             Summary
@@ -209,23 +227,28 @@
         search_results = retriever.search(
             max_results=self.cfg.max_search_results_per_query)
         new_search_urls = await self.get_new_urls([url.get("href") for url in search_results])
 
         # Scrape Urls
         if self.verbose:
             await stream_output("logs", f"🤔 Researching for relevant information...\n", self.websocket)
+
+        # Scrape Urls
         scraped_content_results = scrape_urls(new_search_urls, self.cfg)
         return scraped_content_results
 
     async def get_similar_content_by_query(self, query, pages):
         if self.verbose:
             await stream_output("logs", f"📝 Getting relevant content based on query: {query}...", self.websocket)
+
         # Summarize Raw Data
         context_compressor = ContextCompressor(
-            documents=pages, embeddings=self.memory.get_embeddings())
+            documents=pages,
+            embeddings=self.memory.get_embeddings()
+        )
         # Run Tasks
         return context_compressor.get_context(query, max_results=8)
 
     ########################################################################################
 
     # DETAILED REPORT
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/master/functions.py` & `gpt-researcher-0.5.1/gpt_researcher/master/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import markdown
 
 from gpt_researcher.master.prompts import *
 from gpt_researcher.scraper.scraper import Scraper
 from gpt_researcher.utils.llm import *
 
+
 def get_retriever(retriever):
     """
     Gets the retriever
     Args:
         retriever: retriever name
 
     Returns:
@@ -27,16 +28,14 @@
         case "google":
             from gpt_researcher.retrievers import GoogleSearch
             retriever = GoogleSearch
         case "searx":
             from gpt_researcher.retrievers import SearxSearch
             retriever = SearxSearch
         case "serpapi":
-            raise NotImplementedError(
-                "SerpApiSearch is not fully implemented yet.")
             from gpt_researcher.retrievers import SerpApiSearch
             retriever = SerpApiSearch
         case "googleSerp":
             from gpt_researcher.retrievers import SerperSearch
             retriever = SerperSearch
         case "duckduckgo":
             from gpt_researcher.retrievers import Duckduckgo
@@ -76,15 +75,15 @@
         )
         agent_dict = json.loads(response)
         return agent_dict["server"], agent_dict["agent_role_prompt"]
     except Exception as e:
         return "Default Agent", "You are an AI critical thinker research assistant. Your sole purpose is to write well written, critically acclaimed, objective and structured reports on given text."
 
 
-async def get_sub_queries(query: str, agent_role_prompt: str, cfg, parent_query: str, report_type:str):
+async def get_sub_queries(query: str, agent_role_prompt: str, cfg, parent_query: str, report_type: str):
     """
     Gets the sub queries
     Args:
         query: original query
         agent_role_prompt: agent role prompt
         cfg: Config
 
@@ -97,14 +96,17 @@
         model=cfg.smart_llm_model,
         messages=[
             {"role": "system", "content": f"{agent_role_prompt}"},
             {"role": "user", "content": generate_search_queries_prompt(query, parent_query, report_type, max_iterations=max_research_iterations)}],
         temperature=0,
         llm_provider=cfg.llm_provider
     )
+
+    print("response : ", response)
+
     sub_queries = json.loads(response)
     return sub_queries
 
 
 def scrape_urls(urls, cfg=None):
     """
     Scrapes the urls
@@ -200,18 +202,19 @@
         )
     except Exception as e:
         print(f"{Fore.RED}Error in summarize: {e}{Style.RESET_ALL}")
     return summary
 
 
 async def generate_report(
-    query,
+    query: str,
     context,
-    agent_role_prompt,
-    report_type,
+    agent_role_prompt: str,
+    report_type: str,
+    report_source: str,
     websocket,
     cfg,
     main_topic: str = "",
     existing_headers: list = []
 ):
     """
     generates the final report
@@ -231,16 +234,15 @@
     """
     generate_prompt = get_prompt_by_report_type(report_type)
     report = ""
 
     if report_type == "subtopic_report":
         content = f"{generate_prompt(query, existing_headers, main_topic, context, cfg.report_format, cfg.total_words)}"
     else:
-        content = (
-            f"{generate_prompt(query, context, cfg.report_format, cfg.total_words)}")
+        content = f"{generate_prompt(query, context, report_source, cfg.report_format, cfg.total_words)}"
 
     try:
         report = await create_chat_completion(
             model=cfg.smart_llm_model,
             messages=[
                 {"role": "system", "content": f"{agent_role_prompt}"},
                 {"role": "user", "content": content}],
@@ -268,14 +270,15 @@
     """
     if not websocket or logging:
         print(output)
 
     if websocket:
         await websocket.send_json({"type": type, "output": output})
 
+
 async def get_report_introduction(query, context, role, config, websocket=None):
     try:
         introduction = await create_chat_completion(
             model=config.smart_llm_model,
             messages=[
                 {"role": "system", "content": f"{role}"},
                 {"role": "user", "content": generate_report_introduction(query, context)}],
@@ -284,28 +287,31 @@
             stream=True,
             websocket=websocket,
             max_tokens=config.smart_token_limit
         )
 
         return introduction
     except Exception as e:
-        print(f"{Fore.RED}Error in generating report introduction: {e}{Style.RESET_ALL}")
+        print(
+            f"{Fore.RED}Error in generating report introduction: {e}{Style.RESET_ALL}")
 
     return ""
 
+
 def extract_headers(markdown_text: str):
     # Function to extract headers from markdown text
 
     headers = []
     parsed_md = markdown.markdown(markdown_text)  # Parse markdown text
     lines = parsed_md.split("\n")  # Split text into lines
 
     stack = []  # Initialize stack to keep track of nested headers
     for line in lines:
-        if line.startswith("<h") and len(line) > 1:  # Check if the line starts with an HTML header tag
+        # Check if the line starts with an HTML header tag
+        if line.startswith("<h") and len(line) > 1:
             level = int(line[2])  # Extract header level
             header_text = line[
                 line.index(">") + 1: line.rindex("<")
             ]  # Extract header text
 
             # Pop headers from the stack with higher or equal level
             while stack and stack[-1]["level"] >= level:
@@ -351,14 +357,15 @@
 
         return toc  # Return the generated table of contents
 
     except Exception as e:
         print("table_of_contents Exception : ", e)  # Print exception if any
         return markdown_text  # Return original markdown text if an exception occurs
 
+
 def add_source_urls(report_markdown: str, visited_urls: set):
     """
     This function takes a Markdown report and a set of visited URLs as input parameters.
 
     Args:
       report_markdown (str): The `add_source_urls` function takes in two parameters:
       visited_urls (set): Visited_urls is a set that contains URLs that have already been visited. This
@@ -372,8 +379,8 @@
 
         updated_markdown_report = report_markdown + url_markdown
 
         return updated_markdown_report
 
     except Exception as e:
         print(f"Encountered exception in adding source urls : {e}")
-        return report_markdown
+        return report_markdown
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/master/prompts.py` & `gpt-researcher-0.5.1/gpt_researcher/master/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime, timezone
 import warnings
-from gpt_researcher.utils.enum import ReportType
-
+from gpt_researcher.utils.enum import ReportType, ReportSource
 
 def generate_search_queries_prompt(question: str, parent_query: str, report_type: str, max_iterations: int=3,):
     """ Generates the search queries prompt for the given question.
     Args: 
         question (str): The question to generate the search queries prompt for
         parent_query (str): The main question (only relevant for detailed reports)
         report_type (str): The report type
@@ -21,87 +20,119 @@
 
     return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{task}"' \
            f'Use the current date if needed: {datetime.now().strftime("%B %d, %Y")}.\n' \
            f'Also include in the queries specified task details such as locations, names, etc.\n' \
            f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].'
 
 
-def generate_report_prompt(question, context, report_format="apa", total_words=1000):
+def generate_report_prompt(question: str, context, report_source: str, report_format="apa", total_words=1000):
     """ Generates the report prompt for the given question and research summary.
     Args: question (str): The question to generate the report prompt for
             research_summary (str): The research summary to generate the report prompt for
     Returns: str: The report prompt for the given question and research summary
     """
+    
+    reference_prompt = ""
+    if report_source == ReportSource.Web.value:
+        reference_prompt = f"""
+            You MUST write all used source urls at the end of the report as references, and make sure to not add duplicated sources, but only one reference for each.
+            Every url should be hyperlinked: [url website](url)
+            Additionally, you MUST include hyperlinks to the relevant URLs wherever they are referenced in the report : 
+        
+            eg:    
+                # Report Header
+                
+                This is a sample text. ([url website](url))
+            """
+    else:
+        reference_prompt = f"""
+            You MUST write all used source document names at the end of the report as references, and make sure to not add duplicated sources, but only one reference for each."
+        """
+        
 
     return f'Information: """{context}"""\n\n' \
            f'Using the above information, answer the following' \
            f' query or task: "{question}" in a detailed report --' \
            " The report should focus on the answer to the query, should be well structured, informative," \
            f" in depth and comprehensive, with facts and numbers if available and a minimum of {total_words} words.\n" \
            "You should strive to write the report as long as you can using all relevant and necessary information provided.\n" \
            "You must write the report with markdown syntax.\n " \
            f"Use an unbiased and journalistic tone. \n" \
            "You MUST determine your own concrete and valid opinion based on the given information. Do NOT deter to general and meaningless conclusions.\n" \
-           f"You MUST write all used source urls at the end of the report as references, and make sure to not add duplicated sources, but only one reference for each.\n" \
-           "Every url should be hyperlinked: [url website](url)"\
-           """
-            Additionally, you MUST include hyperlinks to the relevant URLs wherever they are referenced in the report : 
-        
-            eg:    
-                # Report Header
-                
-                This is a sample text. ([url website](url))
-            """\
+           f"{reference_prompt}"\
             f"You MUST write the report in {report_format} format.\n " \
             f"Cite search results using inline notations. Only cite the most \
             relevant results that answer the query accurately. Place these citations at the end \
             of the sentence or paragraph that reference them.\n"\
             f"Please do your best, this is very important to my career. " \
             f"Assume that the current date is {datetime.now().strftime('%B %d, %Y')}"
 
 
-def generate_resource_report_prompt(question, context, report_format="apa", total_words=700):
+def generate_resource_report_prompt(question, context, report_source: str, report_format="apa", total_words=1000):
     """Generates the resource report prompt for the given question and research summary.
 
     Args:
         question (str): The question to generate the resource report prompt for.
         context (str): The research summary to generate the resource report prompt for.
 
     Returns:
         str: The resource report prompt for the given question and research summary.
     """
+    
+    reference_prompt = ""
+    if report_source == ReportSource.Web.value:
+        reference_prompt = f"""
+            You MUST include all relevant source urls.
+            Every url should be hyperlinked: [url website](url)
+            """
+    else:
+        reference_prompt = f"""
+            You MUST write all used source document names at the end of the report as references, and make sure to not add duplicated sources, but only one reference for each."
+        """
+    
     return f'"""{context}"""\n\nBased on the above information, generate a bibliography recommendation report for the following' \
            f' question or topic: "{question}". The report should provide a detailed analysis of each recommended resource,' \
            ' explaining how each source can contribute to finding answers to the research question.\n' \
            'Focus on the relevance, reliability, and significance of each source.\n' \
            'Ensure that the report is well-structured, informative, in-depth, and follows Markdown syntax.\n' \
            'Include relevant facts, figures, and numbers whenever available.\n' \
            f'The report should have a minimum length of {total_words} words.\n' \
-        'You MUST include all relevant source urls.'\
-        'Every url should be hyperlinked: [url website](url)'
+           'You MUST include all relevant source urls.'\
+           'Every url should be hyperlinked: [url website](url)'\
+           f'{reference_prompt}'
 
-
-def generate_custom_report_prompt(query_prompt, context, report_format="apa", total_words=1000):
+def generate_custom_report_prompt(query_prompt, context, report_source: str, report_format="apa", total_words=1000):
     return f'"{context}"\n\n{query_prompt}'
 
 
-def generate_outline_report_prompt(question, context, report_format="apa", total_words=1200):
+def generate_outline_report_prompt(question, context, report_source: str, report_format="apa", total_words=1000):
     """ Generates the outline report prompt for the given question and research summary.
     Args: question (str): The question to generate the outline report prompt for
             research_summary (str): The research summary to generate the outline report prompt for
     Returns: str: The outline report prompt for the given question and research summary
     """
 
     return f'"""{context}""" Using the above information, generate an outline for a research report in Markdown syntax' \
            f' for the following question or topic: "{question}". The outline should provide a well-structured framework' \
            ' for the research report, including the main sections, subsections, and key points to be covered.' \
            f' The research report should be detailed, informative, in-depth, and a minimum of {total_words} words.' \
            ' Use appropriate Markdown syntax to format the outline and ensure readability.'
 
 
+def get_report_by_type(report_type: str):
+    report_type_mapping = {
+        ReportType.ResearchReport.value: generate_report_prompt,
+        ReportType.ResourceReport.value: generate_resource_report_prompt,
+        ReportType.OutlineReport.value: generate_outline_report_prompt,
+        ReportType.CustomReport.value: generate_custom_report_prompt,
+        ReportType.SubtopicReport.value: generate_subtopic_report_prompt
+    }
+    return report_type_mapping[report_type]
+
+
 def auto_agent_instructions():
     return """
         This task involves researching a given topic, regardless of its complexity or the availability of a definitive answer. The research is conducted by a specific server, defined by its type and role, with each server requiring distinct instructions.
         Agent
         The server is determined by the field of the topic and the specific name of the server that could be utilized to research the topic provided. Agents are categorized by their area of expertise, and each server type is associated with a corresponding emoji.
 
         examples:
@@ -163,20 +194,20 @@
                 
                 {format_instructions}
             """
 
 
 def generate_subtopic_report_prompt(
     current_subtopic,
-    existing_headers,
-    main_topic,
+    existing_headers: list,
+    main_topic: str,
     context,
-    report_format="apa",
-    total_words=800,
+    report_format: str = "apa",
     max_subsections=5,
+    total_words=800
 ) -> str:
 
     return f"""
     "Context":
     "{context}"
     
     "Main Topic and Subtopic":
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.5.1/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SerpApi Retriever
 
 # libraries
 import os
 import requests
-import json
+from duckduckgo_search import DDGS
+import urllib.parse
 
 
 class SerpApiSearch():
     """
     SerpApi Retriever
     """
     def __init__(self, query):
         """
         Initializes the SerpApiSearch object
         Args:
             query:
         """
-        raise NotImplementedError("SerpApiSearch is not fully implemented yet.")
         self.query = query
         self.api_key = self.get_api_key()
 
     def get_api_key(self):
         """
         Gets the SerpApi API key
         Returns:
@@ -35,44 +35,43 @@
 
     def search(self, max_results=7):
         """
         Searches the query
         Returns:
 
         """
-        print("Searching with query {0}...".format(self.query))
+        print("SerpApiSearch: Searching with query {0}...".format(self.query))
         """Useful for general internet search queries using SerpApi."""
 
 
-        # Perform the search
-        # TODO: query needs to be url encoded, so the code won't work as is.
-        # Encoding should look something like this (but this is untested):
-        # url_encoded_query = self.query.replace(" ", "+")
-        url = "https://serpapi.com/search.json?engine=google&q=" + self.query + "&api_key=" + self.api_key
-        resp = requests.request("GET", url)
-
-        # Preprocess the results
-        if resp is None:
-            return
+        url = "https://serpapi.com/search.json"
+        params = {
+            "q": self.query,
+            "api_key": self.api_key
+        }
+        encoded_url = url + "?" + urllib.parse.urlencode(params)
+        search_response = []
         try:
-            search_results = json.loads(resp.text)
-        except Exception:
-            return
-        if search_results is None:
-            return
-
-        results = search_results["organic_results"]
-        search_results = []
-
-        # Normalize the results to match the format of the other search APIs
-        for result in results:
-            # skip youtube results
-            if "youtube.com" in result["link"]:
-                continue
-            search_result = {
-                "title": result["title"],
-                "href": result["link"],
-                "body": result["snippet"],
-            }
-            search_results.append(search_result)
+            response = requests.get(encoded_url, timeout=10)
+            if response.status_code == 200:
+                search_results = response.json()
+                if search_results:
+                    results = search_results["organic_results"]
+                    for result in results:
+                        # skip youtube results
+                        if "youtube.com" in result["link"]:
+                            continue
+                        if results_processed >= max_results:
+                            break
+                        search_result = {
+                            "title": result["title"],
+                            "href": result["link"],
+                            "body": result["snippet"],
+                        }
+                        search_response.append(search_result)
+                        results_processed += 1    
+        except Exception as e: # Fallback in case overload on Tavily Search API
+            print(f"Error: {e}")
+            ddg = DDGS()
+            search_response = ddg.text(self.query, region='wt-wt', max_results=max_results)
 
-        return search_results
+        return search_response
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/serper.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         # Search the query (see https://serper.dev/playground for the format)
         url = "https://google.serper.dev/search"
 
         headers = {
         'X-API-KEY': self.api_key,
         'Content-Type': 'application/json'
         }
-        data = json.dumps({"q": self.query})
+        data = json.dumps({"q": self.query, "num": max_results})
 
-        resp = requests.request("POST", url, headers=headers, data=data)
+        resp = requests.request("POST", url, timeout=10, headers=headers, data=data)
 
         # Preprocess the results
         if resp is None:
             return
         try:
             search_results = json.loads(resp.text)
         except Exception:
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Tavily API Retriever
 
 # libraries
 import os
 from tavily import TavilyClient
+from duckduckgo_search import DDGS
+from yahoo_search import search
 
 
-class TavilyNews():
+class TavilySearch():
     """
-    Tavily News API Retriever
-    Retrieve news articles from the Tavily News API
+    Tavily API Retriever
     """
-    def __init__(self, query):
+    def __init__(self, query, topic="general"):
         """
         Initializes the TavilySearch object
         Args:
             query:
         """
         self.query = query
         self.api_key = self.get_api_key()
         self.client = TavilyClient(self.api_key)
+        self.topic = topic
 
     def get_api_key(self):
         """
         Gets the Tavily API key
         Returns:
 
         """
@@ -36,12 +38,24 @@
 
     def search(self, max_results=7):
         """
         Searches the query
         Returns:
 
         """
-        # Search the query
-        results = self.client.search(self.query, search_depth="advanced", topic="news", max_results=max_results)
-        # Return the results
-        search_response = [{"href": obj["url"], "body": obj["content"]} for obj in results.get("results", [])]
+        try:
+            # Search the query
+            results = self.client.search(self.query, search_depth="basic", max_results=max_results, topic=self.topic)
+            sources = results.get("results", [])
+            if not sources:
+                raise Exception("No results found with Tavily API search.")
+            # Return the results
+            search_response = [{"href": obj["url"], "body": obj["content"]} for obj in sources]
+        except Exception as e: # Fallback in case overload on Tavily Search API
+            print(f"Error: {e}. Fallback to DuckDuckGo Search API...")
+            try:
+                ddg = DDGS()
+                search_response = ddg.text(self.query, region='wt-wt', max_results=max_results)
+            except Exception as e:
+                print(f"Error: {e}. Fallback to Yahoo Search API...")
+                search_response = [{"href": obj.link, "body": obj.text, "title": obj.title} for obj in search(self.query).pages]
         return search_response
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher/utils/llm.py` & `gpt-researcher-0.5.1/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.4.5/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.5.1/gpt_researcher.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.4.5
+Version: 0.5.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔎 GPT Researcher
 [![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
-[![Discord Follow](https://dcbadge.vercel.app/api/server/2pFkc83fRq?style=for-the-badge)](https://discord.gg/MN9M86kb)
+[![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
 -  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
 -  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
@@ -60,30 +61,30 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Tutorials
- - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
+ - [How it Works](https://docs.gptr.dev/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
-- 📝 Generate research, outlines, resources and lessons reports
+- 📝 Generate research, outlines, resources and lessons reports with local documents and web sources
 - 📜 Can generate long and detailed research reports (over 2K words)
 - 🌐 Aggregates over 20 web sources per research to form objective and factual conclusions
 - 🖥️ Includes an easy-to-use web interface (HTML/CSS/JS)
 - 🔍 Scrapes web sources with javascript support
 - 📂 Keeps track and context of visited and used web sources
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
-Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
+Please see [here](https://docs.gptr.dev/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
@@ -125,48 +126,70 @@
 uvicorn main:app --reload
 ```
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
-**To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
+**To learn how to get started with [Docker](https://docs.gptr.dev/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.gptr.dev/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.gptr.dev/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.gptr.dev/docs/gpt-researcher/getting-started) page.**
 
 ### Run as PIP package
 ```bash
 pip install gpt-researcher
 ```
 
 ```python
+...
 from gpt_researcher import GPTResearcher
 
 query = "why is Nvidia stock going up?"
 researcher = GPTResearcher(query=query, report_type="research_report")
 # Conduct research on the given query
 research_result = await researcher.conduct_research()
 # Write the report
 report = await researcher.write_report()
+...
 ```
 
-**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.gptr.dev/docs/gpt-researcher/pip-package) page.**
+
+## 📄 Research on Local Documents
+
+You can instruct the GPT Researcher to run research tasks based on your local documents. Currently supported file formats are: PDF, plain text, CSV, Excel, Markdown, PowerPoint, and Word documents.
+
+Step 1: Add the env variable `DOC_PATH` pointing to the folder where your documents are located.
+
+```bash
+export DOC_PATH="./my-docs"
+```
+
+Step 2: 
+ - If you're running the frontend app on localhost:8000, simply select "My Documents" from the the "Report Source" Dropdown Options.
+ - If you're running GPT Researcher with the [PIP package](https://docs.tavily.com/docs/gpt-researcher/pip-package), pass the `report_source` argument as "documents" when you instantiate the `GPTResearcher` class [code sample here](https://docs.tavily.com/docs/gpt-researcher/tailored-research).
+
+### One-Click Deployment
+
+[![Deploy to RepoCloud](https://d16t0pc4846x52.cloudfront.net/deploylobe.svg)](https://repocloud.io/details/?app_id=274)
 
 ## 👪 Multi-Agent Assistant
 As AI evolves from prompt engineering and RAG to multi-agent systems, we're excited to introduce our new multi-agent assistant built with [LangGraph](https://python.langchain.com/v0.1/docs/langgraph/).
 
 By using LangGraph, the research process can be significantly improved in depth and quality by leveraging multiple agents with specialized skills. Inspired by the recent [STORM](https://arxiv.org/abs/2402.14207) paper, this project showcases how a team of AI agents can work together to conduct research on a given topic, from planning to publication.
 
 An average run generates a 5-6 page research report in multiple formats such as PDF, Docx and Markdown.
 
-Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.tavily.com/docs/gpt-researcher/agent_frameworks) for more information.
+Check it out [here](https://github.com/assafelovic/gpt-researcher/tree/master/multi_agents) or head over to our [documentation](https://docs.gptr.dev/docs/gpt-researcher/agent_frameworks) for more information.
 
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
-
+<a href="https://github.com/assafelovic/gpt-researcher/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=assafelovic/gpt-researcher" />
+</a>
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Author Email: assaf.elovic@gmail.com
 
 ## 🛡 Disclaimer
 
 This project, GPT Researcher, is an experimental application and is provided "as-is" without any warranty, express or implied. We are sharing codes for academic purposes under the MIT license. Nothing herein is academic advice, and NOT a recommendation to use in academic or research papers.
```

### Comparing `gpt-researcher-0.4.5/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.5.1/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 gpt_researcher.egg-info/requires.txt
 gpt_researcher.egg-info/top_level.txt
 gpt_researcher/config/__init__.py
 gpt_researcher/config/config.py
 gpt_researcher/context/__init__.py
 gpt_researcher/context/compression.py
 gpt_researcher/context/retriever.py
+gpt_researcher/document/__init__.py
+gpt_researcher/document/document.py
 gpt_researcher/llm_provider/__init__.py
 gpt_researcher/llm_provider/azureopenai/__init__.py
 gpt_researcher/llm_provider/azureopenai/azureopenai.py
 gpt_researcher/llm_provider/google/__init__.py
 gpt_researcher/llm_provider/google/google.py
 gpt_researcher/llm_provider/openai/__init__.py
 gpt_researcher/llm_provider/openai/openai.py
@@ -44,18 +46,18 @@
 gpt_researcher/retrievers/google/google.py
 gpt_researcher/retrievers/searx/__init__.py
 gpt_researcher/retrievers/searx/searx.py
 gpt_researcher/retrievers/serpapi/__init__.py
 gpt_researcher/retrievers/serpapi/serpapi.py
 gpt_researcher/retrievers/serper/__init__.py
 gpt_researcher/retrievers/serper/serper.py
-gpt_researcher/retrievers/tavily_news/__init__.py
-gpt_researcher/retrievers/tavily_news/tavily_news.py
 gpt_researcher/retrievers/tavily_search/__init__.py
 gpt_researcher/retrievers/tavily_search/tavily_search.py
+gpt_researcher/retrievers/yahoo/__init__.py
+gpt_researcher/retrievers/yahoo/yahoo.py
 gpt_researcher/scraper/__init__.py
 gpt_researcher/scraper/scraper.py
 gpt_researcher/scraper/arxiv/__init__.py
 gpt_researcher/scraper/arxiv/arxiv.py
 gpt_researcher/scraper/beautiful_soup/__init__.py
 gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
 gpt_researcher/scraper/newspaper/__init__.py
```

### Comparing `gpt-researcher-0.4.5/pyproject.toml` & `gpt-researcher-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 version = "0.0.5"
 description = "GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks."
 authors = ["Tavily <support@tavily.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
+python = ">=3.10,<3.12"
 beautifulsoup4 = ">=4.12.2"
 colorama = ">=0.4.6"
 duckduckgo_search = ">=4.1.1"
 md2pdf = ">=1.0.1"
 openai = ">=1.3.3"
 playwright = ">=1.39.0"
 python-dotenv = ">=1.0.0"
@@ -32,14 +32,15 @@
 aiofiles = ">=23.2.1"
 newspaper3k = ">=0.2.8"
 langchain_community = ">=0.0.28"
 SQLAlchemy = ">=2.0.28"
 mistune = "^3.0.2"
 htmldocx = "^0.0.6"
 python-docx = "^1.1.0"
-langchain-openai = "^0.1.0"
+langchain-openai = "^0.1.1"
 langchain-google-genai = "^0.0.11"
 lxml = { version = ">=4.9.2", extras = ["html_clean"] }
+unstructured = "^0.13.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gpt-researcher-0.4.5/setup.py` & `gpt-researcher-0.5.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.4.5",
+    version="0.5.1",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

