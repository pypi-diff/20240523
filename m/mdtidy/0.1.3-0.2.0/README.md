# Comparing `tmp/mdtidy-0.1.3.tar.gz` & `tmp/mdtidy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdtidy-0.1.3.tar", last modified: Wed May 22 22:12:59 2024, max compression
+gzip compressed data, was "mdtidy-0.2.0.tar", last modified: Wed May 22 22:33:01 2024, max compression
```

## Comparing `mdtidy-0.1.3.tar` & `mdtidy-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 22:12:59.144988 mdtidy-0.1.3/
--rw-rw-rw-   0        0        0     1070 2024-05-22 09:22:50.000000 mdtidy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3125 2024-05-22 22:12:59.141967 mdtidy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2590 2024-05-22 09:22:49.000000 mdtidy-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 22:12:59.100009 mdtidy-0.1.3/mdtidy/
--rw-rw-rw-   0        0        0        0 2024-05-22 07:42:02.000000 mdtidy-0.1.3/mdtidy/__init__.py
--rw-rw-rw-   0        0        0     4208 2024-05-22 22:12:07.000000 mdtidy-0.1.3/mdtidy/cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-22 22:12:59.137966 mdtidy-0.1.3/mdtidy.egg-info/
--rw-rw-rw-   0        0        0     3125 2024-05-22 22:12:58.000000 mdtidy-0.1.3/mdtidy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-22 22:12:58.000000 mdtidy-0.1.3/mdtidy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 22:12:58.000000 mdtidy-0.1.3/mdtidy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 22:12:58.000000 mdtidy-0.1.3/mdtidy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 22:12:59.144988 mdtidy-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      676 2024-05-22 22:12:38.000000 mdtidy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:33:01.911166 mdtidy-0.2.0/
+-rw-rw-rw-   0        0        0     1070 2024-05-22 09:22:50.000000 mdtidy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3125 2024-05-22 22:33:01.904168 mdtidy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2590 2024-05-22 09:22:49.000000 mdtidy-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 22:33:01.874178 mdtidy-0.2.0/mdtidy/
+-rw-rw-rw-   0        0        0        0 2024-05-22 07:42:02.000000 mdtidy-0.2.0/mdtidy/__init__.py
+-rw-rw-rw-   0        0        0     3813 2024-05-22 22:29:34.000000 mdtidy-0.2.0/mdtidy/cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:33:01.902173 mdtidy-0.2.0/mdtidy.egg-info/
+-rw-rw-rw-   0        0        0     3125 2024-05-22 22:33:01.000000 mdtidy-0.2.0/mdtidy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-22 22:33:01.000000 mdtidy-0.2.0/mdtidy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:33:01.000000 mdtidy-0.2.0/mdtidy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 22:33:01.000000 mdtidy-0.2.0/mdtidy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:33:01.912163 mdtidy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      676 2024-05-22 22:32:12.000000 mdtidy-0.2.0/setup.py
```

### Comparing `mdtidy-0.1.3/LICENSE` & `mdtidy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdtidy-0.1.3/PKG-INFO` & `mdtidy-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdtidy
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python library to clean and format markdown content into Jupyter Notebooks.
 Home-page: https://github.com/davidkjeremiah/mdtidy
 Author: David Jeremiah
 Author-email: flasconnect@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mdtidy-0.1.3/README.md` & `mdtidy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mdtidy-0.1.3/mdtidy/cleaner.py` & `mdtidy-0.2.0/mdtidy/cleaner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 import re
 import json
 
 def process_content_to_ipynb(input_string, output_filename):
     # Remove text blocks enclosed with triple backticks that start with ```text?code_stdout or ```text?code_stderr
-    cleaned_content = re.sub(r'```text\?code_stdout.*?\n.*?\n```', '', input_string, flags=re.DOTALL)
-    cleaned_content = re.sub(r'```text\?code_stderr.*?\n.*?\n```', '', cleaned_content, flags=re.DOTALL)
+    cleaned_content = re.sub(r'```text\?code_(stdout|stderr).*?\n.*?\n```', '', input_string, flags=re.DOTALL)
 
     # Extract code blocks
     code_blocks = re.findall(r'```python\?code.*?\n(.*?)\n```', cleaned_content, flags=re.DOTALL)
 
     # Remove code block markers but keep the actual code for separate handling
     cleaned_content = re.sub(r'```python\?code.*?\n', 'CODE_BLOCK_START\n', cleaned_content)
     cleaned_content = re.sub(r'\n```', '\nCODE_BLOCK_END', cleaned_content)
 
     # Split the content by the markers
     split_content = cleaned_content.split('\n')
 
     # Initialize the notebook cells
     cells = []
     code_block_index = 0
+    markdown_content = []
 
     # Process the split content to organize text and code blocks
-    inside_code_block = False
-    markdown_content = ""
     for line in split_content:
         if line == "CODE_BLOCK_START":
-            if markdown_content.strip():
+            if markdown_content:
                 cells.append({
                     "cell_type": "markdown",
                     "metadata": {},
-                    "source": [line + '\n' for line in markdown_content.strip().split('\n')]
+                    "source": [line + '\n' for line in markdown_content]
                 })
-                markdown_content = ""
-            inside_code_block = True
-            code_content = ""
+                markdown_content = []
         elif line == "CODE_BLOCK_END":
-            inside_code_block = False
             if code_block_index < len(code_blocks):
                 code_content = code_blocks[code_block_index]
                 cells.append({
                     "cell_type": "code",
                     "execution_count": None,
                     "metadata": {},
                     "outputs": [],
                     "source": [line + '\n' for line in code_content.strip().split('\n')]
                 })
                 code_block_index += 1
         else:
-            if inside_code_block:
-                code_content += line + "\n"
-            else:
-                markdown_content += line + "\n"
+            markdown_content.append(line)
 
-    if markdown_content.strip():
+    if markdown_content:
         cells.append({
             "cell_type": "markdown",
             "metadata": {},
-            "source": [line + '\n' for line in markdown_content.strip().split('\n')]
+            "source": [line + '\n' for line in markdown_content]
         })
 
     # Create the notebook structure
     notebook_content = {
         "cells": cells,
         "metadata": {
             "kernelspec": {
@@ -105,8 +97,8 @@
     
     # Count the occurrences of each error type within the tracebacks
     for traceback in tracebacks:
         for error in error_types:
             if f"{error}:" in traceback:
                 error_counts[error] += 1
 
-    return error_counts
+    return error_counts
```

### Comparing `mdtidy-0.1.3/mdtidy.egg-info/PKG-INFO` & `mdtidy-0.2.0/mdtidy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdtidy
-Version: 0.1.3
+Version: 0.2.0
 Summary: A Python library to clean and format markdown content into Jupyter Notebooks.
 Home-page: https://github.com/davidkjeremiah/mdtidy
 Author: David Jeremiah
 Author-email: flasconnect@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mdtidy-0.1.3/setup.py` & `mdtidy-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mdtidy',
-    version='0.1.3',
+    version='0.2.0',
     description='A Python library to clean and format markdown content into Jupyter Notebooks.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='David Jeremiah',
     author_email='flasconnect@gmail.com',
     url='https://github.com/davidkjeremiah/mdtidy',
     license='MIT',
```

