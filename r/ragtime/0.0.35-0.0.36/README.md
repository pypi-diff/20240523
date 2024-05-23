# Comparing `tmp/ragtime-0.0.35.tar.gz` & `tmp/ragtime-0.0.36.tar.gz`

## Comparing `ragtime-0.0.35.tar` & `ragtime-0.0.36.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ragtime-0.0.35/CHANGELOG.md
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.35/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.35/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.35/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/api.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/config.py
--rw-r--r--   0        0        0    22584 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/expe.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/pipeline.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/llm.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/prompter.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/retriever.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/text_generator.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
--rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/__init__.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/answer/base.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/answer/with_retriever.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/eval/fr.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/fact/fr.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/__init__.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/answer_generator.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/eval_generator.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/fact_generator.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/test_quest.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.35/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.35/LICENSE
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.35/README.md
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ragtime-0.0.35/pyproject.toml
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ragtime-0.0.36/CHANGELOG.md
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.36/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.36/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.36/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/api.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/config.py
+-rw-r--r--   0        0        0    22584 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/expe.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/pipeline.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base/llm.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base/prompter.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base/retriever.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base/text_generator.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/prompters/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/prompters/answer/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/prompters/answer/with_retriever.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/prompters/eval/fr.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/prompters/fact/fr.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/text_generators/__init__.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/text_generators/answer_generator.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/text_generators/eval_generator.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ragtime-0.0.36/src/ragtime/text_generators/fact_generator.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.36/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.36/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.36/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.36/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.36/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.36/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ragtime-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.36/PKG-INFO
```

### Comparing `ragtime-0.0.35/CHANGELOG.md` & `ragtime-0.0.36/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/CONTRIBUTING.md` & `ragtime-0.0.36/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/img/Ragtime_logo.png` & `ragtime-0.0.36/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/__init__.py` & `ragtime-0.0.36/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/api.py` & `ragtime-0.0.36/src/ragtime/api.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/config.py` & `ragtime-0.0.36/src/ragtime/config.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/expe.py` & `ragtime-0.0.36/src/ragtime/expe.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/pipeline.py` & `ragtime-0.0.36/src/ragtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base/llm.py` & `ragtime-0.0.36/src/ragtime/base/llm.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base/prompter.py` & `ragtime-0.0.36/src/ragtime/base/prompter.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base/retriever.py` & `ragtime-0.0.36/src/ragtime/base/retriever.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base/text_generator.py` & `ragtime-0.0.36/src/ragtime/base/text_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.36/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.36/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/classes.py` & `ragtime-0.0.36/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/main.py` & `ragtime-0.0.36/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.36/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx` & `ragtime-0.0.36/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/prompters/__init__.py` & `ragtime-0.0.36/src/ragtime/prompters/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/prompters/answer/base.py` & `ragtime-0.0.36/src/ragtime/prompters/answer/base.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/prompters/answer/with_retriever.py` & `ragtime-0.0.36/src/ragtime/prompters/answer/with_retriever.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/prompters/eval/fr.py` & `ragtime-0.0.36/src/ragtime/prompters/eval/fr.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/prompters/fact/fr.py` & `ragtime-0.0.36/src/ragtime/prompters/fact/fr.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/text_generators/answer_generator.py` & `ragtime-0.0.36/src/ragtime/text_generators/answer_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/text_generators/eval_generator.py` & `ragtime-0.0.36/src/ragtime/text_generators/eval_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/src/ragtime/text_generators/fact_generator.py` & `ragtime-0.0.36/src/ragtime/text_generators/fact_generator.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/tests/full_test.py` & `ragtime-0.0.36/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/tests/run_tests.py` & `ragtime-0.0.36/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/tests/test_quest.json` & `ragtime-0.0.36/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/.gitignore` & `ragtime-0.0.36/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/LICENSE` & `ragtime-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/README.md` & `ragtime-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.35/pyproject.toml` & `ragtime-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.35"
+version = "0.0.36"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
```

### Comparing `ragtime-0.0.35/PKG-INFO` & `ragtime-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.35
+Version: 0.0.36
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
```

