# Comparing `tmp/mmdiary-0.2.0.tar.gz` & `tmp/mmdiary-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmdiary-0.2.0.tar", last modified: Wed May  8 00:21:14 2024, max compression
+gzip compressed data, was "mmdiary-0.3.0.tar", last modified: Thu May 23 00:03:56 2024, max compression
```

## Comparing `mmdiary-0.2.0.tar` & `mmdiary-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-01 19:37:11.000000 mmdiary-0.2.0/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-08 00:21:14.010244 mmdiary-0.2.0/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1569 2024-05-01 19:37:11.000000 mmdiary-0.2.0/README.md
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2228 2024-05-08 00:11:48.000000 mmdiary-0.2.0/pyproject.toml
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-08 00:21:14.010244 mmdiary-0.2.0/setup.cfg
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:11.000000 mmdiary-0.2.0/src/mmdiary/__init__.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/notion/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:17.000000 mmdiary-0.2.0/src/mmdiary/notion/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3351 2024-05-07 10:50:37.000000 mmdiary-0.2.0/src/mmdiary/notion/cache.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2158 2024-05-01 15:24:12.000000 mmdiary-0.2.0/src/mmdiary/notion/cleanup.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15600 2024-05-07 15:35:35.000000 mmdiary-0.2.0/src/mmdiary/notion/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary/telegrambot/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:27.000000 mmdiary-0.2.0/src/mmdiary/telegrambot/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7869 2024-05-01 16:58:22.000000 mmdiary-0.2.0/src/mmdiary/telegrambot/telegrambot_service.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/transcriber/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:32.000000 mmdiary-0.2.0/src/mmdiary/transcriber/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1011 2024-05-07 14:37:03.000000 mmdiary-0.2.0/src/mmdiary/transcriber/searcher.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4112 2024-05-07 21:37:56.000000 mmdiary-0.2.0/src/mmdiary/transcriber/transcriber.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    10555 2024-05-08 00:00:16.000000 mmdiary-0.2.0/src/mmdiary/transcriber/verifier.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/utils/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 15:08:11.000000 mmdiary-0.2.0/src/mmdiary/utils/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7050 2024-05-06 23:38:25.000000 mmdiary-0.2.0/src/mmdiary/utils/datelib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1947 2024-05-07 22:50:14.000000 mmdiary-0.2.0/src/mmdiary/utils/jsoncache.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-01 14:41:54.000000 mmdiary-0.2.0/src/mmdiary/utils/log.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5358 2024-05-07 15:40:56.000000 mmdiary-0.2.0/src/mmdiary/utils/medialib.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-01 17:19:04.000000 mmdiary-0.2.0/src/mmdiary/utils/progressbar.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.010244 mmdiary-0.2.0/src/mmdiary/video/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-01 14:53:43.000000 mmdiary-0.2.0/src/mmdiary/video/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4665 2024-05-08 00:01:19.000000 mmdiary-0.2.0/src/mmdiary/video/processor.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8415 2024-05-07 23:11:01.000000 mmdiary-0.2.0/src/mmdiary/video/uploader.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-08 00:21:14.006244 mmdiary-0.2.0/src/mmdiary.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    43431 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      887 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/SOURCES.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/dependency_links.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      583 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/entry_points.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      152 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/requires.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-05-08 00:21:13.000000 mmdiary-0.2.0/src/mmdiary.egg-info/top_level.txt
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.890636 mmdiary-0.3.0/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    35149 2024-05-14 21:19:42.000000 mmdiary-0.3.0/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    53035 2024-05-23 00:03:56.890636 mmdiary-0.3.0/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)    11174 2024-05-22 23:57:28.000000 mmdiary-0.3.0/README.md
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     2227 2024-05-22 23:59:01.000000 mmdiary-0.3.0/pyproject.toml
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-23 00:03:56.890636 mmdiary-0.3.0/setup.cfg
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/mmdiary/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/__init__.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.850636 mmdiary-0.3.0/src/mmdiary/notion/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3375 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/cache.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2174 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/notion/cleanup.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15750 2024-05-15 23:08:07.000000 mmdiary-0.3.0/src/mmdiary/notion/uploader.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.850636 mmdiary-0.3.0/src/mmdiary/telegrambot/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/telegrambot/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7859 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/telegrambot/telegrambot_service.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.854636 mmdiary-0.3.0/src/mmdiary/transcriber/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1011 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/searcher.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4112 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/transcriber/transcriber.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    11389 2024-05-18 00:04:37.000000 mmdiary-0.3.0/src/mmdiary/transcriber/verifier.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.870636 mmdiary-0.3.0/src/mmdiary/utils/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     8643 2024-05-22 23:57:34.000000 mmdiary-0.3.0/src/mmdiary/utils/datelib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1947 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/jsoncache.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1004 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/log.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5364 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/medialib.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      368 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/utils/progressbar.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.890636 mmdiary-0.3.0/src/mmdiary/video/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-14 21:19:42.000000 mmdiary-0.3.0/src/mmdiary/video/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     6134 2024-05-21 21:53:19.000000 mmdiary-0.3.0/src/mmdiary/video/processor.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    12810 2024-05-22 17:08:37.000000 mmdiary-0.3.0/src/mmdiary/video/uploader.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-23 00:03:56.826635 mmdiary-0.3.0/src/mmdiary.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    53035 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      887 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      583 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/entry_points.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      152 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/requires.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)        8 2024-05-23 00:03:56.000000 mmdiary-0.3.0/src/mmdiary.egg-info/top_level.txt
```

### Comparing `mmdiary-0.2.0/LICENSE` & `mmdiary-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/PKG-INFO` & `mmdiary-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -680,15 +680,15 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/sashacmc/mmdiary
 Project-URL: Bug Reports, https://github.com/sashacmc/mmdiary/issues
 Project-URL: Source, https://github.com/sashacmc/mmdiary/
 Project-URL: Changelog, https://github.com/sashacmc/mmdiary/blob/master/CHANGELOG.md
 Keywords: audio,video,multimedia,tool,youtube,notion,transcriber,uploader
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -715,31 +715,272 @@
 
 You can install MultiMedia Diary Tools via pip:
 
 ```bash
 pip install mmdiary
 ```
 
-## Command line tool usage
+## Environment Setup
+
+Ensure you set the necessary environment variables:
+
+- `MMDIARY_AUDIO_LIB_ROOT`: Root directory for audio notes.
+- `MMDIARY_VIDEO_LIB_ROOTS`: Root directories for video notes (multiple roots can be specified, separated by semicolon).
+- `MMDIARY_VIDEO_WORK_DIR`: Work dir for video processing (can be HUGE)
+- `MMDIARY_VIDEO_RES_DIR`: Results dir for video diary files
+- `MMDIARY_NOTION_API_KEY`: Your Notion API Key (see below).
+- `MMDIARY_NOTION_TOKEN`: Your Notion Auth Token v2 (see below).
+- `MMDIARY_NOTION_CACHE`: Notion uploader cache file
+- `MMDIARY_CACHE`: JSON processing cache file (to avoid reading all transribed files each run)
+- `MMDIARY_YOUTUBE_CLIENT_SECRETS`: Path to `client_secrets.json` (see below)
+- `MMDIARY_YOUTUBE_TOKEN`: Path to `token.json` (see below)
+- `MMDIARY_NOTION_AUDIO_DB_ID`: Notion Audio DB ID (see below)
+- `MMDIARY_NOTION_VIDEO_DB_ID`: Notion Video DB ID (see below) 
+
+
+Example:
+
+```bash
+export MMDIARY_AUDIO_LIB_ROOT="/path/to/audio/library"
+export MMDIARY_VIDEO_LIB_ROOTS="/path/to/video/library1:/path/to/video/library2"
+export MMDIARY_VIDEO_WORK_DIR=/"path/to/work/dir"
+export MMDIARY_VIDEO_RES_DIR="/path/to/wideo/result/dir"
+export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
+export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
+export MMDIARY_NOTION_CACHE="~/.mmdiary/notion_cache.pickle"
+export MMDIARY_CACHE="~/.mmdiary/json_cache.pickle"
+export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
+export MMDIARY_YOUTUBE_TOKEN="~/.mmdiary/token.json"
+export MMDIARY_NOTION_AUDIO_DB_ID="7da1480baa9f565198d3fa54c49b1b23"
+export MMDIARY_NOTION_VIDEO_DB_ID="25225aac51ea5cf0bcc74f8c225fbb63"
+```
+
+## Recommended Tools
+
+To ensure unique filenames for your files, it is recommended to use the [photo-importer](https://github.com/sashacmc/photo-importer) tool.
+
+## Notion Setup
+
+To integrate Multimedia Diary Tools with Notion, you'll need to set up both an API Key and an Auth Token v2. This dual setup is necessary because the API Key allows for fast and efficient operations via the official API, while the Auth Token v2 enables functionalities not available through the official API, such as file uploads and locking pages for editing.
+
+### Obtaining and Setting Up the Notion API Key
+
+1. **Create an Integration in Notion**:
+   - Go to [Notion Integrations](https://www.notion.so/my-integrations) and click on "New Integration".
+   - Follow the instructions to create a new integration and obtain your API Key.
+
+2. **Set the Environment Variable**:
+   - Save the API Key in an environment variable named `MMDIARY_NOTION_API_KEY`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
+     ```
+
+### Obtaining and Setting Up the Notion Auth Token v2
+
+1. **Extract the Auth Token v2 from Your Browser**:
+   - Open Notion in your web browser and log in.
+   - Open the developer tools (usually by pressing `F12` or right-clicking on the page and selecting "Inspect").
+   - Go to the "Application" tab and find the `token_v2` under Cookies for `notion.so`.
+   - Copy the value of the `token_v2`.
+
+2. **Set the Environment Variable**:
+   - Save the Auth Token v2 in an environment variable named `MMDIARY_NOTION_TOKEN`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
+     ```
+
+### Initializing Notion Databases
+
+Before you can upload audio (with text) and links to videos (with text) to Notion, you need to create the necessary databases. Follow these steps:
+
+1. **Run the Initialization Script**:
+   - Use the `mmdiary-notion-upload` utility with the `--init` option to create the required databases on a specified Notion page.
+   - Command:
+     ```bash
+     mmdiary-notion-upload --init ROOT_PAGE_ID
+     ```
+   - Make sure the integration has access to this page.
+
+2. **Set the Database IDs as Environment Variables**:
+   - After running the script, two databases will be created on the specified page. Retrieve their IDs and save them in environment variables.
+   - Example:
+     ```bash
+     export MMDIARY_NOTION_AUDIO_DB_ID='7da1480baa9f565198d3fa54c49b1b23'
+     export MMDIARY_NOTION_VIDEO_DB_ID='25225aac51ea5cf0bcc74f8c225fbb63'
+     ```
+
+3. **Move the Databases if Needed**:
+   - You can move the databases to other pages or to the root of your workspace. If you do this, ensure the integration still has access to them.
+
+## YouTube Setup
+
+### Obtaining and Setting Up the YouTube API Client Secrets
+
+1. **Create a Project in Google Developers Console**:
+   - Go to the [Google Developers Console](https://console.developers.google.com/).
+   - Create a new project or select an existing project.
+   - Enable the YouTube Data API v3 for the project.
+
+2. **Obtain the Client Secrets File**:
+   - Go to the Credentials section in your project.
+   - Click on "Create Credentials" and select "OAuth 2.0 Client IDs".
+   - Follow the instructions to create an OAuth 2.0 Client ID.
+   - Download the `client_secrets.json` file and save it and provide a path in an environment variable named `MMDIARY_YOUTUBE_CLIENT_SECRETS`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
+     ```
+### Setting the Upload Limit
+
+By default, the maximum number of videos that can be uploaded via the YouTube API is 4 per day. To request an extension:
+
+1. **Go to the YouTube API Quota Request Form**:
+   - Visit the [YouTube API Quota Request Form](https://support.google.com/youtube/contact/yt_api_form).
+
+2. **Submit the Request**:
+   - Fill out the form with the necessary details about your project and the reasons for needing a higher quota.
+   - Submit the form and wait for approval from the YouTube API team.
+
+### Authenticating with YouTube API
+
+On the first run of `mmdiary-video-upload`, a URL will be provided. Follow these steps:
+
+1. **Open the URL**:
+   - Copy the provided URL and paste it into your web browser.
+   - Select the Google account authorized for your `client_secrets.json`.
+
+2. **Enter the Authentication Code**:
+   - Copy the authentication code provided after logging in.
+   - Paste the authentication code into the prompt in your terminal.
+   - This code will be saved in file specified by `MMDIARY_YOUTUBE_TOKEN` environment variable, and you won't need to repeat this process for future uploads.
+     
+## Step-By-Step Process Overview
+
+### Audio Diary
+
+#### Speech Recognition
+
+Use the `mmdiary-transcriber-run` utility to perform speech-to-text transcription on audio files.
+
+Command:
+
+```bash
+mmdiary-transcriber-run /path/to/audio/files
+```
+
+#### Upload to Notion
+
+Use the `mmdiary-notion-upload` utility to upload the transcribed text and audio files to Notion.
+
+Command:
+```bash
+mmdiary-notion-upload /path/to/audio/files
+```
+
+### Video Diary
+
+#### Speech Recognition
+
+Use the `mmdiary-transcriber-run` utility to perform speech-to-text transcription on video files.
+
+Command:
+
+```bash
+mmdiary-transcriber-run /path/to/video/files
+```
+
+#### Daily Video Concatenation
+
+Use the `mmdiary-video-concat` utility to merge video files into a single daily video.
+
+Command:
+```bash
+mmdiary-video-concat [dates ...]
+```
+
+#### Upload to YouTube
+
+Use the `mmdiary-video-upload` utility to upload the concatenated video to YouTube.
+
+Command:
+```bash
+mmdiary-video-upload [dates ...]
+```
+
+#### Upload to Notion
+
+Use the `mmdiary-notion-upload` utility to upload the transcribed text with YouTube links to Notion.
+
+Command:
+```bash
+mmdiary-notion-upload "$MMDIARY_VIDEO_RES_DIR"
+```
+
+## Auxiliary Tools
+
+### mmdiary-transcriber-search
+
+The `mmdiary-transcriber-search` utility allows you to search through transcribed texts for specific strings. This can be useful for quickly finding occurrences of certain keywords or phrases within your audio or video transcriptions.
+
+#### Usage
 
-### Transcribe files
 ```bash
-mmdiary-transcriber-run /path/to/folder/with/media/files
+mmdiary-transcriber-search /path/to/transcribed/files "search string"
 ```
-### Upload to notion
+
+### mmdiary-transcriber-verify
+
+The `mmdiary-transcriber-verify` utility checks the generated text from the speech-to-text transcriptions and filters out any garbage data. By default, this verification is performed automatically. Manual invocation of this tool is only necessary if the code has been modified (either manually or after updating the version) to avoid re-running the entire lengthy speech recognition process from scratch.
+
+#### Usage
+
+Simply run the utility specifying the paths to the directories or files you wish to verify in interactive mode
+
 ```bash
-mmdiary-notion-upload /path/to/folder/with/media/files
+mmdiary-transcriber-verify /path/to/transcribed/files
 ```
-### Concat video files
+
+Or run the utility with flag `-d` to check all and after with flag `-f` to apply all
+
 ```bash
-mmdiary-video-concat
+mmdiary-transcriber-verify /path/to/transcribed/files -d
+[check output]
+mmdiary-transcriber-verify /path/to/transcribed/files -f
 ```
-### Upload to notion
+
+### mmdiary-utils-datelib
+
+The `mmdiary-utils-datelib` utility provides various functions for managing and querying your multimedia video diary files by date. It includes options to list dates, list files, disable videos, list disabled videos, and set videos for re-upload.
+
+#### Usage
+
+Possible actions:
+
+- `list_dates`: Print all dates with status.
+- `list_files`: Print all files for a date.
+- `disable_video`: Set a flag for a video file to disable concatenating and uploading, also mark the corresponding date as not processed for future regeneration.
+- `list_disabled_videos`: List videos marked as disabled.
+- `set_reupload`: Mark a video as not uploaded for future re-upload (e.g., if the video was deleted on YouTube).
+
+Example:
+
 ```bash
-mmdiary-video-upload
+# list all dates with status "converted"
+mmdiary-utils-datelib -a list_dates -s converted
+
+# list files for date 2010-09-13
+mmdiary-utils-datelib -a list_files --date 2010-09-13
+
+# disable video
+mmdiary-utils-datelib -a disable_video -f 2010-04-14_17-09-50
+
+# set date 2024-03-15 to reupload
+mmdiary-utils-datelib -a set_reupload -e 2024-03-15
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.
 
 ## Show your support
```

### Comparing `mmdiary-0.2.0/pyproject.toml` & `mmdiary-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mmdiary"
-version = "0.2.0"
+version = "0.3.0"
 description = "Multimedia Diary Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["audio", "video", "multimedia", "tool", "youtube", "notion", "transcriber", "uploader"]
 
 authors = [
@@ -19,15 +19,15 @@
 	{ name = "Alexander Bushnev", email = "Alexander@Bushnev.pro" }
 ]
 
 classifiers = [
 	#   3 - Alpha
   	#   4 - Beta
   	#   5 - Production/Stable
-  	"Development Status :: 3 - Alpha",
+  	"Development Status :: 4 - Beta",
 
 	"Operating System :: POSIX :: Linux",
 	"Operating System :: MacOS",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.6",
 	"Programming Language :: Python :: 3.7",
```

### Comparing `mmdiary-0.2.0/src/mmdiary/notion/cache.py` & `mmdiary-0.3.0/src/mmdiary/notion/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,14 @@
     if args.action == 'list':
         for f in db.list_existing_pages():
             print(f)
     elif args.action == 'remove':
         db.remove_from_existing_pages(args.file)
     elif args.action == 'sync':
         db.sync_existing_pages(
-            Client(auth=os.getenv("NOTION_API_KEY")),
-            (os.getenv("NOTION_AUDIO_DB_ID"), os.getenv("NOTION_VIDEO_DB_ID")),
+            Client(auth=os.getenv("MMDIARY_NOTION_API_KEY")),
+            (os.getenv("MMDIARY_NOTION_AUDIO_DB_ID"), os.getenv("MMDIARY_NOTION_VIDEO_DB_ID")),
         )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mmdiary-0.2.0/src/mmdiary/notion/cleanup.py` & `mmdiary-0.3.0/src/mmdiary/notion/cleanup.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,17 @@
             logging.error("Error deleting block batch: %s, Batch: %s", err, bid)
     logging.info("Successfully cleared %i trash blocks.", cnt)
 
 
 def main():
     log.init_logger()
     try:
-        token = os.getenv("NOTION_TOKEN")
+        token = os.getenv("MMDIARY_NOTION_TOKEN")
         if not token:
-            logging.error("No auth token provided. Please set NOTION_TOKEN env variable.")
+            logging.error("No auth token provided. Please set MMDIARY_NOTION_TOKEN env variable.")
             return 1
 
         client = NotionClient(token_v2=token)
 
         block_ids = get_trash(client)
         if block_ids:
             delete_block(client, block_ids)
```

### Comparing `mmdiary-0.2.0/src/mmdiary/notion/uploader.py` & `mmdiary-0.3.0/src/mmdiary/notion/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 from mmdiary.notion import cache
 from mmdiary.video.uploader import seconds_to_time
 
 
 DESCRIPTION = """
 Uploads transcribed file(s) to the notion database.
 Please declare enviromnent variables before use:
-    NOTION_TOKEN - Notion web auth token, please obtain the `token_v2` value by inspectingn
+    MMDIARY_NOTION_TOKEN - Notion web auth token, please obtain the `token_v2` value by inspectingn
         your browser cookies on a logged-in (non-guest) session on Notion.so
-    NOTION_API_KEY - Notion API key, please create notion integration and provide an API key
+    MMDIARY_NOTION_API_KEY - Notion API key, please create notion integration and provide an API key
         see details there: https://www.notion.so/my-integrations
         (don't forget to share your page/workspace with the integration you created)
-    NOTION_AUDIO_DB_ID - Notion Database ID for Audio Notes (can be created by --init command)
-    NOTION_VIDEO_DB_ID - Notion Database ID for Video Diary (can be created by --init command)
+    MMDIARY_NOTION_AUDIO_DB_ID - Notion Database ID for Audio Notes (can be created by --init command)
+    MMDIARY_NOTION_VIDEO_DB_ID - Notion Database ID for Video Diary (can be created by --init command)
     MMDIARY_NOTION_CACHE_FILE - Cache file
 """
 
 
 MAX_TEXT_SIZE = 2000
 MAX_BLOCKS_BATCH_SIZE = 100
 
@@ -417,51 +417,54 @@
 
 
 def main():
     args = __args_parse()
 
     log.init_logger(args.logfile, level=logging.DEBUG)
 
-    token = os.getenv("NOTION_TOKEN")
+    token = os.getenv("MMDIARY_NOTION_TOKEN")
     if not token:
-        print("NOTION_TOKEN was not set")
+        print("MMDIARY_NOTION_TOKEN was not set")
         sys.exit(1)
 
-    api_key = os.getenv("NOTION_API_KEY")
+    api_key = os.getenv("MMDIARY_NOTION_API_KEY")
     if not api_key:
-        print("NOTION_API_KEY was not set")
+        print("MMDIARY_NOTION_API_KEY was not set")
         sys.exit(1)
 
-    audio_db_id = os.getenv("NOTION_AUDIO_DB_ID")
-    video_db_id = os.getenv("NOTION_VIDEO_DB_ID")
+    audio_db_id = os.getenv("MMDIARY_NOTION_AUDIO_DB_ID")
+    video_db_id = os.getenv("MMDIARY_NOTION_VIDEO_DB_ID")
 
     nup = NotionUploader(
         token=token,
         api_key=api_key,
         audio_db_id=audio_db_id,
         video_db_id=video_db_id,
         force_update=args.force,
         dry_run=args.dryrun,
     )
 
     if args.init:
         audio_db_id, video_db_id = nup.init_databases(args.init)
         print("Databases inited")
         print("Plase set ids to your enviromnent:")
-        print(f"export NOTION_AUDIO_DB_ID='{audio_db_id}'")
-        print(f"export NOTION_VIDEO_DB_ID='{video_db_id}'")
+        print(f"export MMDIARY_NOTION_AUDIO_DB_ID='{audio_db_id}'")
+        print(f"export MMDIARY_NOTION_VIDEO_DB_ID='{video_db_id}'")
         print("(don't forget to share created DBs with the your integration)")
         return
 
     if not api_key:
-        print("NOTION_CACHE_DB_FILE was not set")
+        print("MMDIARY_NOTION_CACHE was not set")
         sys.exit(1)
 
     if not audio_db_id or not video_db_id:
-        print("NOTION_AUDIO_DB_ID or NOTION_VIDEO_DB_ID was not set, please use '--init'")
+        print(
+            "MMDIARY_NOTION_AUDIO_DB_ID or MMDIARY_NOTION_VIDEO_DB_ID was not set,",
+            "please use '--init'",
+        )
         sys.exit(1)
 
     if args.inpath is None:
         print("Input path not provided")
         sys.exit(1)
 
     fileslist = []
```

### Comparing `mmdiary-0.2.0/src/mmdiary/telegrambot/telegrambot_service.py` & `mmdiary-0.3.0/src/mmdiary/telegrambot/telegrambot_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     filters,
 )
 
 from mmdiary.utils import log, medialib
 
 MAX_MESSAGE_SIZE = 1024
 
-g_audiofiles = medialib.MediaLib(os.getenv("AUDIO_NOTES_ROOT")).get_processed()
+g_audiofiles = medialib.MediaLib(os.getenv("MMDIARY_AUDIO_LIB_ROOT")).get_processed()
 
 
 class DateSelector:
     EXIT = 0
     YEAR = 1
     MONTH = 2
     DAY = 3
@@ -213,37 +213,37 @@
 def main() -> None:
     log.init_logger(None, level=logging.DEBUG)
 
     logging.getLogger("httpcore").setLevel(logging.WARNING)
     logging.getLogger("httpx").setLevel(logging.WARNING)
     logging.getLogger("telegram").setLevel(logging.WARNING)
 
-    token = os.getenv("AUDIO_NOTES_TELEGRAM_BOT_TOKEN")
+    token = os.getenv("MMDIARY_TELEGRAM_BOT_TOKEN")
 
     job_queue = JobQueue()
     job_queue.run_daily(
         job_random,
-        datetime.strptime(os.getenv("AUDIO_NOTES_TELEGRAM_AUTO_SEND_TIME"), '%H:%M:%S').time(),
+        datetime.strptime(os.getenv("MMDIARY_TELEGRAM_AUTO_SEND_TIME"), '%H:%M:%S').time(),
     )
     # job_queue.run_repeating(job_random, 60)
 
     application = Application.builder().token(token).job_queue(job_queue).build()
 
     application.auth_users = list(
         map(
             lambda u: u.lower(),
-            os.getenv("AUDIO_NOTES_TELEGRAM_USERS").split(","),
+            os.getenv("MMDIARY_TELEGRAM_USERS").split(","),
         )
     )
     application.auto_send_chats = list(
         map(
             int,
             filter(
                 lambda v: v != '',
-                os.getenv("AUDIO_NOTES_TELEGRAM_AUTO_SEND_CHATS").split(","),
+                os.getenv("MMDIARY_TELEGRAM_AUTO_SEND_CHATS").split(","),
             ),
         )
     )
     application.add_handler(CommandHandler("start", command_start))
     application.add_handler(CommandHandler("random", command_random))
     application.add_handler(CommandHandler("get", command_get))
     application.add_handler(CallbackQueryHandler(command_get))
```

### Comparing `mmdiary-0.2.0/src/mmdiary/transcriber/searcher.py` & `mmdiary-0.3.0/src/mmdiary/transcriber/searcher.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/src/mmdiary/transcriber/transcriber.py` & `mmdiary-0.3.0/src/mmdiary/transcriber/transcriber.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/src/mmdiary/transcriber/verifier.py` & `mmdiary-0.3.0/src/mmdiary/transcriber/verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,40 +21,44 @@
     notion - check notion cache and remove missed local files 
     all - include `local` and `notion`
 
 Optional environment variables:
     MMDIARY_TRANSCRIBE_LANGUAGE - Transcribe language (default: "ru")
 
 Sync check require following environment variables:
-    NOTION_TOKEN - Notion web auth token
+    MMDIARY_NOTION_TOKEN - Notion web auth token
     MMDIARY_NOTION_CACHE_FILE - Cache file
 """
 
 HALLUCINATION_TEXTS = {
     "ru": [
-        re.compile("Игорь Негода"),
-        re.compile("Валерий Курас"),
-        re.compile("Фондю любит тебя"),
-        re.compile("ФактФронт"),
-        re.compile("не пропустить новые видео"),
-        re.compile("[Пп]родолжение в следующей части"),
-        re.compile("[Рр]е(д)?актор субтитров"),
-        re.compile("Субтитры субтитров"),
-        re.compile("Спасибо за субтитры"),
-        re.compile("[Сс]убтитры (подготов|делал|сделаны)"),
-        re.compile("[Бб]лагодарю( (тебя|вас|всех))? за (внимание|просмотр)"),
-        re.compile("[Сс]пасибо( (тебе|вам|всем))? за (внимание|просмотр)"),
-        re.compile("[Пп](одписаться|одписывайся|одписывайтесь) на( (мой|наш|этот))? канал"),
-        re.compile("[Пп](одпишись|одпишитесь|одпишите) на( (мой|наш|этот))? канал"),
-        re.compile("[Дд]обро пожаловать (на|в)( (мой|наш|этот))? канал"),
-        re.compile("[Сс]тавь(те)? лайк(и)?"),
-        re.compile("[Жж]ми(те)? лайк(и)?"),
-        re.compile("[Пп]остав(ь|те|ить) лайк(и)?"),
-        re.compile("[Дд](л)?ай(те)? лайк(и)?"),
-        re.compile("Найдите лайки"),
+        re.compile(r"Игорь Негода"),
+        re.compile(r"Валерий Курас"),
+        re.compile(r"Валерий Савинский"),
+        re.compile(r"Фондю любит тебя"),
+        re.compile(r"ФактФронт"),
+        re.compile(r"не пропустить новые видео"),
+        re.compile(r"Корректор (А|В|Е)\."),
+        re.compile(r"[Пп]родолжение в следующей части"),
+        re.compile(r"[Рр]е(д)?актор субтитров"),
+        re.compile(r"Субтитры субтитров"),
+        re.compile(r"Корректор субтитров"),
+        re.compile(r"Спасибо за субтитры"),
+        re.compile(r"[Сс]убтитры (подготов|делал|сделаны)"),
+        re.compile(r"[Бб]лагодарю( (тебя|вас|всех))? за (внимание|просмотр)"),
+        re.compile(r"[Сс]пасибо( (тебе|вам|всем))? за (внимание|просмотр)"),
+        re.compile(r"[Пп](одписаться|одписывайся|одписывайтесь) на( (мой|наш|этот))? канал"),
+        re.compile(r"[Пп](одпишись|одпишитесь|одпишите) на( (мой|наш|этот))? канал"),
+        re.compile(r"[Дд]обро пожаловать (на|в)( (мой|наш|этот))? канал"),
+        re.compile(r"[Сс]тавь(те)? лайк(и)?"),
+        re.compile(r"[Жж]ми(те)? лайк(и)?"),
+        re.compile(r"[Пп]остав(ь|те|ить) лайк(и)?"),
+        re.compile(r"[Дд](л)?ай(те)? лайк(и)?"),
+        re.compile(r"Найдите лайки"),
+        re.compile(r"Я не могу это сделать"),
         # exclude all capitalised except some key words
         re.compile(r"^(?!.*(?:МУЗЫКА|СМЕХ|КАШЕЛЬ|ПЕСНЯ|ПОЮТ|ПОЕТ|КРИК))[А-Я\s]{4,}$"),
     ]
 }
 
 RES_OK = 0
 RES_TO_UPDATE = 1
@@ -95,38 +99,61 @@
         res = ""
 
     if res != s:
         logging.debug("Has incorrect symbols: '%s'->'%s'", s, res)
     return res
 
 
+def cut_long_words(s):
+    lis = []
+    words = s.split(" ")
+    for w in words:
+        lis.append(w[:30])
+
+    res = " ".join(lis)
+    if res != s:
+        logging.debug("Has long words: '%s'->'%s'", s, res)
+    return res
+
+
+def remove_duplicate_lines(src):
+    res = src[0:2]
+    for i in range(2, len(src)):
+        if src[i] != src[i - 1] or src[i] != src[i - 2]:
+            res.append(src[i])
+    if res != src:
+        logging.debug("Has string duplicates: '%s'->'%s'", src, res)
+    return res
+
+
 def check_text(text, language):
     if text == "":
         return text
 
     src = text.split("\n")
     res = []
     for t in src:
         if not has_hall_text(t, language):
             s = clean_wrong_symbols(t, language)
             if s == "":
                 logging.debug("Has empty string (was '%s')", t)
             else:
-                res.append(s)
+                res.append(cut_long_words(s))
+    res = remove_duplicate_lines(res)
     return "\n".join(res)
 
 
 class Verifier:
     def __init__(self, dryrun, force, sync):
         self.__dryrun = dryrun
         self.__force = force
         self.__sync_local = sync in ('all', 'local')
         self.__sync_notion = sync in ('all', 'notion')
         self.__cache = cache.Cache()
-        self.__notion = NotionClient(token_v2=os.getenv("NOTION_TOKEN"))
+        self.__notion = NotionClient(token_v2=os.getenv("MMDIARY_NOTION_TOKEN"))
         self.__language = os.getenv("MMDIARY_TRANSCRIBE_LANGUAGE", "ru")
 
         self.__local_sources = {}
 
         if len(self.__cache.list_existing_pages()) == 0:
             logging.warning("Empty cache")
```

### Comparing `mmdiary-0.2.0/src/mmdiary/utils/datelib.py` & `mmdiary-0.3.0/src/mmdiary/utils/datelib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 #!/usr/bin/python3
 
 import argparse
 import logging
 import os
 
+from fnmatch import fnmatch
 from collections import defaultdict
 
 from mmdiary.utils import log, medialib
 
 DESCRIPTION = """
 Diary video dates DB manipulation tool
 Please declare enviromnent variables before use:
-    VIDEO_LIB_ROOTS - List of video library root dirs
-    VIDEO_PROCESSOR_RES_DIR - Video processor result dir
+    MMDIARY_VIDEO_LIB_ROOTS - List of video library root dirs
+    MMDIARY_VIDEO_RES_DIR - Video processor result dir
 
 Possible actions:
-    list_dates - Print all dates with starus
-    disable_video - Set a flag for video file to disable concatenneting and uploading,
+    list_dates - Print all dates with status
+    list_files - Print all files for date
+    disable_video - Set a flag for video file to disable concatenating and uploading,
                     also mark corresponded date as not processed for future regeneration
+    list_disabled_videos - List videos marked as disabled 
     set_reupload - Mark a video as not uploaded for future reupload
                    (e.g. if video was deleted on the YouTube)
 """
 
 STATE_NONE = "none"
 STATE_INPROCESS = "inprocess"
 STATE_CONVERTED = "converted"
 STATE_UPLOADED = "uploaded"
 
+VALID_STATES = set(
+    [
+        STATE_NONE,
+        STATE_INPROCESS,
+        STATE_CONVERTED,
+        STATE_UPLOADED,
+    ]
+)
+
 
 class DateLib:
     def __init__(self):
         self.__scan_paths = list(
             filter(
                 None,
-                os.getenv("VIDEO_LIB_ROOTS").split(":"),
+                os.getenv("MMDIARY_VIDEO_LIB_ROOTS").split(":"),
             ),
         )
-        self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
+        self.__res_dir = os.getenv("MMDIARY_VIDEO_RES_DIR")
         self.__results = None
         self.__sources = None
 
     def __load_results(self):
         res = {}
         logging.debug("Process results: %s", self.__res_dir)
         lib = medialib.MediaLib(self.__res_dir)
@@ -84,39 +96,54 @@
             )
             fields["recordtime"] = date
             fields["type"] = "mergedvideo"
         self.results()[date].update_fields(fields)
 
     def set_converted(self, date, fields):
         new_fields = {}
-        new_fields.update(fields)
+        if fields is not None:
+            new_fields.update(fields)
         new_fields["state"] = STATE_CONVERTED
         self.results()[date].update_fields(new_fields)
 
     def set_uploaded(self, date, url):
         self.results()[date].update_fields({"state": STATE_UPLOADED, "url": url})
 
-    def get_nonprocessed(self):
+    def set_state(self, date, state):
+        if state not in VALID_STATES:
+            raise UserWarning(f"Incorrect state: {state}")
+        self.results()[date].update_fields({"state": state})
+
+    def get_nonprocessed(self, masks=None):
         all_dates = set(self.sources().keys())
-        processed_dates = set(self.__get_results_dates_by_state(STATE_NONE))
-        return all_dates - processed_dates
+        processed_dates = set(self.__get_results_dates_by_state(VALID_STATES - set([STATE_NONE])))
+        return sorted(self.__filter_by_masks(list(all_dates - processed_dates), masks))
 
-    def __get_results_dates_by_state(self, state):
+    def __filter_by_masks(self, dates, masks):
+        if masks is None or len(masks) == 0 or dates is None or len(dates) == 0:
+            return dates
+        if isinstance(next(iter(dates)), tuple):
+            return filter(lambda date: any(fnmatch(date[0], mask) for mask in masks), dates)
+        return filter(lambda date: any(fnmatch(date, mask) for mask in masks), dates)
+
+    def __get_results_dates_by_state(self, states, masks=None):
+        for state in states:
+            if state not in VALID_STATES:
+                raise UserWarning(f"Incorrect state: {state}")
         res = []
         for date, mf in self.results().items():
-            if mf.state() == state:
+            if mf.state() in states:
                 res.append(date)
-        res.sort()
-        return res
+        return sorted(self.__filter_by_masks(res, masks))
 
-    def get_converted(self):
-        return self.__get_results_dates_by_state(STATE_CONVERTED)
+    def get_converted(self, masks=None):
+        return self.__get_results_dates_by_state([STATE_CONVERTED], masks)
 
-    def get_uploaded(self):
-        return self.__get_results_dates_by_state(STATE_UPLOADED)
+    def get_uploaded(self, masks=None):
+        return self.__get_results_dates_by_state([STATE_UPLOADED], masks)
 
     def get_files_by_date(self, date, for_upload=False):
         mfs = self.sources()[date]
         if for_upload:
             mfs = list(filter(lambda mf: mf.json().get("upload", True), mfs))
         mfs.sort(key=lambda mf: mf.recordtime())
         return mfs
@@ -148,26 +175,24 @@
             return
 
         mf.update_fields({"upload": False})
 
         self.set_not_processed(mf.recorddate())
         logging.info("Video file %s disabled", mf.name())
 
-    def list_dates(self, state):
+    def list_dates(self, state, masks):
         if state is None:
             res = {date: STATE_NONE for date in set(self.sources().keys())}
             res.update({date: mf.state() for date, mf in self.results().items()})
-            res = list(res.items())
-            res.sort()
-            return res
+            return sorted(self.__filter_by_masks(res.items(), masks))
 
         if state == STATE_NONE:
-            return [(date, STATE_NONE) for date in self.get_nonprocessed()]
+            return [(date, STATE_NONE) for date in self.get_nonprocessed(masks)]
 
-        return [(date, state) for date in self.__get_results_dates_by_state(state)]
+        return [(date, state) for date in self.__get_results_dates_by_state([state], masks)]
 
     def list_disabled_videos(self):
         res = []
         for mfs in self.sources().values():
             for mf in mfs:
                 if not mf.json().get("upload", True):
                     res.append(mf.name())
@@ -183,39 +208,50 @@
         "-a",
         "--action",
         help="Action",
         required=True,
         choices=[
             "list_dates",
             "list_disabled_videos",
+            "list_files",
             "disable_video",
             "set_reupload",
         ],
     )
     parser.add_argument("-f", "--file", help="File name (for disable_video)")
-    parser.add_argument("-e", "--date", help="Date (for set_reupload)")
+    parser.add_argument("-e", "--date", help="Date (for set_reupload, list_files)")
     parser.add_argument("-s", "--state", help="State for (list_dates)")
     return parser.parse_args()
 
 
 def main():
     args = __args_parse()
     log.init_logger(level=logging.DEBUG)
     lib = DateLib()
 
     if args.action == "list_dates":
-        for date, state in lib.list_dates(args.state):
+        dates = lib.list_dates(args.state, [args.date] if args.date is not None else None)
+        for date, state in dates:
             print(date, state)
+        print("Total:", len(dates))
     elif args.action == "list_disabled_videos":
-        for filename in lib.list_disabled_videos():
+        filenames = lib.list_disabled_videos()
+        for filename in filenames:
             print(filename)
+        print("Total:", len(filenames))
+    elif args.action == "list_files":
+        mfs = lib.get_files_by_date(args.date)
+        for mf in mfs:
+            print(mf)
+        print("Total:", len(mfs))
     elif args.action == "disable_video":
         lib.disable_video(args.file)
+        logging.info("Done.")
     elif args.action == "set_reupload":
         if lib.get_state(args.date) != STATE_UPLOADED:
             logging.warning("Specified date not yet uploaded: %s", args.date)
         lib.set_converted(args.date, {})
-    logging.info("Done.")
+        logging.info("Done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mmdiary-0.2.0/src/mmdiary/utils/jsoncache.py` & `mmdiary-0.3.0/src/mmdiary/utils/jsoncache.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/src/mmdiary/utils/log.py` & `mmdiary-0.3.0/src/mmdiary/utils/log.py`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/src/mmdiary/utils/medialib.py` & `mmdiary-0.3.0/src/mmdiary/utils/medialib.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,14 @@
 
 
 def get_time_from_timestring(time):
     return time[10:]
 
 
 def main():
-    lib = MediaLib(os.getenv("AUDIO_NOTES_ROOT"))
+    lib = MediaLib(os.getenv("MMDIARY_AUDIO_LIB_ROOT"))
     for f in lib.get_new():
         print(f)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mmdiary-0.2.0/src/mmdiary/video/processor.py` & `mmdiary-0.3.0/src/mmdiary/video/processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,94 +9,128 @@
 import mixvideoconcat
 
 from mmdiary.utils import log, datelib, progressbar
 from mmdiary.utils.medialib import TIME_OUT_FORMAT
 
 
 DESCRIPTION = """
-Concatente siary videos and generate aggregated JSON file
+Concatente diary videos and generate aggregated JSON file
 Please declare enviromnent variables before use:
-    VIDEO_LIB_ROOTS - List of video library root dirs
-    VIDEO_PROCESSOR_WORK_DIR - Work dir for temp files (can be huge!) 
-    VIDEO_PROCESSOR_RES_DIR - Result dir
+    MMDIARY_VIDEO_LIB_ROOTS - List of video library root dirs
+    MMDIARY_VIDEO_WORK_DIR - Work dir for temp files (can be huge!) 
+    MMDIARY_VIDEO_RES_DIR - Result dir
 """
 
 
 class VideoProcessor:
-    def __init__(self, update_existing, json_only):
+    def __init__(self, update_existing, json_only, force, dry_run):
         self.__update_existing = update_existing
         self.__json_only = json_only
-        self.__work_dir = os.getenv("VIDEO_PROCESSOR_WORK_DIR")
+        self.__force = force
+        self.__dry_run = dry_run
+        self.__work_dir = os.getenv("MMDIARY_VIDEO_WORK_DIR")
         if not self.__work_dir:
-            raise UserWarning("VIDEO_PROCESSOR_WORK_DIR not defined")
+            raise UserWarning("MMDIARY_VIDEO_WORK_DIR not defined")
         os.makedirs(self.__work_dir, exist_ok=True)
-        self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
+        self.__res_dir = os.getenv("MMDIARY_VIDEO_RES_DIR")
         if not self.__res_dir:
-            raise UserWarning("VIDEO_PROCESSOR_WORK_DIR not defined")
+            raise UserWarning("MMDIARY_VIDEO_WORK_DIR not defined")
         os.makedirs(self.__res_dir, exist_ok=True)
 
         self.__lib = datelib.DateLib()
 
+    def __check_info_changed(self, mfiles, res_mf):
+        if not res_mf.have_field("videos"):
+            return len(mfiles) != 0
+
+        videos = {info["name"]: info for info in res_mf.get_field("videos")}
+        if len(videos) != len(mfiles):
+            return True
+
+        for mf in mfiles:
+            if mf.name() not in videos:
+                return True
+            info = videos[mf.name()]
+            if (
+                info["caption"] != mf.get_field("caption").strip()
+                or info["text"] != mf.get_field("text").strip()
+                or info["timestamp"] != mf.get_field("recordtime")
+            ):
+                return True
+        return False
+
     def __process_date(self, date):
         logging.info("Start: %s", date)
         res_mf = self.__lib.results()[date]
         starttime = datetime.now()
         mfiles = self.__lib.get_files_by_date(date, for_upload=True)
         fnames = [mf.name() for mf in mfiles]
         logging.info("found %i files", len(fnames))
 
+        if not self.__force and not self.__check_info_changed(mfiles, res_mf):
+            logging.debug("Date: %s not chnaged, skip", date)
+            return None
+
         if os.path.exists(res_mf.name()) and not self.__json_only:
             logging.debug("Remove existing result: %s", res_mf.name())
             os.unlink(res_mf.name())
 
         fileinfos = mixvideoconcat.concat(
-            fnames, res_mf.name(), self.__work_dir, dry_run=self.__json_only
+            fnames, res_mf.name(), self.__work_dir, dry_run=(self.__json_only or self.__dry_run)
         )
 
         videos_info = []
         for mf, info in zip(mfiles, fileinfos):
             mf_info = mf.json()
             info["caption"] = mf_info["caption"].strip()
             info["text"] = mf_info["text"].strip()
-            info["timestamp"] = mf.prop().time().strftime(TIME_OUT_FORMAT)
+            info["timestamp"] = mf_info["recordtime"]
             videos_info.append(info)
 
         processduration = (datetime.now() - starttime).total_seconds()
 
         fields = {
             "videos": videos_info,
             "processduration": processduration,
             "processtime": datetime.now().strftime(TIME_OUT_FORMAT),
             "source": os.path.split(res_mf.name())[1],
             "recordtime": date,
             "type": "mergedvideo",
         }
-        self.__lib.set_converted(date, fields)
-
         logging.info("Done: %s: %s", date, res_mf.json_name())
+        return fields
 
     def process_date(self, date):
         if not self.__update_existing and not self.__json_only:
             if self.__lib.get_state(date) != datelib.STATE_NONE:
                 logging.warning("date: %s already processed, skip", date)
                 return
 
-        self.__lib.set_in_progress(date)
-        try:
-            self.__process_date(date)
-        except (Exception, KeyboardInterrupt):
-            self.__lib.set_not_processed(date)
-            raise
+        if not self.__dry_run:
+            old_state = self.__lib.get_state(date)
+            self.__lib.set_in_progress(date)
+            try:
+                fields = self.__process_date(date)
+                if fields is not None:
+                    self.__lib.set_converted(date, fields)
+                else:
+                    self.__lib.set_state(date, old_state)
+            except:
+                self.__lib.set_state(date, old_state)
+                raise
+        else:
+            fields = self.__process_date(date)
+            logging.debug("dry_run result: %s", fields)
 
-    def process_all(self):
+    def process_all(self, masks):
         toprocess = []
-        if self.__json_only:
-            toprocess = list(self.__lib.get_converted()) + list(self.__lib.get_uploaded())
+        if self.__update_existing:
+            toprocess = sorted(self.__lib.get_converted(masks) + self.__lib.get_uploaded(masks))
         else:
-            toprocess = list(self.__lib.get_nonprocessed())
+            toprocess = self.__lib.get_nonprocessed(masks)
 
         pbar = progressbar.start("Process", len(toprocess))
         for date in toprocess:
             try:
                 self.process_date(date)
             except Exception:
                 logging.exception("Video processing failed")
@@ -107,35 +141,37 @@
 def __args_parse():
     parser = argparse.ArgumentParser(
         description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument(
         "dates", nargs="*", help="Date to process (otherwise all dates will be processed)"
     )
-    parser.add_argument('-l', '--logfile', help='Log file', default=None)
-    parser.add_argument('-u', '--update', help='Update existing', action='store_true')
+    parser.add_argument("-l", "--logfile", help="Log file", default=None)
+    parser.add_argument(
+        "-u", "--update", help="Update already processed, if changed", action="store_true"
+    )
+    parser.add_argument("-f", "--force", help="Force update already processed", action="store_true")
+    parser.add_argument(
+        "-d", "--dry-run", help="Only analize, without real changes", action="store_true"
+    )
     parser.add_argument(
-        '--json-only',
-        help='Only regenerate existing JSONs without video files regeneration',
-        action='store_true',
+        "--json-only",
+        help="Only generate JSONs without video files generation",
+        action="store_true",
     )
     return parser.parse_args()
 
 
 def main():
     args = __args_parse()
     log.init_logger(args.logfile, logging.DEBUG)
     logging.getLogger("py.warnings").setLevel(logging.ERROR)
 
-    vp = VideoProcessor(args.update, args.json_only)
+    vp = VideoProcessor(args.update, args.json_only, args.force, args.dry_run)
 
-    if len(args.dates) == 0:
-        vp.process_all()
-    else:
-        for date in args.dates:
-            vp.process_date(date)
+    vp.process_all(args.dates)
 
     logging.info("Processor done.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mmdiary-0.2.0/src/mmdiary/video/uploader.py` & `mmdiary-0.3.0/src/mmdiary/video/uploader.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,25 @@
 from datetime import datetime
 
 import googleapiclient.discovery
 
 from mmdiary.utils import log, datelib, progressbar
 from mmdiary.utils.medialib import TIME_OUT_FORMAT, split_large_text
 
+DESCRIPTION = """
+Uploads generated diary videos to YouTube
+Please declare enviromnent variables before use:
+    MMDIARY_YOUTUBE_CLIENT_SECRETS - Path/filename to the client_secrets.json file for YouTube API
+        Can be found/created there: https://console.cloud.google.com/apis/credentials
+    MMDIARY_YOUTUBE_TOKEN - Path/filename to the cached YouTube token
+        Path must exists, file will be created after the first authorization
+    MMDIARY_VIDEO_LIB_ROOTS - List of video library root dirs
+    MMDIARY_VIDEO_RES_DIR - Result dir
+"""
+
 YOUTUBE_MAX_DESCRIPTION = 5000
 YOUTUBE_MAX_COMMENT = 5000
 YOUTUBE_URL = "https://www.youtube.com/watch?v="
 
 
 def generate_video_url(video_id):
     return YOUTUBE_URL + video_id
@@ -98,20 +109,22 @@
         return description
 
     logging.warning("description cutted")
     return description[:YOUTUBE_MAX_DESCRIPTION]
 
 
 class VideoUploader:
-    def __init__(self):
-        self.__res_dir = os.getenv("VIDEO_PROCESSOR_RES_DIR")
-        os.makedirs(self.__res_dir, exist_ok=True)
+    def __init__(self, update):
+        self.__update = update
 
         self.__lib = datelib.DateLib()
-        self.__credentials = get_youtube_credentials("client_secrets.json", "token.json")
+        self.__credentials = get_youtube_credentials(
+            os.path.expanduser(os.getenv("MMDIARY_YOUTUBE_CLIENT_SECRETS", "client_secrets.json")),
+            os.path.expanduser(os.getenv("MMDIARY_YOUTUBE_TOKEN", "token.json")),
+        )
         self.__youtube = googleapiclient.discovery.build(
             "youtube", "v3", credentials=self.__credentials
         )
 
     def __gen_time_labels(self, data, text_field, delimiter=" ", skip_empty=False):
         time_labels = []
         for info in data["videos"]:
@@ -152,15 +165,61 @@
                 return None
             if ex.status_code == 400 and ex.error_details[0]["reason"] == "uploadLimitExceeded":
                 logging.error("uploadLimitExceeded")
                 return None
 
             raise
 
+    def update_video(self, video_id, title, time_labels):
+        logging.debug("Update video: %s", video_id)
+        request = self.__youtube.videos().update(
+            part="snippet",
+            body={
+                "id": video_id,
+                "snippet": {
+                    "title": title,
+                    "description": generate_description(time_labels),
+                    "tags": ["daily"],
+                    "categoryId": "22",
+                },
+            },
+        )
+        request.execute()
+
+    def __list_comments(self, video_id):
+        try:
+            request = self.__youtube.commentThreads().list(
+                part="snippet", videoId=video_id, maxResults=100
+            )
+
+            comment_ids = []
+            while request:
+                response = request.execute()
+                for item in response["items"]:
+                    comment_ids.append(item["id"])
+                request = self.__youtube.commentThreads().list_next(request, response)
+
+            return comment_ids
+        except googleapiclient.errors.HttpError as ex:
+            if ex.status_code == 403 and ex.error_details[0]["reason"] == "commentsDisabled":
+                logging.debug("commentsDisabled")
+                return []
+            if ex.status_code == 404 and ex.error_details[0]["reason"] == "videoNotFound":
+                raise UserWarning("videoNotFound") from None
+            raise
+
+    def delete_comments(self, video_id):
+        comment_ids = self.__list_comments(video_id)
+        logging.debug("Remove comments for fideo %s: %s", video_id, comment_ids)
+        for comment_id in comment_ids:
+            self.__youtube.comments().delete(id=comment_id).execute()
+
     def add_comment(self, video_id, comment_text):
+        if comment_text == "":
+            return
         request = self.__youtube.commentThreads().insert(
             part="snippet",
             body={
                 "snippet": {
                     "videoId": video_id,
                     "topLevelComment": {"snippet": {"textOriginal": comment_text}},
                 }
@@ -171,90 +230,139 @@
         response = request.execute()
         logging.debug(response)
 
     def delete_video(self, video_id):
         logging.info("Delete: %s", video_id)
         self.__youtube.videos().delete(id=video_id).execute()
 
+    def check_video_exists(self, video_id):
+        request = self.__youtube.videos().list(part="snippet", id=video_id)
+        response = request.execute()
+
+        return 'items' in response and len(response['items']) > 0
+
     def process_date(self, date):
         mf = self.__lib.results()[date]
         data = mf.json()
-        logging.info("Upload: %s", date)
+        logging.info("Process: %s", date)
 
-        if not mf.have_file():
-            raise FileNotFoundError("Source video file not exists")
         if not mf.have_json():
             raise FileNotFoundError("Json file not exists")
 
-        if "url" in data:
-            try:
-                self.delete_video(extract_video_id(data["url"]))
-            except Exception:
-                logging.exception("Video deletion failed")
+        update = self.__update or not mf.have_file()
+        if update:
+            logging.debug("Update only")
 
         time_labels = self.__gen_time_labels(data, "caption")
         comments_text = self.__gen_comments(data)
         logging.debug(comments_text)
 
-        video_id = self.upload_video(mf.name(), date, time_labels)
-        if video_id is None:
-            return False
+        video_id = None
+        if update:
+            if "url" not in data:
+                raise UserWarning("URL file missed, update impossible")
+            video_id = extract_video_id(data["url"])
+            self.delete_comments(video_id)
+            self.update_video(video_id, date, time_labels)
+        else:
+            if "url" in data:
+                try:
+                    self.delete_video(extract_video_id(data["url"]))
+                except Exception:
+                    logging.exception(
+                        "Video deletion failed, possible it was removed by YouTube, skip uploading"
+                    )
+                    raise
+
+            video_id = self.upload_video(mf.name(), date, time_labels)
+            if video_id is None:
+                return False
 
         for comment_text in comments_text:
             try:
                 self.add_comment(video_id, comment_text)
             except Exception:
                 logging.exception("Add comment failed")
 
         url = generate_video_url(video_id)
         logging.info("Video uploaded: %s", url)
         self.__lib.set_uploaded(date, url)
         logging.info("Upload done: %s", date)
         return True
 
-    def process_all(self):
-        converted = list(self.__lib.get_converted())
+    def process_all(self, masks):
+        converted = list(self.__lib.get_converted(masks))
 
         pbar = progressbar.start("Upload", len(converted))
         err_count = 0
         for date in converted:
             try:
                 if not self.process_date(date):
                     return pbar.value, err_count
             except Exception:
                 err_count += 1
                 logging.exception("Video uploading failed")
 
             pbar.increment()
         return pbar.value, err_count
 
+    def verify_urls(self, masks):
+        toprocess = sorted(self.__lib.get_converted(masks) + self.__lib.get_uploaded(masks))
+        res = {"count": len(toprocess), "err": 0, "no_url": 0, "exists": 0, "not_exists": 0}
+        for date in toprocess:
+            try:
+                mf = self.__lib.results()[date]
+                data = mf.json()
+                if "url" not in data:
+                    res["no_url"] += 1
+                    continue
+                video_id = extract_video_id(data["url"])
+                is_exists = self.check_video_exists(video_id)
+                if is_exists:
+                    res["exists"] += 1
+                else:
+                    res["not_exists"] += 1
+                logging.info("Video %s is exists: %s", date, is_exists)
+            except Exception:
+                res["err"] += 1
+                logging.exception("Video verification failed")
+        return res
+
 
 def __args_parse():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("dates", nargs="*", help="Date to process")
-    parser.add_argument('-l', '--logfile', help='Log file', default=None)
+    parser = argparse.ArgumentParser(
+        description=DESCRIPTION, formatter_class=argparse.RawTextHelpFormatter
+    )
+    parser.add_argument("dates", nargs="*", help="Dates to process")
+    parser.add_argument("-l", "--logfile", help="Log file", default=None)
+    parser.add_argument(
+        "-u",
+        "--update",
+        help="Update video description/comment without reupload",
+        action='store_true',
+    )
+    parser.add_argument(
+        "--verify-urls", help="Verify uploaded videos by urls check", action='store_true'
+    )
     return parser.parse_args()
 
 
 def main():
     args = __args_parse()
     log.init_logger(args.logfile, logging.DEBUG)
     logging.getLogger("py.warnings").setLevel(logging.ERROR)
 
-    vup = VideoUploader()
+    vup = VideoUploader(args.update)
 
-    res_count = 0
-    err_count = 0
-    if len(args.dates) == 0:
-        res_count, err_count = vup.process_all()
-    else:
-        for date in args.dates:
-            vup.process_date(date)
-            res_count += 1
+    if args.verify_urls:
+        res = vup.verify_urls(args.dates)
+        logging.info("Verification done: %s", res)
+        return
 
+    res_count, err_count = vup.process_all(args.dates)
     logging.info("Uploader done: %s, errors: %s", res_count, err_count)
 
 
 if __name__ == "__main__":
     try:
         main()
     except Exception:
```

### Comparing `mmdiary-0.2.0/src/mmdiary.egg-info/PKG-INFO` & `mmdiary-0.3.0/src/mmdiary.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmdiary
-Version: 0.2.0
+Version: 0.3.0
 Summary: Multimedia Diary Tools
 Author-email: Alexander Bushnev <Alexander@Bushnev.pro>
 Maintainer-email: Alexander Bushnev <Alexander@Bushnev.pro>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -680,15 +680,15 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/sashacmc/mmdiary
 Project-URL: Bug Reports, https://github.com/sashacmc/mmdiary/issues
 Project-URL: Source, https://github.com/sashacmc/mmdiary/
 Project-URL: Changelog, https://github.com/sashacmc/mmdiary/blob/master/CHANGELOG.md
 Keywords: audio,video,multimedia,tool,youtube,notion,transcriber,uploader
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -715,31 +715,272 @@
 
 You can install MultiMedia Diary Tools via pip:
 
 ```bash
 pip install mmdiary
 ```
 
-## Command line tool usage
+## Environment Setup
+
+Ensure you set the necessary environment variables:
+
+- `MMDIARY_AUDIO_LIB_ROOT`: Root directory for audio notes.
+- `MMDIARY_VIDEO_LIB_ROOTS`: Root directories for video notes (multiple roots can be specified, separated by semicolon).
+- `MMDIARY_VIDEO_WORK_DIR`: Work dir for video processing (can be HUGE)
+- `MMDIARY_VIDEO_RES_DIR`: Results dir for video diary files
+- `MMDIARY_NOTION_API_KEY`: Your Notion API Key (see below).
+- `MMDIARY_NOTION_TOKEN`: Your Notion Auth Token v2 (see below).
+- `MMDIARY_NOTION_CACHE`: Notion uploader cache file
+- `MMDIARY_CACHE`: JSON processing cache file (to avoid reading all transribed files each run)
+- `MMDIARY_YOUTUBE_CLIENT_SECRETS`: Path to `client_secrets.json` (see below)
+- `MMDIARY_YOUTUBE_TOKEN`: Path to `token.json` (see below)
+- `MMDIARY_NOTION_AUDIO_DB_ID`: Notion Audio DB ID (see below)
+- `MMDIARY_NOTION_VIDEO_DB_ID`: Notion Video DB ID (see below) 
+
+
+Example:
+
+```bash
+export MMDIARY_AUDIO_LIB_ROOT="/path/to/audio/library"
+export MMDIARY_VIDEO_LIB_ROOTS="/path/to/video/library1:/path/to/video/library2"
+export MMDIARY_VIDEO_WORK_DIR=/"path/to/work/dir"
+export MMDIARY_VIDEO_RES_DIR="/path/to/wideo/result/dir"
+export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
+export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
+export MMDIARY_NOTION_CACHE="~/.mmdiary/notion_cache.pickle"
+export MMDIARY_CACHE="~/.mmdiary/json_cache.pickle"
+export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
+export MMDIARY_YOUTUBE_TOKEN="~/.mmdiary/token.json"
+export MMDIARY_NOTION_AUDIO_DB_ID="7da1480baa9f565198d3fa54c49b1b23"
+export MMDIARY_NOTION_VIDEO_DB_ID="25225aac51ea5cf0bcc74f8c225fbb63"
+```
+
+## Recommended Tools
+
+To ensure unique filenames for your files, it is recommended to use the [photo-importer](https://github.com/sashacmc/photo-importer) tool.
+
+## Notion Setup
+
+To integrate Multimedia Diary Tools with Notion, you'll need to set up both an API Key and an Auth Token v2. This dual setup is necessary because the API Key allows for fast and efficient operations via the official API, while the Auth Token v2 enables functionalities not available through the official API, such as file uploads and locking pages for editing.
+
+### Obtaining and Setting Up the Notion API Key
+
+1. **Create an Integration in Notion**:
+   - Go to [Notion Integrations](https://www.notion.so/my-integrations) and click on "New Integration".
+   - Follow the instructions to create a new integration and obtain your API Key.
+
+2. **Set the Environment Variable**:
+   - Save the API Key in an environment variable named `MMDIARY_NOTION_API_KEY`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_NOTION_API_KEY="your_notion_api_key_here"
+     ```
+
+### Obtaining and Setting Up the Notion Auth Token v2
+
+1. **Extract the Auth Token v2 from Your Browser**:
+   - Open Notion in your web browser and log in.
+   - Open the developer tools (usually by pressing `F12` or right-clicking on the page and selecting "Inspect").
+   - Go to the "Application" tab and find the `token_v2` under Cookies for `notion.so`.
+   - Copy the value of the `token_v2`.
+
+2. **Set the Environment Variable**:
+   - Save the Auth Token v2 in an environment variable named `MMDIARY_NOTION_TOKEN`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_NOTION_TOKEN="your_notion_auth_token_v2_here"
+     ```
+
+### Initializing Notion Databases
+
+Before you can upload audio (with text) and links to videos (with text) to Notion, you need to create the necessary databases. Follow these steps:
+
+1. **Run the Initialization Script**:
+   - Use the `mmdiary-notion-upload` utility with the `--init` option to create the required databases on a specified Notion page.
+   - Command:
+     ```bash
+     mmdiary-notion-upload --init ROOT_PAGE_ID
+     ```
+   - Make sure the integration has access to this page.
+
+2. **Set the Database IDs as Environment Variables**:
+   - After running the script, two databases will be created on the specified page. Retrieve their IDs and save them in environment variables.
+   - Example:
+     ```bash
+     export MMDIARY_NOTION_AUDIO_DB_ID='7da1480baa9f565198d3fa54c49b1b23'
+     export MMDIARY_NOTION_VIDEO_DB_ID='25225aac51ea5cf0bcc74f8c225fbb63'
+     ```
+
+3. **Move the Databases if Needed**:
+   - You can move the databases to other pages or to the root of your workspace. If you do this, ensure the integration still has access to them.
+
+## YouTube Setup
+
+### Obtaining and Setting Up the YouTube API Client Secrets
+
+1. **Create a Project in Google Developers Console**:
+   - Go to the [Google Developers Console](https://console.developers.google.com/).
+   - Create a new project or select an existing project.
+   - Enable the YouTube Data API v3 for the project.
+
+2. **Obtain the Client Secrets File**:
+   - Go to the Credentials section in your project.
+   - Click on "Create Credentials" and select "OAuth 2.0 Client IDs".
+   - Follow the instructions to create an OAuth 2.0 Client ID.
+   - Download the `client_secrets.json` file and save it and provide a path in an environment variable named `MMDIARY_YOUTUBE_CLIENT_SECRETS`.
+   - Example for Unix-based systems:
+     ```bash
+     export MMDIARY_YOUTUBE_CLIENT_SECRETS="~/.mmdiary/client_secrets.json"
+     ```
+### Setting the Upload Limit
+
+By default, the maximum number of videos that can be uploaded via the YouTube API is 4 per day. To request an extension:
+
+1. **Go to the YouTube API Quota Request Form**:
+   - Visit the [YouTube API Quota Request Form](https://support.google.com/youtube/contact/yt_api_form).
+
+2. **Submit the Request**:
+   - Fill out the form with the necessary details about your project and the reasons for needing a higher quota.
+   - Submit the form and wait for approval from the YouTube API team.
+
+### Authenticating with YouTube API
+
+On the first run of `mmdiary-video-upload`, a URL will be provided. Follow these steps:
+
+1. **Open the URL**:
+   - Copy the provided URL and paste it into your web browser.
+   - Select the Google account authorized for your `client_secrets.json`.
+
+2. **Enter the Authentication Code**:
+   - Copy the authentication code provided after logging in.
+   - Paste the authentication code into the prompt in your terminal.
+   - This code will be saved in file specified by `MMDIARY_YOUTUBE_TOKEN` environment variable, and you won't need to repeat this process for future uploads.
+     
+## Step-By-Step Process Overview
+
+### Audio Diary
+
+#### Speech Recognition
+
+Use the `mmdiary-transcriber-run` utility to perform speech-to-text transcription on audio files.
+
+Command:
+
+```bash
+mmdiary-transcriber-run /path/to/audio/files
+```
+
+#### Upload to Notion
+
+Use the `mmdiary-notion-upload` utility to upload the transcribed text and audio files to Notion.
+
+Command:
+```bash
+mmdiary-notion-upload /path/to/audio/files
+```
+
+### Video Diary
+
+#### Speech Recognition
+
+Use the `mmdiary-transcriber-run` utility to perform speech-to-text transcription on video files.
+
+Command:
+
+```bash
+mmdiary-transcriber-run /path/to/video/files
+```
+
+#### Daily Video Concatenation
+
+Use the `mmdiary-video-concat` utility to merge video files into a single daily video.
+
+Command:
+```bash
+mmdiary-video-concat [dates ...]
+```
+
+#### Upload to YouTube
+
+Use the `mmdiary-video-upload` utility to upload the concatenated video to YouTube.
+
+Command:
+```bash
+mmdiary-video-upload [dates ...]
+```
+
+#### Upload to Notion
+
+Use the `mmdiary-notion-upload` utility to upload the transcribed text with YouTube links to Notion.
+
+Command:
+```bash
+mmdiary-notion-upload "$MMDIARY_VIDEO_RES_DIR"
+```
+
+## Auxiliary Tools
+
+### mmdiary-transcriber-search
+
+The `mmdiary-transcriber-search` utility allows you to search through transcribed texts for specific strings. This can be useful for quickly finding occurrences of certain keywords or phrases within your audio or video transcriptions.
+
+#### Usage
 
-### Transcribe files
 ```bash
-mmdiary-transcriber-run /path/to/folder/with/media/files
+mmdiary-transcriber-search /path/to/transcribed/files "search string"
 ```
-### Upload to notion
+
+### mmdiary-transcriber-verify
+
+The `mmdiary-transcriber-verify` utility checks the generated text from the speech-to-text transcriptions and filters out any garbage data. By default, this verification is performed automatically. Manual invocation of this tool is only necessary if the code has been modified (either manually or after updating the version) to avoid re-running the entire lengthy speech recognition process from scratch.
+
+#### Usage
+
+Simply run the utility specifying the paths to the directories or files you wish to verify in interactive mode
+
 ```bash
-mmdiary-notion-upload /path/to/folder/with/media/files
+mmdiary-transcriber-verify /path/to/transcribed/files
 ```
-### Concat video files
+
+Or run the utility with flag `-d` to check all and after with flag `-f` to apply all
+
 ```bash
-mmdiary-video-concat
+mmdiary-transcriber-verify /path/to/transcribed/files -d
+[check output]
+mmdiary-transcriber-verify /path/to/transcribed/files -f
 ```
-### Upload to notion
+
+### mmdiary-utils-datelib
+
+The `mmdiary-utils-datelib` utility provides various functions for managing and querying your multimedia video diary files by date. It includes options to list dates, list files, disable videos, list disabled videos, and set videos for re-upload.
+
+#### Usage
+
+Possible actions:
+
+- `list_dates`: Print all dates with status.
+- `list_files`: Print all files for a date.
+- `disable_video`: Set a flag for a video file to disable concatenating and uploading, also mark the corresponding date as not processed for future regeneration.
+- `list_disabled_videos`: List videos marked as disabled.
+- `set_reupload`: Mark a video as not uploaded for future re-upload (e.g., if the video was deleted on YouTube).
+
+Example:
+
 ```bash
-mmdiary-video-upload
+# list all dates with status "converted"
+mmdiary-utils-datelib -a list_dates -s converted
+
+# list files for date 2010-09-13
+mmdiary-utils-datelib -a list_files --date 2010-09-13
+
+# disable video
+mmdiary-utils-datelib -a disable_video -f 2010-04-14_17-09-50
+
+# set date 2024-03-15 to reupload
+mmdiary-utils-datelib -a set_reupload -e 2024-03-15
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.
 
 ## Show your support
```

### Comparing `mmdiary-0.2.0/src/mmdiary.egg-info/SOURCES.txt` & `mmdiary-0.3.0/src/mmdiary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmdiary-0.2.0/src/mmdiary.egg-info/entry_points.txt` & `mmdiary-0.3.0/src/mmdiary.egg-info/entry_points.txt`

 * *Files identical despite different names*

