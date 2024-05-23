# Comparing `tmp/markdown_text_clean-1.0.0.tar.gz` & `tmp/markdown_text_clean-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_text_clean-1.0.0.tar", last modified: Thu May 23 02:38:23 2024, max compression
+gzip compressed data, was "markdown_text_clean-1.0.1.tar", last modified: Thu May 23 02:40:59 2024, max compression
```

## Comparing `markdown_text_clean-1.0.0.tar` & `markdown_text_clean-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:38:23.561260 markdown_text_clean-1.0.0/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     2277 2024-05-23 02:38:23.560923 markdown_text_clean-1.0.0/PKG-INFO
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     1752 2024-05-23 02:33:36.000000 markdown_text_clean-1.0.0/README.md
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:38:23.541128 markdown_text_clean-1.0.0/markdown_text_clean/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       34 2024-05-22 15:41:03.000000 markdown_text_clean-1.0.0/markdown_text_clean/__init__.py
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      540 2024-05-22 15:40:51.000000 markdown_text_clean-1.0.0/markdown_text_clean/text_clean.py
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:38:23.560282 markdown_text_clean-1.0.0/markdown_text_clean.egg-info/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     2277 2024-05-23 02:38:23.000000 markdown_text_clean-1.0.0/markdown_text_clean.egg-info/PKG-INFO
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      256 2024-05-23 02:38:23.000000 markdown_text_clean-1.0.0/markdown_text_clean.egg-info/SOURCES.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)        1 2024-05-23 02:38:23.000000 markdown_text_clean-1.0.0/markdown_text_clean.egg-info/dependency_links.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       20 2024-05-23 02:38:23.000000 markdown_text_clean-1.0.0/markdown_text_clean.egg-info/top_level.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       38 2024-05-23 02:38:23.561365 markdown_text_clean-1.0.0/setup.cfg
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      537 2024-05-23 02:33:59.000000 markdown_text_clean-1.0.0/setup.py
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:40:59.701770 markdown_text_clean-1.0.1/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     2237 2024-05-23 02:40:59.701555 markdown_text_clean-1.0.1/PKG-INFO
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     1712 2024-05-23 02:40:31.000000 markdown_text_clean-1.0.1/README.md
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:40:59.698279 markdown_text_clean-1.0.1/markdown_text_clean/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       34 2024-05-22 15:41:03.000000 markdown_text_clean-1.0.1/markdown_text_clean/__init__.py
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      540 2024-05-22 15:40:51.000000 markdown_text_clean-1.0.1/markdown_text_clean/text_clean.py
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 02:40:59.701195 markdown_text_clean-1.0.1/markdown_text_clean.egg-info/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     2237 2024-05-23 02:40:59.000000 markdown_text_clean-1.0.1/markdown_text_clean.egg-info/PKG-INFO
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      256 2024-05-23 02:40:59.000000 markdown_text_clean-1.0.1/markdown_text_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)        1 2024-05-23 02:40:59.000000 markdown_text_clean-1.0.1/markdown_text_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       20 2024-05-23 02:40:59.000000 markdown_text_clean-1.0.1/markdown_text_clean.egg-info/top_level.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       38 2024-05-23 02:40:59.701852 markdown_text_clean-1.0.1/setup.cfg
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      537 2024-05-23 02:40:56.000000 markdown_text_clean-1.0.1/setup.py
```

### Comparing `markdown_text_clean-1.0.0/PKG-INFO` & `markdown_text_clean-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: markdown_text_clean
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to clean markdown text
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # 概要 (Overview)
         
         markdown-text-clean is a Python library that cleans up text by removing Markdown formatting such as bold, italic, inline code, and strikethrough.
         
         markdown-text-cleanは、太字、斜体、インラインコード、取り消し線などのマークダウン書式を削除してテキストをきれいにするPythonライブラリです。
         
         
         ## インストール (Installation)
         
         ```bash
-        pip install -i https://test.pypi.org/simple/ markdown-text-clean==0.8.5
+        pip install markdown-text-clean
         ```
         
         ## 使用方法 (Usage)
         
         
         This library takes copied Markdown-formatted text and removes Markdown symbols (e.g., `###`, `**`) to convert it into a more readable document format. You can use this function to convert copied Markdown-formatted text to document format. For example:
```

### Comparing `markdown_text_clean-1.0.0/README.md` & `markdown_text_clean-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 markdown-text-cleanは、太字、斜体、インラインコード、取り消し線などのマークダウン書式を削除してテキストをきれいにするPythonライブラリです。
 
 
 ## インストール (Installation)
 
 ```bash
-pip install -i https://test.pypi.org/simple/ markdown-text-clean==0.8.5
+pip install markdown-text-clean
 ```
 
 ## 使用方法 (Usage)
 
 
 This library takes copied Markdown-formatted text and removes Markdown symbols (e.g., `###`, `**`) to convert it into a more readable document format. You can use this function to convert copied Markdown-formatted text to document format. For example:
```

### Comparing `markdown_text_clean-1.0.0/markdown_text_clean/text_clean.py` & `markdown_text_clean-1.0.1/markdown_text_clean/text_clean.py`

 * *Files identical despite different names*

### Comparing `markdown_text_clean-1.0.0/markdown_text_clean.egg-info/PKG-INFO` & `markdown_text_clean-1.0.1/markdown_text_clean.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: markdown-text-clean
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to clean markdown text
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # 概要 (Overview)
         
         markdown-text-clean is a Python library that cleans up text by removing Markdown formatting such as bold, italic, inline code, and strikethrough.
         
         markdown-text-cleanは、太字、斜体、インラインコード、取り消し線などのマークダウン書式を削除してテキストをきれいにするPythonライブラリです。
         
         
         ## インストール (Installation)
         
         ```bash
-        pip install -i https://test.pypi.org/simple/ markdown-text-clean==0.8.5
+        pip install markdown-text-clean
         ```
         
         ## 使用方法 (Usage)
         
         
         This library takes copied Markdown-formatted text and removes Markdown symbols (e.g., `###`, `**`) to convert it into a more readable document format. You can use this function to convert copied Markdown-formatted text to document format. For example:
```

### Comparing `markdown_text_clean-1.0.0/setup.py` & `markdown_text_clean-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="markdown_text_clean",
-    version="1.0.0",
+    version="1.0.1",
     LICENSE = 'MIT',
     description="A package to clean markdown text",
     long_description=long_description,
     long_description_content_type="text/markdown", 
     packages=find_packages(),
     CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
```

