# Comparing `tmp/docrobot-1.1.2.tar.gz` & `tmp/docrobot-1.1.3.tar.gz`

## Comparing `docrobot-1.1.2.tar` & `docrobot-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.1.2/convert.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.1.2/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.1.2/src/docrobot/__init__.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 docrobot-1.1.2/src/docrobot/form.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 docrobot-1.1.2/src/docrobot/form.ui
--rw-r--r--   0        0        0    24069 2020-02-02 00:00:00.000000 docrobot-1.1.2/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.1.2/LICENSE
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.1.2/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 docrobot-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 docrobot-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.1.3/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.1.3/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.1.3/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 docrobot-1.1.3/src/docrobot/form.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 docrobot-1.1.3/src/docrobot/form.ui
+-rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 docrobot-1.1.3/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.1.3/LICENSE
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.1.3/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 docrobot-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 docrobot-1.1.3/PKG-INFO
```

### Comparing `docrobot-1.1.2/.github/workflows/python-publish.yml` & `docrobot-1.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.1.2/src/docrobot/form.py` & `docrobot-1.1.3/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.1.2/src/docrobot/form.ui` & `docrobot-1.1.3/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.1.2/src/docrobot/guimain.pyw` & `docrobot-1.1.3/src/docrobot/guimain.pyw`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         prompt = '项目立项表IP更新完成。 <font color="green"><b>' + str(match) + ' </b></font> 项条目匹配。'
         if unmatch != 0:
             prompt = prompt + ' <font color="red"><b>' + str(unmatch) + ' </b></font> 项条目不匹配。'
         self.textEdit.append(prompt)
 
     def checkpat2(self, doc, prj):
         match = unmatch = 0
-        pat1 = pat2 = pat3 = 0
+        pat1 = pat2 = pat3 = pat4 = 0
         lst = prj.pat_list.splitlines()
         for pat_name in lst:
             if pat_name in self.pat_dict2:
                 pat = self.pat_dict2[pat_name]
                 check_str = '知识产权类型错误时默认字符串'
                 match pat.p_class:
                     case '软件著作权':
@@ -246,14 +246,17 @@
                         pat1 = pat1 + 1
                     case '实用新型':
                         check_str = pat.p_name + '，授权号：' + pat.p_no
                         pat2 = pat2 + 1
                     case '发明专利' | '发明公布':
                         check_str = pat.p_name + '，授权号：' + pat.p_no
                         pat3 = pat3 + 1
+                    case '集成电路布图':
+                        check_str = pat.p_name + '，授权号：' + pat.p_no
+                        pat4 = pat4 + 1
                     case _:
                         self.textEdit.append('知识产权类型错误：' + pat.p_name + '：' + pat.p_class)
                 found = False
                 for i, para in enumerate(doc.tables[2].rows[4].cells[0].paragraphs):
                     if check_str in para.text:
                         found |= True
                         match = match + 1
```

### Comparing `docrobot-1.1.2/LICENSE` & `docrobot-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.1.2/PKG-INFO` & `docrobot-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: docrobot
-Version: 1.1.2
+Version: 1.1.3
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

