# Comparing `tmp/gpt-researcher-0.5.1.tar.gz` & `tmp/gpt-researcher-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.5.1.tar", last modified: Thu May 23 13:07:56 2024, max compression
+gzip compressed data, was "gpt-researcher-0.5.2.tar", last modified: Thu May 23 13:11:20 2024, max compression
```

## Comparing `gpt-researcher-0.5.1.tar` & `gpt-researcher-0.5.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.210263 gpt-researcher-0.5.1/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:07:56.209420 gpt-researcher-0.5.1/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    12159 2024-05-23 11:18:14.000000 gpt-researcher-0.5.1/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.143611 gpt-researcher-0.5.1/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.144427 gpt-researcher-0.5.1/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.146011 gpt-researcher-0.5.1/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.147425 gpt-researcher-0.5.1/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.1/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.148609 gpt-researcher-0.5.1/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.153520 gpt-researcher-0.5.1/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.158984 gpt-researcher-0.5.1/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.1/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.160966 gpt-researcher-0.5.1/gpt_researcher/document/
--rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/document/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/document/document.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.162286 gpt-researcher-0.5.1/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.164500 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.166120 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.167658 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.172222 gpt-researcher-0.5.1/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.1/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.1/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    14872 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.174605 gpt-researcher-0.5.1/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.5.1/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.175727 gpt-researcher-0.5.1/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      500 2024-05-23 13:00:48.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.177210 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.179434 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.181403 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.183486 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.185478 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.187304 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.189154 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2028 2024-05-23 13:06:48.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.190703 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1152 2024-05-23 13:04:41.000000 gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/yahoo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.192795 gpt-researcher-0.5.1/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.194812 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.196899 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.198929 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.200888 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.203013 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.207885 gpt-researcher-0.5.1/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.1/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.1/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:07:56.151890 gpt-researcher-0.5.1/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2781 2024-05-23 13:07:56.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      393 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-23 13:07:55.000000 gpt-researcher-0.5.1/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.1/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-23 13:07:56.210489 gpt-researcher-0.5.1/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-23 13:07:51.000000 gpt-researcher-0.5.1/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.445988 gpt-researcher-0.5.2/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:11:20.445381 gpt-researcher-0.5.2/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    12159 2024-05-23 11:18:14.000000 gpt-researcher-0.5.2/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.389207 gpt-researcher-0.5.2/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.390263 gpt-researcher-0.5.2/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.391657 gpt-researcher-0.5.2/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.393171 gpt-researcher-0.5.2/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.2/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.394304 gpt-researcher-0.5.2/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.2/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.399045 gpt-researcher-0.5.2/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.2/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.402036 gpt-researcher-0.5.2/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.2/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.2/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.2/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.403898 gpt-researcher-0.5.2/gpt_researcher/document/
+-rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/gpt_researcher/document/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/gpt_researcher/document/document.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.404776 gpt-researcher-0.5.2/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.406421 gpt-researcher-0.5.2/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.408014 gpt-researcher-0.5.2/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.409405 gpt-researcher-0.5.2/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.2/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.412606 gpt-researcher-0.5.2/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.2/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.2/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12450 2024-05-23 13:10:15.000000 gpt-researcher-0.5.2/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    14872 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.414427 gpt-researcher-0.5.2/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.2/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.5.2/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.415308 gpt-researcher-0.5.2/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      500 2024-05-23 13:00:48.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.416571 gpt-researcher-0.5.2/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.418247 gpt-researcher-0.5.2/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.419640 gpt-researcher-0.5.2/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.421008 gpt-researcher-0.5.2/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.422408 gpt-researcher-0.5.2/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.423695 gpt-researcher-0.5.2/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.425445 gpt-researcher-0.5.2/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2028 2024-05-23 13:06:48.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.427603 gpt-researcher-0.5.2/gpt_researcher/retrievers/yahoo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/yahoo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1152 2024-05-23 13:04:41.000000 gpt-researcher-0.5.2/gpt_researcher/retrievers/yahoo/yahoo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.430426 gpt-researcher-0.5.2/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.432606 gpt-researcher-0.5.2/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.435054 gpt-researcher-0.5.2/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.437044 gpt-researcher-0.5.2/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.438350 gpt-researcher-0.5.2/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.439804 gpt-researcher-0.5.2/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.443832 gpt-researcher-0.5.2/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.2/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.2/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:11:20.397588 gpt-researcher-0.5.2/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:11:20.000000 gpt-researcher-0.5.2/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2781 2024-05-23 13:11:20.000000 gpt-researcher-0.5.2/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-23 13:11:20.000000 gpt-researcher-0.5.2/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      393 2024-05-23 13:11:20.000000 gpt-researcher-0.5.2/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-23 13:11:20.000000 gpt-researcher-0.5.2/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.2/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-23 13:11:20.446210 gpt-researcher-0.5.2/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-23 13:10:39.000000 gpt-researcher-0.5.2/setup.py
```

### Comparing `gpt-researcher-0.5.1/LICENSE` & `gpt-researcher-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/PKG-INFO` & `gpt-researcher-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.1
+Version: 0.5.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.5.1/README.md` & `gpt-researcher-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.5.2/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.5.2/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/backend/server.py` & `gpt-researcher-0.5.2/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/backend/utils.py` & `gpt-researcher-0.5.2/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/backend/websocket_manager.py` & `gpt-researcher-0.5.2/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/config/config.py` & `gpt-researcher-0.5.2/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/context/compression.py` & `gpt-researcher-0.5.2/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/context/retriever.py` & `gpt-researcher-0.5.2/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/document/document.py` & `gpt-researcher-0.5.2/gpt_researcher/document/document.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.5.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.5.2/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.5.2/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/master/agent.py` & `gpt-researcher-0.5.2/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/master/functions.py` & `gpt-researcher-0.5.2/gpt_researcher/master/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,33 +18,33 @@
         retriever: Retriever class
 
     """
     match retriever:
         case "tavily":
             from gpt_researcher.retrievers import TavilySearch
             retriever = TavilySearch
-        case "tavily_news":
-            from gpt_researcher.retrievers import TavilyNews
-            retriever = TavilyNews
         case "google":
             from gpt_researcher.retrievers import GoogleSearch
             retriever = GoogleSearch
+        case "yahoo":
+            from gpt_researcher.retrievers import YahooSearch
+            retriever = YahooSearch
         case "searx":
             from gpt_researcher.retrievers import SearxSearch
             retriever = SearxSearch
         case "serpapi":
             from gpt_researcher.retrievers import SerpApiSearch
             retriever = SerpApiSearch
         case "googleSerp":
             from gpt_researcher.retrievers import SerperSearch
             retriever = SerperSearch
         case "duckduckgo":
             from gpt_researcher.retrievers import Duckduckgo
             retriever = Duckduckgo
-        case "BingSearch":
+        case "bing":
             from gpt_researcher.retrievers import BingSearch
             retriever = BingSearch
 
         case _:
             raise Exception("Retriever not found.")
 
     return retriever
```

### Comparing `gpt-researcher-0.5.1/gpt_researcher/master/prompts.py` & `gpt-researcher-0.5.2/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.5.2/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/retrievers/yahoo/yahoo.py` & `gpt-researcher-0.5.2/gpt_researcher/retrievers/yahoo/yahoo.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.5.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher/utils/llm.py` & `gpt-researcher-0.5.2/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.5.2/gpt_researcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.1
+Version: 0.5.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.5.1/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.5.2/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/pyproject.toml` & `gpt-researcher-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.1/setup.py` & `gpt-researcher-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.5.1",
+    version="0.5.2",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

