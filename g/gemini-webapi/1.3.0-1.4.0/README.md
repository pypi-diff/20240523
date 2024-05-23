# Comparing `tmp/gemini_webapi-1.3.0.tar.gz` & `tmp/gemini_webapi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_webapi-1.3.0.tar", last modified: Wed May 22 00:26:05 2024, max compression
+gzip compressed data, was "gemini_webapi-1.4.0.tar", last modified: Thu May 23 21:36:03 2024, max compression
```

## Comparing `gemini_webapi-1.3.0.tar` & `gemini_webapi-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.488650 gemini_webapi-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.488650 gemini_webapi-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55231 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55231 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_save_image.py
```

### Comparing `gemini_webapi-1.3.0/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/.gitignore` & `gemini_webapi-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/LICENSE` & `gemini_webapi-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/PKG-INFO` & `gemini_webapi-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.3.0
+Version: 1.4.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -815,19 +815,22 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generate contents from image (currently only supports one image at a time). Optionally, you can pass image data in `bytes` or its path in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
-    response = await client.generate_content("Describe the image", image="assets/banner.png")
+    response = await client.generate_content(
+            "Describe each of these images",
+            images=["assets/banner.png", "assets/favicon.png"],
+        )
     print(response.text)
 
 asyncio.run(main())
 ```
 
 ### Conversations across multiple turns
```

### Comparing `gemini_webapi-1.3.0/README.md` & `gemini_webapi-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,19 +133,22 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generate contents from image (currently only supports one image at a time). Optionally, you can pass image data in `bytes` or its path in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
-    response = await client.generate_content("Describe the image", image="assets/banner.png")
+    response = await client.generate_content(
+            "Describe each of these images",
+            images=["assets/banner.png", "assets/favicon.png"],
+        )
     print(response.text)
 
 asyncio.run(main())
 ```
 
 ### Conversations across multiple turns
```

#### html2text {}

```diff
@@ -61,20 +61,20 @@
 recommended to set `auto_close` to `True` combined with reasonable seconds of
 `close_delay` for better resource management. ### Generate contents from text
 Ask a one-turn quick question by calling `GeminiClient.generate_content`.
 ```python async def main(): response = await client.generate_content("Hello
 World!") print(response.text) asyncio.run(main()) ``` > [!TIP] > > Simply use
 `print(response)` to get the same output if you just want to see the response
 text ### Generate contents from image Gemini supports image recognition and
-generate contents from image (currently only supports one image at a time).
-Optionally, you can pass image data in `bytes` or its path in `str` to
-`GeminiClient.generate_content` together with text prompt. ```python async def
-main(): response = await client.generate_content("Describe the image",
-image="assets/banner.png") print(response.text) asyncio.run(main()) ``` ###
-Conversations across multiple turns If you want to keep conversation
+generating contents from images. Optionally, you can pass images in a list of
+file data in `bytes` or their paths in `str` to `GeminiClient.generate_content`
+together with text prompt. ```python async def main(): response = await
+client.generate_content( "Describe each of these images", images=["assets/
+banner.png", "assets/favicon.png"], ) print(response.text) asyncio.run(main())
+``` ### Conversations across multiple turns If you want to keep conversation
 continuous, please use `GeminiClient.start_chat` to create a `ChatSession`
 object and send messages through it. The conversation history will be
 automatically handled and get updated after each turn. ```python async def main
 (): chat = client.start_chat() response1 = await chat.send_message("Briefly
 introduce Europe") response2 = await chat.send_message("What's the population
 there?") print(response1.text, response2.text, sep="\n\n-----------------------
 -----------\n\n") asyncio.run(main()) ``` > [!TIP] > > Same as
```

### Comparing `gemini_webapi-1.3.0/assets/banner.png` & `gemini_webapi-1.4.0/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/assets/logo.svg` & `gemini_webapi-1.4.0/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/pyproject.toml` & `gemini_webapi-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/client.py` & `gemini_webapi-1.4.0/src/gemini_webapi/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,20 +104,20 @@
         secure_1psid: str | None = None,
         secure_1psidts: str | None = None,
         proxies: dict | None = None,
     ):
         self.cookies = {}
         self.proxies = proxies
         self.running: bool = False
-        self.client: AsyncClient = None
-        self.access_token: str = None
+        self.client: AsyncClient | None = None
+        self.access_token: str | None = None
         self.timeout: float = 30
         self.auto_close: bool = False
         self.close_delay: float = 300
-        self.close_task: Task = None
+        self.close_task: Task | None = None
         self.auto_refresh: bool = True
         self.refresh_interval: float = 540
 
         # Validate cookies
         if secure_1psid:
             self.cookies["__Secure-1PSID"] = secure_1psid
             if secure_1psidts:
@@ -248,26 +248,26 @@
                 self.cookies["__Secure-1PSIDTS"] = new_1psidts
             await asyncio.sleep(self.refresh_interval)
 
     @running(retry=1)
     async def generate_content(
         self,
         prompt: str,
-        image: bytes | str | None = None,
+        images: list[bytes | str] | None = None,
         chat: Optional["ChatSession"] = None,
     ) -> ModelOutput:
         """
         Generates contents with prompt.
 
         Parameters
         ----------
         prompt: `str`
             Prompt provided by user.
-        image: `bytes` | `str`, optional
-            File data in bytes, or path to the image file to be sent together with the prompt.
+        images: `list[bytes | str]`, optional
+            List of image file data in bytes or file paths in string.
         chat: `ChatSession`, optional
             Chat data to retrieve conversation history. If None, will automatically generate a new chat id when sending post request.
 
         Returns
         -------
         :class:`ModelOutput`
             Output data from gemini.google.com, use `ModelOutput.text` to get the default text reply, `ModelOutput.images` to get a list
@@ -296,20 +296,30 @@
                 data={
                     "at": self.access_token,
                     "f.req": json.dumps(
                         [
                             None,
                             json.dumps(
                                 [
-                                    image
+                                    images
                                     and [
                                         prompt,
                                         0,
                                         None,
-                                        [[[await upload_file(image, self.proxies), 1]]],
+                                        [
+                                            [
+                                                [
+                                                    await upload_file(
+                                                        image, self.proxies
+                                                    ),
+                                                    1,
+                                                ]
+                                            ]
+                                            for image in images
+                                        ],
                                     ]
                                     or [prompt],
                                     None,
                                     chat and chat.metadata,
                                 ]
                             ),
                         ]
@@ -471,26 +481,26 @@
         super().__setattr__(name, value)
         # update conversation history when last output is updated
         if name == "last_output" and isinstance(value, ModelOutput):
             self.metadata = value.metadata
             self.rcid = value.rcid
 
     async def send_message(
-        self, prompt: str, image: bytes | str | None = None
+        self, prompt: str, images: list[bytes | str] | None = None,
     ) -> ModelOutput:
         """
         Generates contents with prompt.
         Use as a shortcut for `GeminiClient.generate_content(prompt, image, self)`.
 
         Parameters
         ----------
         prompt: `str`
             Prompt provided by user.
-        image: `bytes` | `str`, optional
-            File data in bytes, or path to the image file to be sent together with the prompt.
+        images: `list[bytes | str]`, optional
+            List of image file data in bytes or file paths in string.
 
         Returns
         -------
         :class:`ModelOutput`
             Output data from gemini.google.com, use `ModelOutput.text` to get the default text reply, `ModelOutput.images` to get a list
             of images in the default reply, `ModelOutput.candidates` to get a list of all answer candidates in the output.
 
@@ -503,15 +513,15 @@
         `gemini_webapi.GenimiError`
             If no reply candidate found in response.
         `gemini_webapi.APIError`
             - If request failed with status code other than 200.
             - If response structure is invalid and failed to parse.
         """
         return await self.geminiclient.generate_content(
-            prompt=prompt, image=image, chat=self
+            prompt=prompt, images=images, chat=self
         )
 
     def choose_candidate(self, index: int) -> ModelOutput:
         """
         Choose a candidate from the last `ModelOutput` to control the ongoing conversation flow.
 
         Parameters
```

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/constants.py` & `gemini_webapi-1.4.0/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.4.0/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.4.0/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/types/image.py` & `gemini_webapi-1.4.0/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.4.0/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.4.0/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.4.0/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.4.0/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.4.0/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.4.0/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.4.0/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.3.0
+Version: 1.4.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -815,19 +815,22 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generate contents from image (currently only supports one image at a time). Optionally, you can pass image data in `bytes` or its path in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
-    response = await client.generate_content("Describe the image", image="assets/banner.png")
+    response = await client.generate_content(
+            "Describe each of these images",
+            images=["assets/banner.png", "assets/favicon.png"],
+        )
     print(response.text)
 
 asyncio.run(main())
 ```
 
 ### Conversations across multiple turns
```

### Comparing `gemini_webapi-1.3.0/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.4.0/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 .github/workflows/github-release.yml
 .github/workflows/pypi-publish.yml
 .vscode/launch.json
 .vscode/settings.json
 assets/banner.png
+assets/favicon.png
 assets/logo.svg
 src/gemini_webapi/__init__.py
 src/gemini_webapi/client.py
 src/gemini_webapi/constants.py
 src/gemini_webapi/exceptions.py
 src/gemini_webapi.egg-info/PKG-INFO
 src/gemini_webapi.egg-info/SOURCES.txt
```

### Comparing `gemini_webapi-1.3.0/tests/test_client_features.py` & `gemini_webapi-1.4.0/tests/test_client_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     async def test_successful_request(self):
         response = await self.geminiclient.generate_content("Hello World!")
         self.assertTrue(response.text)
 
     @logger.catch(reraise=True)
     async def test_upload_image(self):
         response = await self.geminiclient.generate_content(
-            "Describe the image", image="assets/banner.png"
+            "Describe the image", images=["assets/banner.png"]
         )
         self.assertTrue(response.text)
         logger.debug(response.text)
 
     @logger.catch(reraise=True)
     async def test_continuous_conversation(self):
         chat = self.geminiclient.start_chat()
@@ -55,19 +55,20 @@
         response = await previous_chat.send_message("What was my previous message?")
         logger.debug(response)
 
     @logger.catch(reraise=True)
     async def test_chatsession_with_image(self):
         chat = self.geminiclient.start_chat()
         response1 = await chat.send_message(
-            "Describe the image", image="assets/banner.png"
+            "What's the difference between these two images?",
+            images=["assets/pic1.png", "assets/pic2.png"],
         )
         self.assertTrue(response1.text)
         logger.debug(response1.text)
-        response2 = await chat.send_message("Tell me more about it.")
+        response2 = await chat.send_message("Tell me more.")
         self.assertTrue(response2.text)
         logger.debug(response2.text)
 
     @logger.catch(reraise=True)
     async def test_send_web_image(self):
         response = await self.geminiclient.generate_content(
             "Send me some pictures of cats"
```

### Comparing `gemini_webapi-1.3.0/tests/test_rotate_cookies.py` & `gemini_webapi-1.4.0/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.3.0/tests/test_save_image.py` & `gemini_webapi-1.4.0/tests/test_save_image.py`

 * *Files identical despite different names*

