# Comparing `tmp/sdl-webui-lite-0.1.1.tar.gz` & `tmp/sdl-webui-lite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdl-webui-lite-0.1.1.tar", last modified: Thu May 23 20:45:25 2024, max compression
+gzip compressed data, was "sdl-webui-lite-0.1.2.tar", last modified: Thu May 23 21:04:16 2024, max compression
```

## Comparing `sdl-webui-lite-0.1.1.tar` & `sdl-webui-lite-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.710336 sdl-webui-lite-0.1.1/
--rw-rw-rw-   0        0        0     1100 2024-05-22 22:37:29.000000 sdl-webui-lite-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       83 2024-05-23 19:58:53.000000 sdl-webui-lite-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2024-05-23 20:45:25.708992 sdl-webui-lite-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1687 2024-05-23 20:10:07.000000 sdl-webui-lite-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.695323 sdl-webui-lite-0.1.1/sdl_webui_lite/
--rw-rw-rw-   0        0        0        0 2024-05-23 20:09:54.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/__init__.py
--rw-rw-rw-   0        0        0     3169 2024-05-23 19:29:44.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/app.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.702249 sdl-webui-lite-0.1.1/sdl_webui_lite/static/
--rw-rw-rw-   0        0        0     1150 2024-02-15 19:57:46.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/static/favicon.ico
--rw-rw-rw-   0        0        0    63464 2024-05-21 22:31:17.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/static/logo.png
--rw-rw-rw-   0        0        0    41343 2024-05-23 19:22:39.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/static/page_screenshot.png
--rw-rw-rw-   0        0        0     2050 2024-05-22 19:54:05.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/static/style.css
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.705479 sdl-webui-lite-0.1.1/sdl_webui_lite/templates/
--rw-rw-rw-   0        0        0     3643 2024-05-22 19:51:12.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/templates/base.html
--rw-rw-rw-   0        0        0     5356 2024-05-22 21:50:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/templates/experiment.html
--rw-rw-rw-   0        0        0      146 2024-05-22 20:19:12.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/templates/home.html
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.707779 sdl-webui-lite-0.1.1/sdl_webui_lite/utils/
--rw-rw-rw-   0        0        0        0 2024-05-22 21:02:04.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/utils/__init__.py
--rw-rw-rw-   0        0        0     2596 2024-05-22 22:28:15.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/utils/scheduler.py
--rw-rw-rw-   0        0        0     5059 2024-05-22 20:19:12.000000 sdl-webui-lite-0.1.1/sdl_webui_lite/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:45:25.698767 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/
--rw-rw-rw-   0        0        0     2107 2024-05-23 20:45:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2024-05-23 20:45:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:45:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 20:45:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 20:45:25.000000 sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 20:45:25.710336 sdl-webui-lite-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-05-23 20:39:11.000000 sdl-webui-lite-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.843305 sdl-webui-lite-0.1.2/
+-rw-rw-rw-   0        0        0     1100 2024-05-22 22:37:29.000000 sdl-webui-lite-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       83 2024-05-23 19:58:53.000000 sdl-webui-lite-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2031 2024-05-23 21:04:16.841806 sdl-webui-lite-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1611 2024-05-23 20:58:17.000000 sdl-webui-lite-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.824305 sdl-webui-lite-0.1.2/sdl_webui_lite/
+-rw-rw-rw-   0        0        0        0 2024-05-23 20:09:54.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/__init__.py
+-rw-rw-rw-   0        0        0     3169 2024-05-23 19:29:44.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/app.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.833305 sdl-webui-lite-0.1.2/sdl_webui_lite/static/
+-rw-rw-rw-   0        0        0     1150 2024-02-15 19:57:46.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/static/favicon.ico
+-rw-rw-rw-   0        0        0    63464 2024-05-21 22:31:17.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/static/logo.png
+-rw-rw-rw-   0        0        0    41343 2024-05-23 19:22:39.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/static/page_screenshot.png
+-rw-rw-rw-   0        0        0     2050 2024-05-22 19:54:05.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/static/style.css
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.836806 sdl-webui-lite-0.1.2/sdl_webui_lite/templates/
+-rw-rw-rw-   0        0        0     3643 2024-05-22 19:51:12.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/templates/base.html
+-rw-rw-rw-   0        0        0     5356 2024-05-22 21:50:25.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/templates/experiment.html
+-rw-rw-rw-   0        0        0      146 2024-05-22 20:19:12.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/templates/home.html
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.840306 sdl-webui-lite-0.1.2/sdl_webui_lite/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-22 21:02:04.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/utils/__init__.py
+-rw-rw-rw-   0        0        0     2596 2024-05-22 22:28:15.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/utils/scheduler.py
+-rw-rw-rw-   0        0        0     5059 2024-05-22 20:19:12.000000 sdl-webui-lite-0.1.2/sdl_webui_lite/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:04:16.828804 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/
+-rw-rw-rw-   0        0        0     2031 2024-05-23 21:04:16.000000 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2024-05-23 21:04:16.000000 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:04:16.000000 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 21:04:16.000000 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 21:04:16.000000 sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:04:16.843305 sdl-webui-lite-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-05-23 21:04:14.000000 sdl-webui-lite-0.1.2/setup.py
```

### Comparing `sdl-webui-lite-0.1.1/LICENSE` & `sdl-webui-lite-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/PKG-INFO` & `sdl-webui-lite-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: sdl-webui-lite
-Version: 0.1.1
+Version: 0.1.2
 Summary: This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically.
 Home-page: https://gitlab.com/heingroup/sdl_webui_lite
 Author: Ivory Zhang
 Author-email: ivoryzhang@chem.ubc.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask-SocketIO
 
 # Self-driving lab Web UI - lite
-We don't define Self-driving labs (SDLs). We enable UI for them. This is the lite version of [SDL Web UI](https://gitlab.com/heingroup/web_controller)
+We don't define Self-driving labs (SDLs). We enable UI for them. 
+This is the lite version of Hein Lab [SDL Web UI](https://gitlab.com/heingroup/web_controller)
 
 ## Description
 
 
 Granting SDL flexibility makes it impossible to design a UI, yet it's a necessity for allowing more people to interact with it. 
-This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically. 
+This web UI aims to ease up the control of any Python-based SDLs by displaying functions and parameters dynamically. 
 This lite version allow user to put actions in queue for simply workflow design. 
 
 ## Installation
 ```
-git clone https://gitlab.com/heingroup/sdl-webui-lite.git
-pip install -r .\sdl_webui_lite\requirements.txt
+pip install sdl-webui-lite
 ```
 
 ## Usage
 in your self-driving platform class, use `start_gui(your_sdl)`. Example in [sample_code.py](sample_code.py)
 ```python
 sdl = YourSDL()
 from sdl_webui_lite.app import start_gui
```

### Comparing `sdl-webui-lite-0.1.1/README.md` & `sdl-webui-lite-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Self-driving lab Web UI - lite
-We don't define Self-driving labs (SDLs). We enable UI for them. This is the lite version of [SDL Web UI](https://gitlab.com/heingroup/web_controller)
+We don't define Self-driving labs (SDLs). We enable UI for them. 
+This is the lite version of Hein Lab [SDL Web UI](https://gitlab.com/heingroup/web_controller)
 
 ## Description
 
 
 Granting SDL flexibility makes it impossible to design a UI, yet it's a necessity for allowing more people to interact with it. 
-This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically. 
+This web UI aims to ease up the control of any Python-based SDLs by displaying functions and parameters dynamically. 
 This lite version allow user to put actions in queue for simply workflow design. 
 
 ## Installation
 ```
-git clone https://gitlab.com/heingroup/sdl-webui-lite.git
-pip install -r .\sdl_webui_lite\requirements.txt
+pip install sdl-webui-lite
 ```
 
 ## Usage
 in your self-driving platform class, use `start_gui(your_sdl)`. Example in [sample_code.py](sample_code.py)
 ```python
 sdl = YourSDL()
 from sdl_webui_lite.app import start_gui
```

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/app.py` & `sdl-webui-lite-0.1.2/sdl_webui_lite/app.py`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/static/favicon.ico` & `sdl-webui-lite-0.1.2/sdl_webui_lite/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/static/logo.png` & `sdl-webui-lite-0.1.2/sdl_webui_lite/static/logo.png`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/static/page_screenshot.png` & `sdl-webui-lite-0.1.2/sdl_webui_lite/static/page_screenshot.png`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/static/style.css` & `sdl-webui-lite-0.1.2/sdl_webui_lite/static/style.css`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/templates/base.html` & `sdl-webui-lite-0.1.2/sdl_webui_lite/templates/base.html`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/templates/experiment.html` & `sdl-webui-lite-0.1.2/sdl_webui_lite/templates/experiment.html`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/utils/scheduler.py` & `sdl-webui-lite-0.1.2/sdl_webui_lite/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite/utils/utils.py` & `sdl-webui-lite-0.1.2/sdl_webui_lite/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/PKG-INFO` & `sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: sdl-webui-lite
-Version: 0.1.1
+Version: 0.1.2
 Summary: This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically.
 Home-page: https://gitlab.com/heingroup/sdl_webui_lite
 Author: Ivory Zhang
 Author-email: ivoryzhang@chem.ubc.ca
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask-SocketIO
 
 # Self-driving lab Web UI - lite
-We don't define Self-driving labs (SDLs). We enable UI for them. This is the lite version of [SDL Web UI](https://gitlab.com/heingroup/web_controller)
+We don't define Self-driving labs (SDLs). We enable UI for them. 
+This is the lite version of Hein Lab [SDL Web UI](https://gitlab.com/heingroup/web_controller)
 
 ## Description
 
 
 Granting SDL flexibility makes it impossible to design a UI, yet it's a necessity for allowing more people to interact with it. 
-This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically. 
+This web UI aims to ease up the control of any Python-based SDLs by displaying functions and parameters dynamically. 
 This lite version allow user to put actions in queue for simply workflow design. 
 
 ## Installation
 ```
-git clone https://gitlab.com/heingroup/sdl-webui-lite.git
-pip install -r .\sdl_webui_lite\requirements.txt
+pip install sdl-webui-lite
 ```
 
 ## Usage
 in your self-driving platform class, use `start_gui(your_sdl)`. Example in [sample_code.py](sample_code.py)
 ```python
 sdl = YourSDL()
 from sdl_webui_lite.app import start_gui
```

### Comparing `sdl-webui-lite-0.1.1/sdl_webui_lite.egg-info/SOURCES.txt` & `sdl-webui-lite-0.1.2/sdl_webui_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdl-webui-lite-0.1.1/setup.py` & `sdl-webui-lite-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sdl-webui-lite',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     description='This web UI aims to ease up the control of any Python-based SDLs by displaying functions and their parameters dynamically.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ivory Zhang',
     author_email='ivoryzhang@chem.ubc.ca',
```

