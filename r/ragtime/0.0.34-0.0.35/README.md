# Comparing `tmp/ragtime-0.0.34.tar.gz` & `tmp/ragtime-0.0.35.tar.gz`

## Comparing `ragtime-0.0.34.tar` & `ragtime-0.0.35.tar`

### file list

```diff
@@ -1,31 +1,44 @@
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 ragtime-0.0.34/CHANGELOG.md
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.34/CONTRIBUTING.md
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.34/deploy/deploy.py
--rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.34/img/Ragtime_logo.png
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/api.py
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/config.py
--rw-r--r--   0        0        0    21163 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/expe.py
--rw-r--r--   0        0        0    43142 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/generators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/LICENSE
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/README.md
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/classes.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/main.py
--rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/html_templates/basic_template.jinja
--rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
--rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
--rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
--rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
--rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
--rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.34/tests/full_test.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.34/tests/run_tests.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.34/tests/test_quest.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.34/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.34/LICENSE
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.34/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragtime-0.0.34/pyproject.toml
--rw-r--r--   0        0        0     7473 2020-02-02 00:00:00.000000 ragtime-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ragtime-0.0.35/CHANGELOG.md
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 ragtime-0.0.35/CONTRIBUTING.md
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ragtime-0.0.35/deploy/deploy.py
+-rw-r--r--   0        0        0    20599 2020-02-02 00:00:00.000000 ragtime-0.0.35/img/Ragtime_logo.png
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/api.py
+-rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/config.py
+-rw-r--r--   0        0        0    22584 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/expe.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/pipeline.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/llm.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/prompter.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/retriever.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base/text_generator.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/LICENSE
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/README.md
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/classes.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/main.py
+-rw-r--r--   0        0        0    15410 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/html_templates/basic_template.jinja
+-rw-r--r--   0        0        0    91060 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx
+-rw-r--r--   0        0        0    21761 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx
+-rw-r--r--   0        0        0    33574 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx
+-rw-r--r--   0        0        0    27639 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx
+-rw-r--r--   0        0        0    29959 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx
+-rw-r--r--   0        0        0    33387 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/__init__.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/answer/base.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/answer/with_retriever.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/eval/fr.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/prompters/fact/fr.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/__init__.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/answer_generator.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/eval_generator.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 ragtime-0.0.35/src/ragtime/text_generators/fact_generator.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/full_test.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/run_tests.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragtime-0.0.35/tests/test_quest.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 ragtime-0.0.35/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 ragtime-0.0.35/LICENSE
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 ragtime-0.0.35/README.md
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 ragtime-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 ragtime-0.0.35/PKG-INFO
```

### Comparing `ragtime-0.0.34/CHANGELOG.md` & `ragtime-0.0.35/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# v0.0.36 
+- Module renamed
+- Removed deprecated prompter (see v0.0.33)
+
+# v0.0.35
+- PR in progress
+
 # v0.0.34 - May 16th 2024
 - bug fixed in question number display in logs (in `LiteLLM.complete`)
 
 # v0.0.33 - May 15th 2024
 - removed old Eval prompters `PptrTwoFactsEvalFR` and `PptrSimpleEvalFR` and old Eval generator `TwoFactsEvalGenerator`
 - removed old Facts prompter `PptrSimpleFactsFR`
 - renamed Answer prompter `PptrBaseAns` to `PptrAnsBase`, Facts prompter `PptrFactsFRv2` to `PptrFactsFR`, Evals prompter `PptrEvalFRv2` to `PptrEvalFR`
```

### Comparing `ragtime-0.0.34/CONTRIBUTING.md` & `ragtime-0.0.35/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/img/Ragtime_logo.png` & `ragtime-0.0.35/img/Ragtime_logo.png`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/__init__.py` & `ragtime-0.0.35/src/ragtime/__init__.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/api.py` & `ragtime-0.0.35/src/ragtime/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,34 +16,34 @@
     REQ_DELETE: requests.delete,
     }
 
 ################
 # call
 # @retry(Exception, tries=5, delay=3, jitter=(0,3))
 def call(a_req_type: str, a_url: str, **kwargs) -> Response:
-    """Calls API and manages errors
+    """
+    Calls API and manages errors
     Args:
         a_req_type: type of request (GET, POST, PUT, DELETE)
         a_url
         *args: variable number of extra argument
         **kwargs: variable number of keyword arguments
     Returns:
         Response
     """
-    r: Optional[Response] = None
+    response: Optional[Response] = None
     err_msg:str = f'Type: {a_req_type} - Route: {a_url} - Args: {kwargs}'
 
     try:
         if kwargs == {}:
-            r = _req_type_func[a_req_type](url=a_url)
+            response = _req_type_func[a_req_type](url=a_url)
         else:
-            r = _req_type_func[a_req_type](a_url, **kwargs)
-        if r is not None:
-            err_msg += '\n'+f'Response status: {r.status_code} - Response reason:{r.reason} - Response content: {str(r.content)}'
+            response = _req_type_func[a_req_type](a_url, **kwargs)
+        if response is not None:
+            err_msg += '\n'+f'Response status: {response.status_code} - Response reason:{response.reason} - Response content: {str(response.content)}'
     except:
-        s: str = 'before' if r is None else 'after'
+        s: str = 'before' if response is None else 'after'
         raise Exception(f'Exception raised {s} calling - {err_msg}')
-    if r is not None and r.status_code < 300:
-        return r
+    if response is not None and response.status_code < 300:
+        return response
     else:
         raise Exception(f'API called but returned error - {err_msg}')
-
```

### Comparing `ragtime-0.0.34/src/ragtime/config.py` & `ragtime-0.0.35/src/ragtime/config.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/expe.py` & `ragtime-0.0.35/src/ragtime/expe.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,33 @@
 from enum import Enum, IntEnum
 import json
 from pathlib import Path
 import re
 import shutil
 from openpyxl import load_workbook, Workbook
 from openpyxl.worksheet.worksheet import Worksheet
+from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
 from copy import copy
 from datetime import datetime
 from typing import Any, Callable, Generic, Optional, TypeVar, Union
 from pydantic import BaseModel, Field
-from ragtime.config import DEFAULT_FACTS_COL, DEFAULT_HUMAN_EVAL_COL, DEFAULT_HEADER_SIZE, DEFAULT_HUMAN_EVAL_COL, DEFAULT_ANSWERS_COL, DEFAULT_QUESTION_COL, DEFAULT_SPREADSHEET_TEMPLATE, DEFAULT_WORKSHEET, RagtimeException, logger, DEFAULT_HTML_RENDERING, DEFAULT_HTML_TEMPLATE
+from ragtime.config import (
+    DEFAULT_FACTS_COL,
+    DEFAULT_HUMAN_EVAL_COL,
+    DEFAULT_HEADER_SIZE,
+    DEFAULT_HUMAN_EVAL_COL,
+    DEFAULT_ANSWERS_COL,
+    DEFAULT_QUESTION_COL,
+    DEFAULT_SPREADSHEET_TEMPLATE,
+    DEFAULT_WORKSHEET,
+    RagtimeException,
+    logger,
+    DEFAULT_HTML_RENDERING,
+    DEFAULT_HTML_TEMPLATE
+    )
 from jinja2 import Environment, FileSystemLoader
 from tabulate import tabulate
 
 class RagtimeBase(BaseModel):
     meta: dict[str, Any] = {}
 
 class RagtimeText(RagtimeBase):
@@ -218,14 +232,22 @@
             qa_list:dict = data
             if 'meta' in data:
                 self.meta = data['meta']
                 qa_list = data['items']
             for json_qa in qa_list:
                 qa:QA = QA(**json_qa)
                 self.append(qa)
+
+    def filter_answer(self, llm_facts_name: str):
+        """
+        Filters the current Expe object to include only the QA pairs with answers from the specified LLM.
+        """
+        for qa in self:
+            filtered_answers = [a for a in qa.answers if a.llm_answer and a.llm_answer.name == llm_facts_name]
+            qa.answers = Answers(items=filtered_answers)
     
     # TODO: Cannot implement this function due to circular imports issue (need objects from generators.py objects and generators.py needs
     # expe.py objects too) - if someone finds a way, that would be nice since it would allow to easily chain Answer, Facts and Eval generation
     # def gen_Eval(self, folder_out:Path, prompter:Prompter, llm_names:list[str],
     #             start_from:StartFrom=StartFrom.beginning, b_missing_only:bool = False, only_llms:list[str] = None, save_every:int=0):
     #     eval_gen:EvalGenerator = EvalGenerator(llm_names=llm_names, prompter=prompter)
     #     eval_gen.generate(self, start_from=start_from,  b_missing_only=b_missing_only, only_llms=only_llms, save_every=save_every)
@@ -296,119 +318,150 @@
             file_name:str = f'{name}{self.json_path.stem}'
             file_path:str = self.json_path.parent
         else:
             file_name:str = f'{name}.json'
             file_path:str = ''
         self.save_to_json(path=Path(file_path) / Path(file_name), b_overwrite=True, b_add_suffix=True)
 
-    def save_to_json(self, path:Path=None, b_overwrite:bool=False, b_add_suffix:bool = True) -> Path:
-        """Saves Expe to JSON - can generate a suffix for the filename
-        Returns the Path of the file actually saved"""
-        path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, 
-                                                    b_add_suffix=b_add_suffix, force_ext='.json')
+    def save_to_json(
+            self,
+            path:Path=None,
+            b_overwrite:bool=False,
+            b_add_suffix:bool = True
+    ) -> Path:
+        """
+        Saves Expe to JSON - can generate a suffix for the filename
+        Returns the Path of the file actually saved
+        """
+        path:Path = self._file_check_before_writing(
+            path,
+            b_overwrite = b_overwrite,
+            b_add_suffix = b_add_suffix,
+            force_ext='.json'
+        )
         with open(path, mode='w', encoding='utf-8') as file:
             file.write(self.model_dump_json(indent=2))
         self.json_path = path
         logger.info(f'Expe saved as JSON to {path}')
         return path
 
-    def save_to_html(self, path:Path=None, render_params:dict[str,bool]=DEFAULT_HTML_RENDERING,
-                     template_path:Path=DEFAULT_HTML_TEMPLATE, b_overwrite:bool=False, b_add_suffix:bool = True):
-        """Saves Expe to an HTML file from a Jinja template - can generate a suffix for the filename
-        Returns the Path of the file actually saved"""
+    def save_to_html(
+            self,
+            path:Path = None,
+            b_overwrite:bool=False,
+            b_add_suffix:bool = True,
+            render_params:dict[str,bool] = DEFAULT_HTML_RENDERING,
+            template_path:Path = DEFAULT_HTML_TEMPLATE,
+    ):
+        """
+        Saves Expe to an HTML file from a Jinja template - can generate a suffix for the filename
+        Returns the Path of the file actually saved
+        """
         path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext='.html')
         environment = Environment(loader=FileSystemLoader(searchpath=template_path.parent,encoding='utf-8'))
         template = environment.get_template(template_path.name)
         context = {"expe": self, **render_params, "report_name": self.get_name(), "sub": (lambda pattern, repl, s: re.sub(pattern, repl, s))}
         with open(path, mode='w', encoding='utf-8') as file:
             file.write(template.render(context))
         logger.info(f'Expe saved as HTML to {path}')
         return path
 
-    def save_to_spreadsheet(self, path:Path=None, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
-                            header_size:int=DEFAULT_HEADER_SIZE, sheet_name:str = DEFAULT_WORKSHEET,
-                            b_overwrite:bool=False, b_add_suffix:bool = True):
-        """Saves Expe to a spreadsheet - can generate a suffix for the filename
-        Returns the Path of the file actually saved"""
-        path:Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix, force_ext='.xlsx')
-        
-        # Prepare the result file
-        # Copy template
-        shutil.copy(template_path, path)
-        wb:Workbook = load_workbook(path)
-        wb.iso_dates = True
-        
-        # Create worksheet
-        ws:Worksheet = wb[sheet_name]
-
-        # Retreive sst configuration from original file
-        # ws_conf is a list of str, each element describes the path of the data to be added in the current row
-        ws_conf:list[str] = [cell.value for cell in ws[header_size+1]]
-        
-        # Write the values at specific rows - they are defined in second row, below the one describing the value to insert
-        for cell in ws[header_size+2]: # read the row just after the conf row - it contains configuration for specific rows
-            # if a value is present, analyse it - it should contain a "row" indication e.g. "answers[0].full_name, row=1"
-            if cell.value:
-                if cell.value == "#": continue # special token # used to indicate question number
-                val:str = cell.value
-                row:int = int(val[val.find('row=')+len('row='):])
-                if row < 1: raise RagtimeException(f'The row value "row={row}" specified in cell {cell.coordinate} is invalid and must be greater than 0')
-                # write the value since it does not need to be done for each row
-                p:str = val[:val.find(',')]
-                # get the first non empty value in the required column
-                val = next((qa.get_attr(p) for qa in self if qa.get_attr(p)), "")
-                ws.cell(row=row, column=cell.column, value=val)
-
-        qa:QA
-        row:int = header_size+1
-        col_with_formulas:dict[int, str] = {c: ws.cell(column=c, row=row).value
-                                            for c in range(1, ws.max_column) 
-                                            if ws.cell(column=c, row=row).value and str(ws.cell(column=c, row=row).value)[0] == "="}
-        for num_q, qa in enumerate(self, start=1): # write each row in expe
-            next_row:int = 0
-            for col, p in enumerate(ws_conf, start=1):
-                if p == "#": # special token # used to indicate question number
-                    val = [num_q]
-                elif p[0] == "=": # if a formula is here, write it as is in the formula field
-                    continue
-                else: # if it is a path to get a value in QA, get it
-                    # Get value in the QA object
-                    val = qa.get_attr(p)
-                    if val is None or val == []: val = [""] # write a blank if nothing is found
-                if not isinstance(val, list): val = [val]
-                
-                # Write the value(s)
-                for offset, v in enumerate(val):
-                    # Do standard conversions to string
-                    if isinstance(v, list): v = str(v)
-                    elif isinstance(v, datetime): v = v.strftime("%d/%m/%Y %H:%M:%S")
-                    # Write value
-                    ws.cell(row=row+offset, column=col).value = v
-                    # From second row copy cell style from the one up
-                    if row+offset > header_size+1:
-                        ws.cell(row=row+offset, column=col)._style = copy(ws.cell(row=header_size+1, column=col)._style)
-                
-                next_row = max(next_row, row+offset+1)
-            row = next_row
-
-        # extend the formulas
-        for row in range(header_size+1, ws.max_row):
-            for col, formula in col_with_formulas.items():
-                # simply adjust the row number in the formula
-                cell_refs:set = set(re.findall(r"[A-Z]+[0-9]+", formula))
-                for cell_ref in cell_refs:
-                    new_cell_ref:str = cell_ref.replace(str(header_size+1), str(row))
-                    formula = formula.replace(cell_ref, new_cell_ref)
-                ws.cell(row=row, column=col, value=formula)
-        
-        # save spreadsheet
-        wb.save(path)
-        logger.info(f'Expe saved as Spreadsheet to {path}')
-        return path
+    def save_to_spreadsheet(self, path: Path = None, template_path: Path = DEFAULT_SPREADSHEET_TEMPLATE,
+                        header_size: int = DEFAULT_HEADER_SIZE, sheet_name: str = DEFAULT_WORKSHEET,
+                        b_overwrite: bool = False, b_add_suffix: bool = True):
+            """Saves Expe to a spreadsheet - can generate a suffix for the filename
+            Returns the Path of the file actually saved"""
+            path: Path = self._file_check_before_writing(path, b_overwrite=b_overwrite, b_add_suffix=b_add_suffix,
+                                                        force_ext='.xlsx')
+
+            # Prepare the result file
+            # Copy template
+            shutil.copy(template_path, path)
+            wb: Workbook = load_workbook(path)
+            wb.iso_dates = True
+
+            # Create worksheet
+            ws: Worksheet = wb[sheet_name]
+
+            # Retrieve sst configuration from original file
+            # ws_conf is a list of str, each element describes the path of the data to be added in the current row
+            ws_conf: list[str] = [cell.value for cell in ws[header_size + 1]]
+
+            # Write the values at specific rows - they are defined in second row, below the one describing the value to insert
+            for cell in ws[header_size + 2]:  # read the row just after the conf row - it contains configuration for specific rows
+                # if a value is present, analyse it - it should contain a "row" indication e.g. "answers[0].full_name, row=1"
+                if cell.value:
+                    if cell.value == "#":
+                        continue  # special token # used to indicate question number
+                    val: str = cell.value
+                    row: int = int(val[val.find('row=') + len('row='):])
+                    if row < 1:
+                        raise RagtimeException(
+                            f'The row value "row={row}" specified in cell {cell.coordinate} is invalid and must be greater than 0')
+                    # write the value since it does not need to be done for each row
+                    p: str = val[:val.find(',')]
+                    # get the first non empty value in the required column
+                    val = next((qa.get_attr(p) for qa in self if qa.get_attr(p)), "")
+                    ws.cell(row=row, column=cell.column, value=val)
+
+            qa: QA
+            row: int = header_size + 1
+            col_with_formulas: dict[int, str] = {c: ws.cell(column=c, row=row).value
+                                                for c in range(1, ws.max_column)
+                                                if ws.cell(column=c, row=row).value and str(ws.cell(column=c, row=row).value)[
+                                                    0] == "="}
+            for num_q, qa in enumerate(self, start=1):  # write each row in expe
+                next_row: int = 0
+                for col, p in enumerate(ws_conf, start=1):
+                    if p == "#":  # special token # used to indicate question number
+                        val = [num_q]
+                    elif p[0] == "=":  # if a formula is here, write it as is in the formula field
+                        continue
+                    else:  # if it is a path to get a value in QA, get it
+                        # Get value in the QA object
+                        val = qa.get_attr(p)
+                        if val is None or val == []:
+                            val = [""]  # write a blank if nothing is found
+                    if not isinstance(val, list):
+                        val = [val]
+
+                    # Write the value(s)
+                    for offset, v in enumerate(val):
+                        # Do standard conversions to string
+                        if isinstance(v, list):
+                            v = str(v)
+                        elif isinstance(v, datetime):
+                            v = v.strftime("%d/%m/%Y %H:%M:%S")
+                        # Remove illegal characters before writing the value
+                        cleaned_value = ILLEGAL_CHARACTERS_RE.sub("", str(v))
+                        # Write value
+                        ws.cell(row=row + offset, column=col).value = cleaned_value
+                        # From second row copy cell style from the one up
+                        if row + offset > header_size + 1:
+                            ws.cell(row=row + offset, column=col)._style = copy(ws.cell(row=header_size + 1, column=col)._style)
+
+                    next_row = max(next_row, row + offset + 1)
+                row = next_row
+
+            # extend the formulas
+            for row in range(header_size + 1, ws.max_row):
+                for col, formula in col_with_formulas.items():
+                    # simply adjust the row number in the formula
+                    cell_refs: set = set(re.findall(r"[A-Z]+[0-9]+", formula))
+                    for cell_ref in cell_refs:
+                        new_cell_ref: str = cell_ref.replace(str(header_size + 1), str(row))
+                        formula = formula.replace(cell_ref, new_cell_ref)
+                    ws.cell(row=row, column=col, value=formula)
+
+            # save spreadsheet
+            wb.save(path)
+            logger.info(f'Expe saved as Spreadsheet to {path}')
+            return path
     
+
 def analyse_expe_folder(path:Path):
     if not path.is_dir(): raise Exception(f'"{path}" is not a folder - please provide one')
     print(f'In "{path}":')
     res:defaultdict = defaultdict(list)
     for f in [f for f in path.iterdir() if f.is_file() and f.suffix == '.json']:
         exp:Expe = Expe(json_path=f)
         res['File'].append(f.name)
@@ -420,8 +473,8 @@
                      template_path:Path=DEFAULT_HTML_TEMPLATE):
   expe:Expe = Expe(json_path=json_path)
   expe.save_to_html(path=json_path, render_params=render_params, template_path=template_path, b_add_suffix=True)
 
 def export_to_spreadsheet(json_path:Path, template_path:Path=DEFAULT_SPREADSHEET_TEMPLATE,
                             header_size:int=DEFAULT_HEADER_SIZE, sheet_name:str = DEFAULT_WORKSHEET,):
   expe:Expe = Expe(json_path=json_path)
-  expe.save_to_spreadsheet(path=json_path, template_path=template_path, header_size=header_size, sheet_name=sheet_name, b_add_suffix=True)
+  expe.save_to_spreadsheet(path=json_path, template_path=template_path, header_size=header_size, sheet_name=sheet_name, b_add_suffix=True)
```

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/.gitignore` & `ragtime-0.0.35/src/ragtime/base_folder/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/LICENSE` & `ragtime-0.0.35/src/ragtime/base_folder/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/classes.py` & `ragtime-0.0.35/src/ragtime/base_folder/classes.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/main.py` & `ragtime-0.0.35/src/ragtime/base_folder/main.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/expe/01. Questions/json_helper.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/html_templates/basic_template.jinja` & `ragtime-0.0.35/src/ragtime/base_folder/res/html_templates/basic_template.jinja`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/MCQ.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/first_questions.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/test_facts.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/with_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/without_retriever.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/basic_template_old.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx` & `ragtime-0.0.35/src/ragtime/base_folder/res/spreadsheet_templates/old/spreadsheet_rich_template.xlsx`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/tests/full_test.py` & `ragtime-0.0.35/tests/full_test.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/tests/run_tests.py` & `ragtime-0.0.35/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/tests/test_quest.json` & `ragtime-0.0.35/tests/test_quest.json`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/.gitignore` & `ragtime-0.0.35/.gitignore`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/LICENSE` & `ragtime-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/README.md` & `ragtime-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `ragtime-0.0.34/pyproject.toml` & `ragtime-0.0.35/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ragtime"
-version = "0.0.34"
+version = "0.0.35"
 
 authors = [
   { name="Gilles Moyse", email="gilles@recital.ai" },
 ]
 maintainers = [
   { name="reciTAL", email="ragtime@recital.ai" },
 ]
@@ -20,12 +20,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["RAG", "LLM", "Evaluation"]
 dependencies = ['requests', 'retry', 'pathlib', 'openpyxl', 'langdetect',
-'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv', 'py_setenv', 'lazy_import']
+'pydantic', 'jinja2', 'tabulate', 'unidecode', 'litellm', 'setenv', 'py_setenv', 'lazy_import',
+'asyncio', 'toml']
 
 [project.urls]
 Homepage = "https://github.com/recitalAI/ragtime-package"
-Issues = "https://github.com/recitalAI/ragtime-package/issues"
+Issues = "https://github.com/recitalAI/ragtime-package/issues"
```

### Comparing `ragtime-0.0.34/PKG-INFO` & `ragtime-0.0.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragtime
-Version: 0.0.34
+Version: 0.0.35
 Summary: Ragtime 🎹 is an LLMOps framework to automatically evaluate Retrieval Augmented Generation (RAG) systems and compare different RAGs / LLMs
 Project-URL: Homepage, https://github.com/recitalAI/ragtime-package
 Project-URL: Issues, https://github.com/recitalAI/ragtime-package/issues
 Author-email: Gilles Moyse <gilles@recital.ai>
 Maintainer-email: reciTAL <ragtime@recital.ai>
 License: MIT License
         
@@ -30,26 +30,28 @@
 License-File: LICENSE
 Keywords: Evaluation,LLM,RAG
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
+Requires-Dist: asyncio
 Requires-Dist: jinja2
 Requires-Dist: langdetect
 Requires-Dist: lazy-import
 Requires-Dist: litellm
 Requires-Dist: openpyxl
 Requires-Dist: pathlib
 Requires-Dist: py-setenv
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: retry
 Requires-Dist: setenv
 Requires-Dist: tabulate
+Requires-Dist: toml
 Requires-Dist: unidecode
 Description-Content-Type: text/markdown
 
 <img src="img/Ragtime_logo.png" alt="Ragtime 🎹 LLM Ops for all">
 
 # Presentation
 **Ragtime** 🎹 is an LLMOps framework which allows you to automatically:
```

