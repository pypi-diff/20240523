# Comparing `tmp/zeval-0.1.1.tar.gz` & `tmp/zeval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeval-0.1.1.tar", last modified: Tue May 21 08:54:33 2024, max compression
+gzip compressed data, was "zeval-0.1.2.tar", last modified: Thu May 23 08:16:10 2024, max compression
```

## Comparing `zeval-0.1.1.tar` & `zeval-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.409367 zeval-0.1.1/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-21 08:54:33.409211 zeval-0.1.1/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-21 08:54:33.409400 zeval-0.1.1/setup.cfg
--rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-21 08:53:46.000000 zeval-0.1.1/setup.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.407220 zeval-0.1.1/zeval/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.1/zeval/__init__.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.407843 zeval-0.1.1/zeval/config/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.1/zeval/config/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.1/zeval/config/model_config.py
--rw-r--r--   0 everfly    (501) wheel        (0)      492 2024-05-20 12:59:22.000000 zeval-0.1.1/zeval/evaluation.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408495 zeval-0.1.1/zeval/evaluators/
--rw-r--r--   0 everfly    (501) wheel        (0)      211 2024-05-10 10:53:55.000000 zeval-0.1.1/zeval/evaluators/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)     6929 2024-05-19 09:09:39.000000 zeval-0.1.1/zeval/evaluators/answer_relevancy.py
--rw-r--r--   0 everfly    (501) wheel        (0)     4327 2024-05-19 09:09:28.000000 zeval-0.1.1/zeval/evaluators/context_precision.py
--rw-r--r--   0 everfly    (501) wheel        (0)     8276 2024-05-19 09:09:17.000000 zeval-0.1.1/zeval/evaluators/context_recall.py
--rw-r--r--   0 everfly    (501) wheel        (0)     9640 2024-05-20 12:57:21.000000 zeval-0.1.1/zeval/evaluators/faithfulness.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408687 zeval-0.1.1/zeval/utils/
--rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.1/zeval/utils/__init__.py
--rw-r--r--   0 everfly    (501) wheel        (0)     1245 2024-05-19 07:31:36.000000 zeval-0.1.1/zeval/utils/model.py
-drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-21 08:54:33.408983 zeval-0.1.1/zeval.egg-info/
--rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) wheel        (0)        6 2024-05-21 08:54:33.000000 zeval-0.1.1/zeval.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680909 zeval-0.1.2/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-23 08:16:10.680729 zeval-0.1.2/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)       38 2024-05-23 08:16:10.680940 zeval-0.1.2/setup.cfg
+-rw-r--r--   0 everfly    (501) wheel        (0)      887 2024-05-23 08:14:56.000000 zeval-0.1.2/setup.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.678072 zeval-0.1.2/zeval/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:04:24.000000 zeval-0.1.2/zeval/__init__.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.678839 zeval-0.1.2/zeval/config/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:33.000000 zeval-0.1.2/zeval/config/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      180 2024-05-10 10:53:55.000000 zeval-0.1.2/zeval/config/model_config.py
+-rw-r--r--   0 everfly    (501) wheel        (0)      492 2024-05-20 12:59:22.000000 zeval-0.1.2/zeval/evaluation.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.679962 zeval-0.1.2/zeval/evaluators/
+-rw-r--r--   0 everfly    (501) wheel        (0)      211 2024-05-10 10:53:55.000000 zeval-0.1.2/zeval/evaluators/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     6948 2024-05-22 12:55:23.000000 zeval-0.1.2/zeval/evaluators/answer_relevancy.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     4210 2024-05-23 08:14:48.000000 zeval-0.1.2/zeval/evaluators/context_precision.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     8173 2024-05-22 13:01:41.000000 zeval-0.1.2/zeval/evaluators/context_recall.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     9640 2024-05-20 12:57:21.000000 zeval-0.1.2/zeval/evaluators/faithfulness.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680278 zeval-0.1.2/zeval/utils/
+-rw-r--r--   0 everfly    (501) wheel        (0)        0 2024-05-01 07:08:26.000000 zeval-0.1.2/zeval/utils/__init__.py
+-rw-r--r--   0 everfly    (501) wheel        (0)     1245 2024-05-19 07:31:36.000000 zeval-0.1.2/zeval/utils/model.py
+drwxr-xr-x   0 everfly    (501) wheel        (0)        0 2024-05-23 08:16:10.680535 zeval-0.1.2/zeval.egg-info/
+-rw-r--r--   0 everfly    (501) wheel        (0)      651 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) wheel        (0)      461 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        1 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)       25 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) wheel        (0)        6 2024-05-23 08:16:10.000000 zeval-0.1.2/zeval.egg-info/top_level.txt
```

### Comparing `zeval-0.1.1/PKG-INFO` & `zeval-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zeval-0.1.1/setup.py` & `zeval-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zeval',
-    version='0.1.1',
+    version='0.1.2',
     author='everfly',
     author_email='tagriver@gmail.com',
     description='A Python library for evaluating RAG outputs of Chinese large language models.',
     # long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourgithub/zeval',
     packages=find_packages(),
```

### Comparing `zeval-0.1.1/zeval/evaluators/answer_relevancy.py` & `zeval-0.1.2/zeval/evaluators/answer_relevancy.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,25 @@
         context = dataset["context"]
 
         question_prompt = self.get_prompt('QUESTION_TEMPLATE').format(answer=answer)
         if isinstance(question_prompt, str):
             messages = [{"role": "user", "content": question_prompt}]
 
         gen_question_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
-        gen_question = ModelCaller.parse_response(gen_question_response)
+        gen_question = ModelCaller.parse_response(self, gen_question_response)
         gen_question_response.elapsed_time = elapsed_time
         gen_question_response.prompt = json.dumps(question_prompt)
         gen_question_response.completion = gen_question
 
         correlation_prompt = self.get_prompt('CORRELATION_PROMPT_TEMPLATE').format(statement_one=question, statement_two=gen_question)
         if isinstance(correlation_prompt, str):
             messages = [{"role": "user", "content": correlation_prompt}]
 
         correlation_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
-        correlation_result = self.parse_response(correlation_response)
+        correlation_result = ModelCaller.parse_response(self, correlation_response)
         correlation_response.elapsed_time = elapsed_time
         correlation_response.prompt = json.dumps(correlation_prompt)
         correlation_response.completion = correlation_result
 
         result_score = self.extract_score(correlation_result)
 
         reasoning = self.get_prompt('REASONING_MESSAGE').format(answer=answer, gen_question=gen_question, question=question, result=result_score)
```

### Comparing `zeval-0.1.1/zeval/evaluators/context_precision.py` & `zeval-0.1.2/zeval/evaluators/context_precision.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,20 +83,16 @@
         determine_results = []
         for context in contexts:
             start_time = time.time()  # 开始计时
             determine_prompt = self.get_prompt('CONTEXT_PRECISION_TEMPLATE').format(question=question, context=context)
             if isinstance(determine_prompt, str):
                 messages = [{"role": "user", "content": determine_prompt}]
 
-            determine_response = ModelCaller.call(self, messages=messages, **sample_kwargs)
-            elapsed_time = time.time() - start_time  # 计算经过的时间
-
-            determine_result = ModelCaller.parse_response(determine_response)
-
-            print("determine_result: ", determine_result)
+            determine_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
+            determine_result = ModelCaller.parse_response(self, determine_response)
 
             determine_response.elapsed_time = elapsed_time
             determine_response.prompt = json.dumps(determine_prompt)
             determine_response.completion = determine_result
 
             determine_results.append("Yes" in determine_result)
             determine_responses.append(determine_response)
```

### Comparing `zeval-0.1.1/zeval/evaluators/context_recall.py` & `zeval-0.1.2/zeval/evaluators/context_recall.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,19 +104,16 @@
         # 使用 CONTEXT_RECALL_RA 模板
         prompt = self.get_prompt('CONTEXT_RECALL_RA').format(context=context, ideal=ideal)
 
         # 创建 PromptFn 实例
         if isinstance(prompt, str):
             messages = [{"role": "user", "content": prompt}]
 
-        start_time = time.time()  # 开始计时
-        attribute_response = ModelCaller.call(self, messages=messages, **sample_kwargs)
-        elapsed_time = time.time() - start_time  # 计算经过的时间
-
-        attribute_answer = ModelCaller.parse_response(attribute_response)
+        attribute_response, elapsed_time = ModelCaller.call(self, messages=messages, **sample_kwargs)
+        attribute_answer = ModelCaller.parse_response(self, attribute_response)
 
         attribute_response.elapsed_time = elapsed_time
         attribute_response.prompt = json.dumps(prompt)
         attribute_response.completion = attribute_answer
 
         classification = []
         for line in attribute_answer.split('\n'):
```

### Comparing `zeval-0.1.1/zeval/evaluators/faithfulness.py` & `zeval-0.1.2/zeval/evaluators/faithfulness.py`

 * *Files identical despite different names*

### Comparing `zeval-0.1.1/zeval/utils/model.py` & `zeval-0.1.2/zeval/utils/model.py`

 * *Files identical despite different names*

### Comparing `zeval-0.1.1/zeval.egg-info/PKG-INFO` & `zeval-0.1.2/zeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeval
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for evaluating RAG outputs of Chinese large language models.
 Home-page: https://github.com/yourgithub/zeval
 Author: everfly
 Author-email: tagriver@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

