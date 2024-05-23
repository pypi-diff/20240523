# Comparing `tmp/aicelltype-0.0.5.tar.gz` & `tmp/aicelltype-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicelltype-0.0.5.tar", last modified: Wed May 15 03:07:34 2024, max compression
+gzip compressed data, was "aicelltype-0.0.6.tar", last modified: Thu May 23 09:49:26 2024, max compression
```

## Comparing `aicelltype-0.0.5.tar` & `aicelltype-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:07:34.455223 aicelltype-0.0.5/
--rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.5/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3608 2024-05-15 03:07:34.454222 aicelltype-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3128 2024-05-14 07:50:19.000000 aicelltype-0.0.5/README.md
--rw-rw-rw-   0        0        0      575 2024-05-15 03:05:18.000000 aicelltype-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 03:07:34.456221 aicelltype-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 03:07:34.424564 aicelltype-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 03:07:34.425564 aicelltype-0.0.5/src/AICelltype/
--rw-rw-rw-   0        0        0     7770 2024-05-15 03:06:47.000000 aicelltype-0.0.5/src/AICelltype/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 03:07:34.453221 aicelltype-0.0.5/src/AICelltype.egg-info/
--rw-rw-rw-   0        0        0     3608 2024-05-15 03:07:34.000000 aicelltype-0.0.5/src/AICelltype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-05-15 03:07:34.000000 aicelltype-0.0.5/src/AICelltype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:07:34.000000 aicelltype-0.0.5/src/AICelltype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-15 03:07:34.000000 aicelltype-0.0.5/src/AICelltype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-15 03:07:34.000000 aicelltype-0.0.5/src/AICelltype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:49:26.821114 aicelltype-0.0.6/
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:10:46.000000 aicelltype-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-02-03 13:12:25.000000 aicelltype-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3608 2024-05-23 09:49:26.819114 aicelltype-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3128 2024-05-14 07:50:19.000000 aicelltype-0.0.6/README.md
+-rw-rw-rw-   0        0        0      575 2024-05-23 09:46:29.000000 aicelltype-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:49:26.821114 aicelltype-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 09:49:26.790113 aicelltype-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:49:26.791113 aicelltype-0.0.6/src/AICelltype/
+-rw-rw-rw-   0        0        0     7766 2024-05-23 09:46:29.000000 aicelltype-0.0.6/src/AICelltype/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:49:26.818113 aicelltype-0.0.6/src/AICelltype.egg-info/
+-rw-rw-rw-   0        0        0     3608 2024-05-23 09:49:26.000000 aicelltype-0.0.6/src/AICelltype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-05-23 09:49:26.000000 aicelltype-0.0.6/src/AICelltype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:49:26.000000 aicelltype-0.0.6/src/AICelltype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-23 09:49:26.000000 aicelltype-0.0.6/src/AICelltype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 09:49:26.000000 aicelltype-0.0.6/src/AICelltype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      490 2024-02-03 13:12:00.000000 aicelltype-0.0.6/src/__init__.py
```

### Comparing `aicelltype-0.0.5/PKG-INFO` & `aicelltype-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.5
+Version: 0.0.6
 Summary: AICelltype: Annotate cell type through gpt-4 without openai key.
 Author-email: renzhg <rzgedu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
```

### Comparing `aicelltype-0.0.5/README.md` & `aicelltype-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aicelltype-0.0.5/pyproject.toml` & `aicelltype-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "AICelltype"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name = "renzhg", email = "rzgedu@163.com" },
 ]
 dependencies = ['dashscope==1.17.1', 'requests==2.31.0']
 description = "AICelltype: Annotate cell type through gpt-4 without openai key."
 readme = "README.md"
 requires-python = ">=3.10.0"
```

### Comparing `aicelltype-0.0.5/src/AICelltype/__init__.py` & `aicelltype-0.0.6/src/AICelltype/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     usage3:
         # ERNIE-4.0 model
         import os
         os.environ['API_KEY'] = 'your AIP_KEY'  # Add API_KEY to environ, keep secret to yourself.
         os.environ['SECRET_KEY'] = 'your SECRET_KEY'  # Add SECRET_KEY to environ, keep secret to yourself.
 
         from AICelltype import aicelltype
-        cell_lt = aicelltype(tissue_name, gene_lt, model='qwen-max')
+        cell_lt = aicelltype(tissue_name, gene_lt, model='ERNIE-4.0')
         print(cell_lt)
     output3:
         ['Prostate glandular cells (or Prostate epithelial cells)', 'Lymphatic endothelial cells', 'T-cells (or T-lymphocytes)', 'Unknown cell type (or Possibly cancer-associated cells or Stromal cells; needs further investigation)']  # This model give more explaination.
     """
     if model == 'gpt4':
         cell_lt = gpt4(tissue_name, gene_list)
     elif model == 'qwen-max':
@@ -113,15 +113,15 @@
 
 
 def qwen(tissue_name, gene_list):
     gene_str = '\n'.join([','.join(i) for i in gene_list])
     input_msg = f'Identify cell types of {tissue_name} cells using the following markers. Identify one cell type for each row. Only provide the cell type name and nothing else without number before the output. Some could be a mixture of multiple cell types. Some could be unknown cell types.\n{gene_str}'
     # print(input_msg)
     messages = [{'role': 'user', 'content': input_msg}]
-    response = Generation.call("qwen-max-0403",
+    response = Generation.call("qwen-max",
                                messages=messages,
                                result_format='message',
                               )
     if response.status_code == HTTPStatus.OK:
         # print(response)
         cellstr= response['output']['choices'][0]['message']['content']
         cell_lt = cellstr.split('\n')
```

### Comparing `aicelltype-0.0.5/src/AICelltype.egg-info/PKG-INFO` & `aicelltype-0.0.6/src/AICelltype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICelltype
-Version: 0.0.5
+Version: 0.0.6
 Summary: AICelltype: Annotate cell type through gpt-4 without openai key.
 Author-email: renzhg <rzgedu@163.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
```

