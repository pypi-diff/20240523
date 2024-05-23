# Comparing `tmp/ru_text_cleaner-1.1.5.tar.gz` & `tmp/ru_text_cleaner-2.0.0.tar.gz`

## Comparing `ru_text_cleaner-1.1.5.tar` & `ru_text_cleaner-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,33 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/requirements.txt
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/.gitignore
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/TextCleaner.iml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/vcs.xml
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/workspace.xml
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/TextCleaner.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/__init__.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_clean_stopwords.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_emoji_cleaner.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_html_cleaner.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_punctuation_cleaner.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_spaces_cleaner.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_to_lower.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/src/ru_text_cleaner/_to_morpheme.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/LICENSE
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 ru_text_cleaner-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/requirements.txt
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/TextCleaner.iml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/__init__.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/__init__.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/TextCleaner.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/__init__.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_clean_stopwords.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_emoji_cleaner.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_html_cleaner.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_punctuation_cleaner.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_spaces_cleaner.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_to_lower.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/src/ru_text_cleaner/tensor_cleaner/_to_morpheme.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/README.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 ru_text_cleaner-2.0.0/PKG-INFO
```

### Comparing `ru_text_cleaner-1.1.5/.idea/inspectionProfiles/Project_Default.xml` & `ru_text_cleaner-2.0.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.5/src/ru_text_cleaner/TextCleaner.py` & `ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/TextCleaner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from . import *
+from ._html_cleaner import clean_html
+from ._spaces_cleaner import clean_spaces
+from ._to_morpheme import text_to_morphems
+from ._to_lower import to_lower_text
+from ._emoji_cleaner import clean_emoji
+from ._clean_stopwords import clean_stopwords
+from ._punctuation_cleaner import clean_punctuation
 
 
 class TextCleaner:
     def __init__(self, spaces=True, punctuation=True, html=True, emoji=True, lower=True,
                  stop_words=True, morpheme=True):
 
         """
@@ -35,47 +41,57 @@
         self.to_morpheme = text_to_morphems
 
     def clean_text(self, text: str) -> str:
 
         """ Метод clean_text форматирует текст в зависимости от поставленных флагов"""
 
         if self.lower:
-            text = self.to_lower(self, text)
+            text = self.to_lower(text)
         if self.emoji:
-            text = self.clean_emoji(self, text)
+            text = self.clean_emoji(text)
         if self.html:
-            text = self.clean_html(self, text)
+            text = self.clean_html(text)
         if self.punctuation:
-            text = self.clean_punctuation(self, text)
+            text = self.clean_punctuation(text)
         if self.stopwords:
-            text = self.clean_stopwords(self, text)
+            text = self.clean_stopwords(text)
         if self.morpheme:
-            text = self.to_morpheme(self, text)
+            text = self.to_morpheme(text)
         if self.spaces:
-            text = self.clean_space(self, text)
+            text = self.clean_space(text)
 
         return text
 
     def clean_texts(self, texts: []) -> []:
 
         clean_texts = []
 
         """ Метод clean_texts форматирует массив в зависимости от поставленных флагов"""
 
         for text in texts:
             if self.lower:
-                text = self.to_lower(self, text)
+                text = self.to_lower(text)
             if self.emoji:
-                text = self.clean_emoji(self, text)
+                text = self.clean_emoji(text)
             if self.html:
-                text = self.clean_html(self, text)
+                text = self.clean_html(text)
             if self.punctuation:
-                text = self.clean_punctuation(self, text)
+                text = self.clean_punctuation(text)
             if self.stopwords:
-                text = self.clean_stopwords(self, text)
+                text = self.clean_stopwords(text)
             if self.morpheme:
-                text = self.to_morpheme(self, text)
+                text = self.to_morpheme(text)
             if self.spaces:
-                text = self.clean_space(self, text)
+                text = self.clean_space(text)
             clean_texts.append(text)
 
         return clean_texts
+
+    def to_vector(self, text: str) -> []:
+        return self.clean_text(text).split()
+
+    def to_vectors(self, text: []) -> []:
+        clean_texts = self.clean_texts(text)
+        answer = []
+        for t in clean_texts:
+            answer.append(t.split())
+        return answer
```

### Comparing `ru_text_cleaner-1.1.5/src/ru_text_cleaner/_clean_stopwords.py` & `ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_clean_stopwords.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import nltk
 nltk.download('stopwords')
 from nltk.corpus import stopwords
 
 
-def clean_stopwords(self, text: str) -> str:
+def clean_stopwords(text: str) -> str:
 
     """
     Метод clean_stopwords убирает все стоп слова
 
     stop_words = set(stopwords.words('russian')) - Получает список стоп слов
 
     words = text.split(' ') - Слова заменяет на пробелы
```

### Comparing `ru_text_cleaner-1.1.5/src/ru_text_cleaner/_spaces_cleaner.py` & `ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_spaces_cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-def clean_spaces(self, text: str) -> str:
+def clean_spaces(text: str) -> str:
 
     """
     Метод clean_spaces убирает лишние пробелы из текста
 
         re.sub(r' +', ' ', text) - Ищет в переданном тексте лишние пробелы, заменяет их на один пробел
         return text.strip() - Возвращает готовый текст убирая лишние пробелы
```

### Comparing `ru_text_cleaner-1.1.5/src/ru_text_cleaner/_to_morpheme.py` & `ru_text_cleaner-2.0.0/src/ru_text_cleaner/simple_cleaner/_to_morpheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pymorphy2
 
 
-def text_to_morphems(self, text: str) -> str:
+def text_to_morphems(text: str) -> str:
 
     """
     Метод text_to_morphems заменяет слова на морфемы
 
     morph = pymorphy2.MorphAnalyzer(lang='ru') - получает список морфем
 
     for i in text.split(' '):
```

### Comparing `ru_text_cleaner-1.1.5/LICENSE` & `ru_text_cleaner-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.5/README.md` & `ru_text_cleaner-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ru_text_cleaner-1.1.5/pyproject.toml` & `ru_text_cleaner-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1']
+requires = ['pymorphy2>=0.9.1', 'nltk>=3.8.1', 'hatchling', 'emoji>=2.11.1', 'tensorflow>=2.16.1']
 build-backend = "hatchling.build"
 
 [project]
 name = "ru-text-cleaner"
-version = "1.1.5"
+version = "2.0.0"
 authors = [
     { name="Vildan Nasyrov", email="" },
     { name="Artem Gafarov", email="a.m.gafarov@ya.ru" },
 ]
 description = "Cleans russian text and preparing for NLP"
 requires-python = ">=3.10.4"
 readme = "README.md"
```

### Comparing `ru_text_cleaner-1.1.5/PKG-INFO` & `ru_text_cleaner-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ru-text-cleaner
-Version: 1.1.5
+Version: 2.0.0
 Summary: Cleans russian text and preparing for NLP
 Project-URL: Homepage, https://github.com/rvneural/TextCleaner
 Project-URL: Issues, https://github.com/rvneural/TextCleaner/issues
 Author: Vildan Nasyrov
 Author-email: Artem Gafarov <a.m.gafarov@ya.ru>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

