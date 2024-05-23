# Comparing `tmp/FinRobot-0.1.1.tar.gz` & `tmp/finrobot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinRobot-0.1.1.tar", last modified: Wed May 22 13:41:45 2024, max compression
+gzip compressed data, was "finrobot-0.1.2.tar", last modified: Thu May 23 02:50:15 2024, max compression
```

## Comparing `FinRobot-0.1.1.tar` & `finrobot-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,31 @@
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-05-22 13:41:45.155167 FinRobot-0.1.1/
-drwxr-xr-x   0 bruce      (501) staff       (20)        0 2024-05-22 13:41:45.154692 FinRobot-0.1.1/FinRobot.egg-info/
--rw-r--r--   0 bruce      (501) staff       (20)     1400 2024-05-22 13:41:45.000000 FinRobot-0.1.1/FinRobot.egg-info/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)      185 2024-05-22 13:41:45.000000 FinRobot-0.1.1/FinRobot.egg-info/SOURCES.txt
--rw-r--r--   0 bruce      (501) staff       (20)        1 2024-05-22 13:41:45.000000 FinRobot-0.1.1/FinRobot.egg-info/dependency_links.txt
--rw-r--r--   0 bruce      (501) staff       (20)      178 2024-05-22 13:41:45.000000 FinRobot-0.1.1/FinRobot.egg-info/requires.txt
--rw-r--r--   0 bruce      (501) staff       (20)        1 2024-05-22 13:41:45.000000 FinRobot-0.1.1/FinRobot.egg-info/top_level.txt
--rw-r--r--   0 bruce      (501) staff       (20)      588 2024-05-22 13:39:37.000000 FinRobot-0.1.1/LICENSE
--rw-r--r--   0 bruce      (501) staff       (20)     1400 2024-05-22 13:41:45.154960 FinRobot-0.1.1/PKG-INFO
--rw-r--r--   0 bruce      (501) staff       (20)    11563 2024-05-22 13:39:37.000000 FinRobot-0.1.1/README.md
--rw-r--r--   0 bruce      (501) staff       (20)       38 2024-05-22 13:41:45.155216 FinRobot-0.1.1/setup.cfg
--rw-r--r--   0 bruce      (501) staff       (20)     1553 2024-05-22 13:39:37.000000 FinRobot-0.1.1/setup.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 02:50:15.915234 finrobot-0.1.2/
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 02:50:15.914539 finrobot-0.1.2/FinRobot.egg-info/
+-rw-r--r--   0 wangneng   (501) staff       (20)     1400 2024-05-23 02:50:15.000000 finrobot-0.1.2/FinRobot.egg-info/PKG-INFO
+-rw-r--r--   0 wangneng   (501) staff       (20)      683 2024-05-23 02:50:15.000000 finrobot-0.1.2/FinRobot.egg-info/SOURCES.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)        1 2024-05-23 02:50:15.000000 finrobot-0.1.2/FinRobot.egg-info/dependency_links.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)      178 2024-05-23 02:50:15.000000 finrobot-0.1.2/FinRobot.egg-info/requires.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)        9 2024-05-23 02:50:15.000000 finrobot-0.1.2/FinRobot.egg-info/top_level.txt
+-rw-r--r--   0 wangneng   (501) staff       (20)    11380 2024-05-23 02:46:09.000000 finrobot-0.1.2/LICENSE
+-rw-r--r--   0 wangneng   (501) staff       (20)     1400 2024-05-23 02:50:15.915016 finrobot-0.1.2/PKG-INFO
+-rw-r--r--   0 wangneng   (501) staff       (20)    12267 2024-05-23 02:46:09.000000 finrobot-0.1.2/README.md
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 02:50:15.910364 finrobot-0.1.2/finrobot/
+-rw-r--r--   0 wangneng   (501) staff       (20)        0 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/__init__.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 02:50:15.912265 finrobot-0.1.2/finrobot/data_source/
+-rw-r--r--   0 wangneng   (501) staff       (20)      429 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/__init__.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    10136 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/finnhub_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    14297 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/finnlp_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     7867 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/fmp_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3054 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/sec_utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     4364 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/data_source/yfinance_utils.py
+drwxr-xr-x   0 wangneng   (501) staff       (20)        0 2024-05-23 02:50:15.914273 finrobot-0.1.2/finrobot/functional/
+-rw-r--r--   0 wangneng   (501) staff       (20)      251 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/__init__.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    18299 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/analyzer.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     8790 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/charting.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3107 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/coding.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     7357 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/quantitative.py
+-rw-r--r--   0 wangneng   (501) staff       (20)    15099 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/reportlab.py
+-rw-r--r--   0 wangneng   (501) staff       (20)      780 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/functional/text.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     3133 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/toolkits.py
+-rw-r--r--   0 wangneng   (501) staff       (20)     2537 2024-05-23 02:46:09.000000 finrobot-0.1.2/finrobot/utils.py
+-rw-r--r--   0 wangneng   (501) staff       (20)       38 2024-05-23 02:50:15.915273 finrobot-0.1.2/setup.cfg
+-rw-r--r--   0 wangneng   (501) staff       (20)     1553 2024-05-23 02:49:55.000000 finrobot-0.1.2/setup.py
```

### Comparing `FinRobot-0.1.1/FinRobot.egg-info/PKG-INFO` & `finrobot-0.1.2/FinRobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinRobot
-Version: 0.1.1
+Version: 0.1.2
 Summary: FinRobot: An Open-Source AI Agent Platform for Financial Applications using LLMs
 Home-page: https://github.com/AI4Finance-Foundation/FinRobot
 Author: AI4Finance Foundation
 Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Financial Large Language Models,AI Agents
 Platform: any
```

### Comparing `FinRobot-0.1.1/PKG-INFO` & `finrobot-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinRobot
-Version: 0.1.1
+Version: 0.1.2
 Summary: FinRobot: An Open-Source AI Agent Platform for Financial Applications using LLMs
 Home-page: https://github.com/AI4Finance-Foundation/FinRobot
 Author: AI4Finance Foundation
 Author-email: contact@ai4finance.org
 License: MIT
 Keywords: Financial Large Language Models,AI Agents
 Platform: any
```

### Comparing `FinRobot-0.1.1/README.md` & `finrobot-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -91,27 +91,41 @@
 ├── OAI_CONFIG_LIST_sample
 ├── config_api_keys_sample
 ├── requirements.txt
 └── README.md
 ```
 
 ## Installation:
+1. download the FinRobot repo use terminal or download it manually 
 ```shell
 git clone https://github.com/AI4Finance-Foundation/FinRobot.git
 ```
-
+2. install dependencies
 cd into this repository
 ```bash
 cd FinRobot
+pip install -e ..
 ```
-
-Dependencies
+3. modify OAI_CONFIG_LIST_sample file
+```shell
+1) rename OAI_CONFIG_LIST_sample to OAI_CONFIG_LIST
+2) remove the four lines of comment within the OAI_CONFIG_LIST file
+3) add your own openai api-key <your OpenAI API key here>
+```
+4. modify config_api_keys_sample file
 ```shell
-pip install -r requirements.txt
+1) rename config_api_keys_sample to config_api_keys
+2) remove the comment within the config_api_keys file
+3) add your own finnhub-api "YOUR_FINNHUB_API_KEY"
+4) add your own financialmodelingprep and sec-api keys "YOUR_FMP_API_KEY" and "YOUR_SEC_API_KEY" (for financial report generation)
 ```
+5. Run tutorials, use jupyter notebook navigate to the tutorials folder
+```shell
+```
+
 
 ## AI Agent Papers
 
 + [Stanford University + Microsoft Research] [Agent AI: Surveying the Horizons of Multimodal Interaction](https://arxiv.org/abs/2401.03568)
 + [Stanford University] [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442)
 + [Fudan NLP Group] [The Rise and Potential of Large Language Model Based Agents: A Survey](https://arxiv.org/abs/2309.07864)
 + [Fudan NLP Group] [LLM-Agent-Paper-List](https://github.com/WooooDyy/LLM-Agent-Paper-List)
```

### Comparing `FinRobot-0.1.1/setup.py` & `finrobot-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         REQUIRES = [line.split("#", 1)[0].strip() for line in f if line.strip()]
 except:
     print("'requirements.txt' not found!")
     REQUIRES = list()
 
 setup(
     name="FinRobot",
-    version="0.1.1",
+    version="0.1.2",
     include_package_data=True,
     author="AI4Finance Foundation",
     author_email="contact@ai4finance.org",
     url="https://github.com/AI4Finance-Foundation/FinRobot",
     license="MIT",
     packages=find_packages(),
     install_requires=REQUIRES,
```

