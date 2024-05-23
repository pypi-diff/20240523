# Comparing `tmp/suskabot-0.2.2.tar.gz` & `tmp/suskabot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suskabot-0.2.2.tar", max compression
+gzip compressed data, was "suskabot-0.2.3.tar", max compression
```

## Comparing `suskabot-0.2.2.tar` & `suskabot-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2024-05-08 22:15:32.362063 suskabot-0.2.2/LICENSE
--rw-r--r--   0        0        0     1706 2024-05-08 22:15:32.362063 suskabot-0.2.2/README.md
--rw-r--r--   0        0        0      815 2024-05-08 22:15:32.369063 suskabot-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      510 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/__init__.py
--rw-r--r--   0        0        0      581 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/__main__.py
--rw-r--r--   0        0        0       23 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/app/__init__.py
--rw-r--r--   0        0        0     1529 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/app/app.py
--rw-r--r--   0        0        0      381 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/config/.env.example
--rw-r--r--   0        0        0        4 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/config/.gitignore
--rw-r--r--   0        0        0       26 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/config/__init__.py
--rw-r--r--   0        0        0     4908 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/config/config.py
--rw-r--r--   0        0        0       32 2024-05-08 22:15:32.369063 suskabot-0.2.2/suskabot/controllers/__init__.py
--rw-r--r--   0        0        0       24 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/bot.py
--rw-r--r--   0        0        0       67 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/__init__.py
--rw-r--r--   0        0        0     1331 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/app.py
--rw-r--r--   0        0        0     1776 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/translator.py
--rw-r--r--   0        0        0     6758 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
--rw-r--r--   0        0        0       56 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/services/__init__.py
--rw-r--r--   0        0        0     4151 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/services/translator.py
--rw-r--r--   0        0        0     5924 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/services/youtube_downloader.py
--rw-r--r--   0        0        0       25 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/utils/__init__.py
--rw-r--r--   0        0        0      861 2024-05-08 22:15:32.370063 suskabot-0.2.2/suskabot/utils/utils.py
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 suskabot-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 11:47:00.739677 suskabot-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1817 2024-05-23 11:47:00.739677 suskabot-0.2.3/README.md
+-rw-r--r--   0        0        0      815 2024-05-23 11:47:00.748679 suskabot-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      510 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/__main__.py
+-rw-r--r--   0        0        0       23 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/app/__init__.py
+-rw-r--r--   0        0        0     1529 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/app/app.py
+-rw-r--r--   0        0        0      381 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/.env.example
+-rw-r--r--   0        0        0        4 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/.gitignore
+-rw-r--r--   0        0        0       26 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/__init__.py
+-rw-r--r--   0        0        0     4908 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/config/config.py
+-rw-r--r--   0        0        0       32 2024-05-23 11:47:00.748679 suskabot-0.2.3/suskabot/controllers/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/bot.py
+-rw-r--r--   0        0        0       67 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/__init__.py
+-rw-r--r--   0        0        0     1331 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/app.py
+-rw-r--r--   0        0        0     1776 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/translator.py
+-rw-r--r--   0        0        0     6758 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/youtube_downloader.py
+-rw-r--r--   0        0        0       56 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/__init__.py
+-rw-r--r--   0        0        0     4151 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/translator.py
+-rw-r--r--   0        0        0     5924 2024-05-23 11:47:00.749679 suskabot-0.2.3/suskabot/services/youtube_downloader.py
+-rw-r--r--   0        0        0       25 2024-05-23 11:47:00.750679 suskabot-0.2.3/suskabot/utils/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-23 11:47:00.750679 suskabot-0.2.3/suskabot/utils/utils.py
+-rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 suskabot-0.2.3/PKG-INFO
```

### Comparing `suskabot-0.2.2/LICENSE` & `suskabot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/README.md` & `suskabot-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,19 @@
    To run the tests use:
    ```shell
    poetry run pytest -v -s -n auto
    ```
 
 
 ## Usage
-### Manual 
+### Manual
+0) Get the project:
+   ```shell
+   git clone https://gitlab.com/vinyl_summer/suskabot.git && cd suskabot
+   ```
 1) Create and activate a new virtual environment
    ```shell
    poetry shell
    ```
 2) Install the project requirements
    ```shell
    poetry install
```

### Comparing `suskabot-0.2.2/pyproject.toml` & `suskabot-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 package-mode = true
 name = "suskabot"
-version = "0.2.2"
+version = "0.2.3"
 description = "telegram bot with various functions"
 authors = ["vinyl_summer <vinyl6428@gmail.dotcom>"]
 readme = "README.md"
 license = "LICENSE"
 
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://gitlab.com/api/v4/projects/45324644/packages/pypi/simple"
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 lingua-language-detector = "^2.0.2"
 translators = "^5.9.1"
-pytube = { source = "gitlab", version = "15.0.1" }
+pytube = { source = "gitlab", version = "15.0.2" }
 python-telegram-bot = {extras = ["job-queue"], version = "^21.1.1"}
 pydantic = "^2.7.1"
 python-dotenv = "^1.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4"
 pytest-sugar = "*"
```

### Comparing `suskabot-0.2.2/suskabot/__main__.py` & `suskabot-0.2.3/suskabot/__main__.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/app/app.py` & `suskabot-0.2.3/suskabot/app/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/config/config.py` & `suskabot-0.2.3/suskabot/config/config.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/controllers/telegram_api/bot.py` & `suskabot-0.2.3/suskabot/controllers/telegram_api/bot.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/app.py` & `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/app.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/translator.py` & `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/translator.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/controllers/telegram_api/handlers/youtube_downloader.py` & `suskabot-0.2.3/suskabot/controllers/telegram_api/handlers/youtube_downloader.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/services/translator.py` & `suskabot-0.2.3/suskabot/services/translator.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/services/youtube_downloader.py` & `suskabot-0.2.3/suskabot/services/youtube_downloader.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/suskabot/utils/utils.py` & `suskabot-0.2.3/suskabot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `suskabot-0.2.2/PKG-INFO` & `suskabot-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: suskabot
-Version: 0.2.2
+Version: 0.2.3
 Summary: telegram bot with various functions
 License: LICENSE
 Author: vinyl_summer
 Author-email: vinyl6428@gmail.dotcom
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: lingua-language-detector (>=2.0.2,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-telegram-bot[job-queue] (>=21.1.1,<22.0.0)
-Requires-Dist: pytube (==15.0.1)
+Requires-Dist: pytube (==15.0.2)
 Requires-Dist: translators (>=5.9.1,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Suskabot
 Telegram Bot that really can do it all!
 
 [PyPi package](https://pypi.org/project/suskabot/)
@@ -43,15 +43,19 @@
    To run the tests use:
    ```shell
    poetry run pytest -v -s -n auto
    ```
 
 
 ## Usage
-### Manual 
+### Manual
+0) Get the project:
+   ```shell
+   git clone https://gitlab.com/vinyl_summer/suskabot.git && cd suskabot
+   ```
 1) Create and activate a new virtual environment
    ```shell
    poetry shell
    ```
 2) Install the project requirements
    ```shell
    poetry install
```

