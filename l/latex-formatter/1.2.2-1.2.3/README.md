# Comparing `tmp/latex_formatter-1.2.2.tar.gz` & `tmp/latex_formatter-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_formatter-1.2.2.tar", last modified: Thu May 23 06:38:38 2024, max compression
+gzip compressed data, was "latex_formatter-1.2.3.tar", last modified: Thu May 23 06:51:21 2024, max compression
```

## Comparing `latex_formatter-1.2.2.tar` & `latex_formatter-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.563888 latex_formatter-1.2.2/
--rw-rw-rw-   0        0        0       62 2024-05-23 06:38:38.561890 latex_formatter-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-11-17 10:14:19.000000 latex_formatter-1.2.2/README.md
--rw-rw-rw-   0        0        0       52 2023-10-17 03:55:42.000000 latex_formatter-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 06:38:38.563888 latex_formatter-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      318 2024-05-23 06:38:34.000000 latex_formatter-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.510004 latex_formatter-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.516680 latex_formatter-1.2.2/src/latex_formatter/
--rw-rw-rw-   0        0        0      103 2023-12-21 06:45:34.000000 latex_formatter-1.2.2/src/latex_formatter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.552668 latex_formatter-1.2.2/src/latex_formatter/converter/
--rw-rw-rw-   0        0        0       62 2023-12-21 06:45:01.000000 latex_formatter-1.2.2/src/latex_formatter/converter/__init__.py
--rw-rw-rw-   0        0        0    16202 2024-05-22 02:43:32.000000 latex_formatter-1.2.2/src/latex_formatter/converter/converter.py
--rw-rw-rw-   0        0        0    28904 2024-05-23 06:25:35.000000 latex_formatter-1.2.2/src/latex_formatter/converter/web_converter.py
--rw-rw-rw-   0        0        0       71 2023-10-17 07:08:30.000000 latex_formatter-1.2.2/src/latex_formatter/test.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.558883 latex_formatter-1.2.2/src/latex_formatter/utils/
--rw-rw-rw-   0        0        0       87 2023-10-17 07:21:19.000000 latex_formatter-1.2.2/src/latex_formatter/utils/__init__.py
--rw-rw-rw-   0        0        0    20221 2023-11-15 07:06:02.000000 latex_formatter-1.2.2/src/latex_formatter/utils/text_to_latex.py
--rw-rw-rw-   0        0        0      233 2023-11-16 06:42:03.000000 latex_formatter-1.2.2/src/latex_formatter/utils/transfer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:38:38.545670 latex_formatter-1.2.2/src/latex_formatter.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-23 06:38:38.000000 latex_formatter-1.2.2/src/latex_formatter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2024-05-23 06:38:38.000000 latex_formatter-1.2.2/src/latex_formatter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:38:38.000000 latex_formatter-1.2.2/src/latex_formatter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-23 06:38:38.000000 latex_formatter-1.2.2/src/latex_formatter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 06:38:38.000000 latex_formatter-1.2.2/src/latex_formatter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.075698 latex_formatter-1.2.3/
+-rw-rw-rw-   0        0        0       62 2024-05-23 06:51:21.074690 latex_formatter-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-11-17 10:14:19.000000 latex_formatter-1.2.3/README.md
+-rw-rw-rw-   0        0        0       52 2023-10-17 03:55:42.000000 latex_formatter-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:51:21.076475 latex_formatter-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      318 2024-05-23 06:49:12.000000 latex_formatter-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.009534 latex_formatter-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.027124 latex_formatter-1.2.3/src/latex_formatter/
+-rw-rw-rw-   0        0        0      103 2023-12-21 06:45:34.000000 latex_formatter-1.2.3/src/latex_formatter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.060640 latex_formatter-1.2.3/src/latex_formatter/converter/
+-rw-rw-rw-   0        0        0       62 2023-12-21 06:45:01.000000 latex_formatter-1.2.3/src/latex_formatter/converter/__init__.py
+-rw-rw-rw-   0        0        0    16162 2024-05-23 06:41:47.000000 latex_formatter-1.2.3/src/latex_formatter/converter/converter.py
+-rw-rw-rw-   0        0        0    28904 2024-05-23 06:25:35.000000 latex_formatter-1.2.3/src/latex_formatter/converter/web_converter.py
+-rw-rw-rw-   0        0        0       71 2023-10-17 07:08:30.000000 latex_formatter-1.2.3/src/latex_formatter/test.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.060640 latex_formatter-1.2.3/src/latex_formatter/utils/
+-rw-rw-rw-   0        0        0       87 2023-10-17 07:21:19.000000 latex_formatter-1.2.3/src/latex_formatter/utils/__init__.py
+-rw-rw-rw-   0        0        0    20221 2023-11-15 07:06:02.000000 latex_formatter-1.2.3/src/latex_formatter/utils/text_to_latex.py
+-rw-rw-rw-   0        0        0      233 2023-11-16 06:42:03.000000 latex_formatter-1.2.3/src/latex_formatter/utils/transfer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:21.043527 latex_formatter-1.2.3/src/latex_formatter.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-23 06:51:20.000000 latex_formatter-1.2.3/src/latex_formatter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2024-05-23 06:51:20.000000 latex_formatter-1.2.3/src/latex_formatter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:51:20.000000 latex_formatter-1.2.3/src/latex_formatter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 06:51:20.000000 latex_formatter-1.2.3/src/latex_formatter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 06:51:20.000000 latex_formatter-1.2.3/src/latex_formatter.egg-info/top_level.txt
```

### Comparing `latex_formatter-1.2.2/src/latex_formatter/converter/converter.py` & `latex_formatter-1.2.3/src/latex_formatter/converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,26 +344,26 @@
             for key, value in caption.items():
                 if isinstance(value, dict) and "index" in value and "type" in value:
                     index.append(value)
                 elif isinstance(value, (dict, list)):
                     temp = get_answer_index(value)
                     if temp:
                         index.extend(temp)
-        return index if index else False
+        return index
 
     elif isinstance(caption, list):
         index = []
         for item in caption:
             if isinstance(item, dict) and "index" in item and "type" in item:
                 index.append(item)
             elif isinstance(item, (dict, list)):
                 temp = get_answer_index(item)
                 if temp:
                     index.extend(temp)
-        return index if index else False
+        return index
 
 
 def ttl_question_show_answer(question, q_type=1, mode=0):
     if question["type"] != 4:
         return False
 
     splits = split_question(
```

### Comparing `latex_formatter-1.2.2/src/latex_formatter/converter/web_converter.py` & `latex_formatter-1.2.3/src/latex_formatter/converter/web_converter.py`

 * *Files identical despite different names*

### Comparing `latex_formatter-1.2.2/src/latex_formatter/utils/text_to_latex.py` & `latex_formatter-1.2.3/src/latex_formatter/utils/text_to_latex.py`

 * *Files identical despite different names*

### Comparing `latex_formatter-1.2.2/src/latex_formatter.egg-info/SOURCES.txt` & `latex_formatter-1.2.3/src/latex_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

