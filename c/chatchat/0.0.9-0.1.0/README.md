# Comparing `tmp/chatchat-0.0.9.tar.gz` & `tmp/chatchat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.9.tar", last modified: Wed May 22 14:16:59 2024, max compression
+gzip compressed data, was "chatchat-0.1.0.tar", last modified: Wed May 22 23:33:33 2024, max compression
```

## Comparing `chatchat-0.0.9.tar` & `chatchat-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.964593 chatchat-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 14:16:55.000000 chatchat-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:16:59.964593 chatchat-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:55.000000 chatchat-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.960593 chatchat-0.0.9/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.964593 chatchat-0.0.9/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:16:59.964593 chatchat-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 14:16:55.000000 chatchat-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:33:33.617401 chatchat-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 23:33:27.000000 chatchat-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 23:33:33.617401 chatchat-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:33:27.000000 chatchat-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:33:33.617401 chatchat-0.1.0/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:33:27.000000 chatchat-0.1.0/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-22 23:33:27.000000 chatchat-0.1.0/chatchat/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 23:33:27.000000 chatchat-0.1.0/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 23:33:27.000000 chatchat-0.1.0/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-22 23:33:27.000000 chatchat-0.1.0/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:33:33.617401 chatchat-0.1.0/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 23:33:33.000000 chatchat-0.1.0/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 23:33:33.000000 chatchat-0.1.0/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:33:33.000000 chatchat-0.1.0/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:33:33.000000 chatchat-0.1.0/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 23:33:33.000000 chatchat-0.1.0/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:33:33.617401 chatchat-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 23:33:27.000000 chatchat-0.1.0/setup.py
```

### Comparing `chatchat-0.0.9/LICENSE` & `chatchat-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.9/PKG-INFO` & `chatchat-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.9
+Version: 0.1.0
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.9/chatchat/alibaba.py` & `chatchat-0.1.0/chatchat/alibaba.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,8 +45,17 @@
 
 class Chat(Completion):
     def __init__(self, jfile, model='qwen-turbo', history=[]):
         super().__init__(jfile, model=model)
         self.history = history
 
     def chat(self, message):
-        ...
+        self.history.append({
+            'role': 'user',
+            'content': message,
+        })
+
+        r = self.send_message(self.history)
+        assistant_output = r['output']['choices'][0]['message']
+        self.history.append(assistant_output)
+
+        return r
```

### Comparing `chatchat-0.0.9/chatchat/baidu.py` & `chatchat-0.1.0/chatchat/baidu.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.9/chatchat/xunfei.py` & `chatchat-0.1.0/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.9/chatchat.egg-info/PKG-INFO` & `chatchat-0.1.0/chatchat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.9
+Version: 0.1.0
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.9/setup.py` & `chatchat-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.9',
+    version = '0.1.0',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

