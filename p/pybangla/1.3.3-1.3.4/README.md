# Comparing `tmp/pybangla-1.3.3.tar.gz` & `tmp/pybangla-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.3.3.tar", last modified: Wed May 22 12:29:48 2024, max compression
+gzip compressed data, was "pybangla-1.3.4.tar", last modified: Thu May 23 18:06:30 2024, max compression
```

## Comparing `pybangla-1.3.3.tar` & `pybangla-1.3.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:44.000000 pybangla-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-22 12:29:48.586884 pybangla-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-22 12:29:44.000000 pybangla-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.582884 pybangla-1.3.3/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:29:48.586884 pybangla-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 12:29:44.000000 pybangla-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-22 12:29:44.000000 pybangla-1.3.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:30.886899 pybangla-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:26.000000 pybangla-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-23 18:06:30.886899 pybangla-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-23 18:06:26.000000 pybangla-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:30.882899 pybangla-1.3.4/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:30.886899 pybangla-1.3.4/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31159 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/phone_number_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/report_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-23 18:06:26.000000 pybangla-1.3.4/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:30.886899 pybangla-1.3.4/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-23 18:06:30.000000 pybangla-1.3.4/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-23 18:06:30.000000 pybangla-1.3.4/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:06:30.000000 pybangla-1.3.4/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 18:06:30.000000 pybangla-1.3.4/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 18:06:30.000000 pybangla-1.3.4/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:06:30.886899 pybangla-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 18:06:26.000000 pybangla-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:30.886899 pybangla-1.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-23 18:06:26.000000 pybangla-1.3.4/tests/test.py
```

### Comparing `pybangla-1.3.3/pybangla/module/config.py` & `pybangla-1.3.4/pybangla/module/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,28 +304,28 @@
         "‘": ' ', 
         "”": '"', # won't be replaced
         "`": ' ', 
         ";": " ", 
         ":": " ",  
         "'": " ", 
         "\\": " ", 
-        "-": "-", # won't be replaced
+        # "-": "-", # won't be replaced
         "[": " ", 
         "]": " ", 
         "{": " ", 
         "}": " ", 
         "(": " ", 
         ")": " ", 
         '–': " ", 
         "—": " ", 
         "―": " ", 
         "~": " ",
         "<": " ",
         ">": " ",
-        "/": " ",
+        # "/": " ",
         "�": " ",
         "…": " ",
         "【": " ",
         "】": " ",
         "・": " ",
         "。": " ",
         "『": " ",
```

### Comparing `pybangla-1.3.3/pybangla/module/date_extractor.py` & `pybangla-1.3.4/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.3/pybangla/module/main.py` & `pybangla-1.3.4/pybangla/module/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,62 @@
 
 import re
 import time
 import datetime
+import difflib
 from .config import Config as cfg
 from .parser import DateParser, TextParser, NumberParser, EmojiRemoval
 from .number_parser import Word2NumberMap
 from .date_extractor import DateExtractor
+from .phone_number_extractor import PhoneNumberExtractor
 dp, tp, npr, wnmp, emr = DateParser(), TextParser(), NumberParser(), Word2NumberMap(), EmojiRemoval()
+pne = PhoneNumberExtractor()
 dt = DateExtractor()
 data = cfg.data
 
+class CheckDiff:
+    def __init__(self):
+        pass
+    def diff_text(self, org_text, pro_text):
+        # Split the strings into words
+        org_words, pro_words = org_text.split(),  pro_text.split()
+        # Use difflib to find differences
+        diff = difflib.ndiff(org_words, pro_words)
+        removed_chunk, added_chunk, added_chunks, removed_chunks = [], [], [], []
+        for change in diff:
+            if change.startswith('+ '):
+                added_chunk.append(change[2:])
+                if removed_chunk:
+                    removed_chunks.append(" ".join(removed_chunk))
+                    removed_chunk = []
+            elif change.startswith('- '):
+                removed_chunk.append(change[2:])
+                if added_chunk:
+                    added_chunks.append(" ".join(added_chunk))
+                    added_chunk = []
+            else:
+                if added_chunk:
+                    added_chunks.append(" ".join(added_chunk))
+                    added_chunk = []
+                if removed_chunk:
+                    removed_chunks.append(" ".join(removed_chunk))
+                    removed_chunk = []
+        # Append any remaining chunks
+        if added_chunk:
+            added_chunks.append(" ".join(added_chunk))
+        if removed_chunk:
+            removed_chunks.append(" ".join(removed_chunk))
+        return removed_chunks, added_chunks
+
 class Normalizer:
     def __init__(self):
+        # self.supper()
 
         self.bn_regex = cfg.bn_regex
+        self.cdiff = CheckDiff()
     
     def today(self, language="bn"):
 
         """
         It return today date if may Bangla and English
         
         """
@@ -165,14 +204,24 @@
         formated_date = [self.date_format(i)for i in dates]
         # print(f"Input: {sentence}: Output: {dates}")
         if len(formated_date):
             return formated_date
         else:
             print("No date found")
 
+    def text_diff(self, text1, text2):
+        remove_chunk, add_chunk = self.cdiff.diff_text(text1, text2)
+        return remove_chunk, add_chunk
+    
+    def process_phone_number(self, text):
+
+        text = pne.phn_num_extractor(text)
+
+        return text
+
     
 if __name__ == "__main__":
 
 
     # Testing Date format
     date_list = [
         "০১-এপ্রিল/২০২৩",
```

### Comparing `pybangla-1.3.3/pybangla/module/number_parser.py` & `pybangla-1.3.4/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.3/pybangla/module/parser.py` & `pybangla-1.3.4/pybangla/module/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import datetime
 import string
 from .config import Config as cfg
 from num2words import num2words
 from .date_extractor import DateExtractor
 from fuzzywuzzy import fuzz
 # from bnemo import Translator
-# from .number_parser import Word2NumberMap
+from .phone_number_extractor import PhoneNumberExtractor
 
 
 dt = DateExtractor()
-# nr = Normalizer()
+pne = PhoneNumberExtractor()
 data = cfg.data
 
 _abbreviations = cfg._abbreviations
 _symbols = cfg._symbols
 _ordinal_re = cfg._ordinal_re
 _whitespace_re = cfg._whitespace_re
 _currency = cfg._currency
@@ -29,15 +29,15 @@
 class NumberParser:
     def __init__(self):
         self.english_digits = english_digits
         self.bangla_numeric_words = bangla_numeric_words
         self.en_regex = cfg.en_regex
         self.bn_regex = cfg.bn_regex
 
-    def is_english_digit_string(s):
+    def is_english_digit_string(self, s):
         # Check if all characters in the string are digits (0-9)
         return all(char.isdigit() for char in s)
     
     def contains_only_english(self, input_string):
         # Check if all characters in the string are English (ASCII) characters
         return all(ord(char) < 128 for char in input_string)
 
@@ -239,36 +239,37 @@
         if p in l_p:
             return True
         return False
     
     def number_processing(self, text):
         pattern = r'[\d,\.]+'
         matches = re.findall(pattern, text)
-        for n in matches:
+        sorted_matches = sorted(matches, key=len, reverse=True)
+        for n in sorted_matches:
             p_status = self.check_comma_dot_dari(n)
-
             if p_status:
                 text = text.replace(n, n+" ")
+                # print("p_status : ", text)
             else:
                 status = self.contains_only_english(n)
                 m_re = n.replace(",", "")
                 if status:
+
                     if "." in m_re:
                         bn_m= self.fraction_number_conversion(m_re)
                     else:
                         bn_m= self.number_to_words(self._digit_converter(m_re))
-                    
                     text = text.replace(n, bn_m)
                 else:
                     if "." in m_re:
                         bn_m= self.fraction_number_conversion(m_re, language="bn")
                     else:
                         bn_m= self.number_to_words(m_re)
+                    # print("else : bn_m ", n, bn_m)
                     text = text.replace(n, bn_m)
-
         return text
 
 class DateParser:
     def __init__(self):
         self.samples = cfg.samples
 
         self.npr = NumberParser()
@@ -350,25 +351,27 @@
         return None, None
 
 
     def get_date_indexes(self, date_list):
         """
         Get Date index  
         """
+
+        # print(date_list)
         day, month, year = None, None, None
         for idx, elem in enumerate(date_list):
             if elem.isdigit() and len(elem) == 4:
                 year_idx = idx
                 year = date_list[idx]
                 # print(year)
                 day, month = self.get_day_and_month(year_idx, idx, date_list)
                 # print(day, month)
         return [day, month, year]
     
-    def date_processing(self, date_, language="bn"):
+    def date_processing(self, date_, slash_status=True,language="bn"):
 
         # print(date_)
         if isinstance(date_, list):
             if len(date_):
                 formatted_date = date_
         else:
             split_date = self.data_splitter(date_)
@@ -437,20 +440,27 @@
         self.currency_pattern = r'(?:\$|£|৳|€|¥|₹|₽|₺)?(?:\d+(?:,\d{3})*(?:\.\d+)?|\d+(?:\.\d+)?)'
         self.npr = NumberParser()
         self.dp = DateParser() 
 
     def collapse_whitespace(self, text):
         return re.sub(_whitespace_re, " ", text)
     
+    def phone_number_processing(self):
+        pass
+    
     def exception_year_processing(self, text):
-        _year_with_hyphen = re.findall(r'(\d{4}(?:-|–|—|―)\d{2})', text)
+
+        # if len(text
+        # s+(\d{4}(?:-|–|—|―)\d{2})\s+
+        # _year_with_hyphen = re.findall(r'(\d{4}(?:-|–|—|―)\d{2})', text)
         # print(_year_with_hyphen)
+        _year_with_hyphen = re.findall(r'\s+(\d{4}(?:-|–|—|―)\d{2})\s+', text)
         replce_map = {}
         for year in _year_with_hyphen:
-            # print(year)
+            print("year : ", year)
             rep_year = year.replace('–', '-')
             rep_year = rep_year.replace('—', '-')
             rep_year = rep_year.replace('―', '-')
             four_digit_year, two_digit_year = rep_year.split('-')
             rep_year = self.npr.year_in_number(four_digit_year) + " " + self.npr.number_to_words(two_digit_year)
             text = text.replace(year, rep_year)
         return text
@@ -459,31 +469,37 @@
         
         # https://stackoverflow.com/questions/63256077/how-to-remove-redundant-punctuations-keep-only-the-first-one-in-text
         def my_replace(match): 
             match = match.group()
             return match[0] + (" " if " " in match else "")
 
         _redundent_punc_removal = r"[!\"#$%&\'()*+,\-.\/:;<=>?@\[\\\]^_`।{|}~ ]{2,}"
+        _remove_hyphen_slash = r'(?<!\d)[-/](?!\d)'
+        _remove_comma = r'(?<=\d),(?=\d)'
+        _remove_space_in_punctuations = r'(?<=[^\w\s])\s+(?=[^\w\s])'
         
         text = _STANDARDIZE_ZW.sub('\u200D', text)
         text = re.sub(r'\u200d', '', text)
         text = _DELETE_ZW.sub('', text)
         
         text = text.replace("'র" , " এর")
         text = text.replace("-র" , " এর")
-        text = text.replace("-" , " ")
+        text = text.replace("\uf038" , " ")
         text = text.replace("°F", "° ফারেনহাইট")
         text = text.replace("° F", "° ফারেনহাইট")
         text = text.replace("°C", "° সেলসিয়াস")
         text = text.replace("° C", "° সেলসিয়াস")
-        
-        
-        text = re.sub(r'(?<=[^\w\s])\s+(?=[^\w\s])', '', text) # deleting space between two punctuations
+        text = text.replace("-সালের", " সালের")
+
+        text = re.sub(_remove_space_in_punctuations, '', text) 
         text = re.sub(_redundent_punc_removal, my_replace, text, 0) # only keep the first punctuation
         
+        text = re.sub(_remove_comma, '', text) 
+        text = re.sub(_remove_hyphen_slash, ' ', text)
+        
         translation_table = str.maketrans(_punctuations)
         text = text.translate(translation_table)
         return text
 
 
     def expand_symbols(self, text, lang="bn"):
         for key, replacement in  _symbols[lang]:
@@ -495,24 +511,14 @@
             text = text.replace(key, replacement)
         return text
     
     def expand_position(self, text, lang="bn"):
 
         """
         Replace : 
-            ("১ম", "প্রথম"),
-            ("২য়", "দ্বিতীয়"),
-            ("৩য়", "তৃতীয়"),
-            ("৪র্থ", "চতুর্থ"),
-            ("৫ম","পঞ্চম"),
-            ("৬ষ্ঠ", "ষষ্ঠ"),
-            ("৭ম", "সপ্তম"),
-            ("৮ম", "অষ্টম"),
-            ("৯ম", "নবম"),
-            ("১০ম", "দশম")
         রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম -> রাহিম ক্লাস ওয়ান এ প্রথম, এগারোতম বাইশতম তেত্রিশতম
         
         """
         for regex, replacement in _ordinal_re[lang]:
             text = re.sub(regex, replacement, text)
         if lang=="bn":
             matches = re.findall(r'(\d+)(?:\s*)(?:তম)', text)
@@ -537,15 +543,17 @@
 
 
     def extract_currency_amounts(self, text):
 
         matches = re.findall(self.currency_pattern, text)
         pattern = r'[৳$£€¥₹₽₺]'
 
-        for m in matches:
+        sorted_matches = sorted(matches, key=len, reverse=True)
+
+        for m in sorted_matches:
             currency = re.findall(pattern, m)
             if currency:
                 n_m = m.replace(currency[0], "")
                 n_m = n_m.replace(",", "")
                 language = "en" if self.npr.contains_only_english(n_m) else "bn"
                 if "." in n_m:
                     word = self.npr.fraction_number_conversion(n_m, language=language)
@@ -587,14 +595,16 @@
                     text = text.replace(t[0], t[1])
                 return status, text
             if n_d in self.year_patterns:
                 return True, text
         return False, text
     
     def add_spaces_to_numbers(self, text):
+
+        # print("text : ", text)
         # Define a regular expression pattern to match both Bangla and English digits without spaces around them
         pattern = r'(?<![০-৯0-9])[\u09E6-\u09EF0-9]+(?![০-৯0-9])'
         # Use re.sub to find and replace matches with spaces around them
         result = re.sub(pattern, lambda x: ' ' + x.group(0) + ' ', text)
         # print(result)
         result = " ".join([i for i in result.split(" ") if i.strip()]).strip()
         return result
@@ -602,74 +612,135 @@
 
     def extract_year(self, text):
         pattern = re.findall(self.year_pattern, text)
         for p in pattern:
             text = text.replace(p, f" {p} ")
         return text
     
+    def check_date_format(self, date_string):
+        # Define the regex pattern for English and Bangla digits with slashes or hyphens
+        pattern = r'^[\d০-৯]{1,2}[-/][\d০-৯]{1,2}[-/][\d০-৯]{2}([\d০-৯]{2})?$'
+        
+        # Check if the date string matches the pattern
+        if re.match(pattern, date_string):
+            return True
+        else:
+            return False
+
+    def check_date_format_exception_case(self, date_string):
+        if not self.check_date_format(date_string):
+            return None
+        
+        # Split the date string by either '/' or '-'
+        parts = re.split(r'[-/]', date_string)
+        
+        return parts
+    
+    def english_date_to_bangla_date(self, date_list):
+
+        bn_data_list = []
+        for d_l in date_list:
+            en_digits_status  = self.npr.is_english_digit_string(d_l)
+            if en_digits_status:
+                d_character = []
+                for en_d in d_l:
+                    if en_d in cfg._english2bangla2_digits_mapping:
+                        bn_d = cfg._english2bangla2_digits_mapping[en_d]
+                        d_character.append(bn_d)
+                    else:
+                        d_character.append(en_d)
+                bn_digits = "".join(d_character)
+                bn_data_list.append(bn_digits)
+            else:
+                bn_data_list.append(d_l)
+        # print("bn_data_list : ", bn_data_list)
+        return  bn_data_list
+
+    
     def replance_date_processing(self, text):
         text = self.extract_year(text)
         original_text = text
         r_text = text
         # print("original_text : ", original_text)
         dates = dt.get_dates(text)
 
         # print("dates : ", dates)
         # print("+++++++++++++++++++++++++++ date :++++++++++++++++++++++++", dates)
         for date in dates:
             r_date = date
-            # spanning_position = self.npr.find_word_index(text, date)
-            # print(spanning_position)
-            date = self.add_spaces_to_numbers(date)
-            # print("date:", date)
-            status = True
-            if " " in date:
-                status, text = self.date_formate_validation(date, text)
-            if status:
-                formated_date = self.dp.date_processing(date)
-                original_date = date
-                date_list = [i for i in date.split(" ") if i.strip()]
-                # print(date_list)
+            date_list = self.check_date_format_exception_case(date.strip())
+
+            # print("date_list : ", date_list)
+            if date_list:
+                formated_date = self.dp.date_processing(date_list)
+
+                bn_data_list = self.english_date_to_bangla_date(date_list)
+
+                # print("formated_date : ", formated_date)
+
                 for k, v in formated_date.items():
-                    if v in date_list:
+                    if v in bn_data_list:
+                        # print("v : ", v)
                         key = k if "txt" in k else f"txt_{k}"
-                        index = date_list.index(v)
-                        date_list[index] = formated_date[key]
-
-                process_date = " ".join(date_list).strip()
-                # print("process_date", process_date)
-                if process_date.isdigit():
-                    continue
-                else:
-                    original_text = original_text.replace(r_date, " "+process_date+" ")
-                # search for only year
+                        index = bn_data_list.index(v)
+                        bn_data_list[index] = formated_date[key]
+                process_date = " ".join(bn_data_list).strip()
+                original_text = original_text.replace(r_date, " "+process_date+" ")
+            else:
+                # else:
+                date = self.add_spaces_to_numbers(date)
+                # print("date:", date)
+                status = True
+                if " " in date:
+                    status, text = self.date_formate_validation(date, text)
+                if status:
+                    formated_date = self.dp.date_processing(date)
+                    original_date = date
+                    date_list = [i for i in date.split(" ") if i.strip()]
+                    # print(date_list)
+
+                    # print("formated_date : ", formated_date)
+
+                    bn_data_list = self.english_date_to_bangla_date(date_list)
+                    for k, v in formated_date.items():
+                        if v in bn_data_list:
+                            key = k if "txt" in k else f"txt_{k}"
+                            index = bn_data_list.index(v)
+                            bn_data_list[index] = formated_date[key]
+
+                    process_date = " ".join(bn_data_list).strip()
+                    # print("process_date", process_date)
+                    if process_date.isdigit():
+                        continue
+                    else:
+                        original_text = original_text.replace(r_date, " "+process_date+" ")
+                
         
         _only_years = re.findall(self.year_pattern, original_text)
         # print(_only_years)
         for y in _only_years:
             if y.isdigit():
                 continue
             else:
                 original_text = original_text.replace(y, " " +self.npr.year_in_number(y) + " ")
         return original_text
 
     
 
     def processing(self, text):
         text = self.exception_year_processing(text)
+        text = pne.phn_num_extractor(text)
         text = self.unwanted_puntuation_removing(text)
         text = self.expand_symbols(text)
         text = self.expand_abbreviations(text)
         text = self.expand_position(text)
         text = self.extract_currency_amounts(text)
+        # print(text)
         text = self.replance_date_processing(text)
-        # handel the exception year like 2017-18
-
-        # print("text : ", text)
-        
+        # print(text)
         text = self.npr.number_processing(text)
         text = self.collapse_whitespace(text)
         return text
     
 
 class EmojiRemoval:
```

### Comparing `pybangla-1.3.3/pybangla/module/word_to_number.py` & `pybangla-1.3.4/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.3/pybangla/test.py` & `pybangla-1.3.4/pybangla/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -216,26 +216,48 @@
     # " সাঃ কিমি হাফিক বিডিটি এয়ারলাইনসসহ তিনটি এয়ারলাইনসের ৫১টি কিমি. ফ্লাইটে মোট ২০ হাজার ২৯১ জন হজযাত্রী সৌদি আরবে গেছেন। এ বছর হজ করতে ৮৫ হাজার ২৫৭ জনের সৌদি আরবে যাওয়ার কথা রয়েছে। ৫ম",
     # "প্রদর্শনীটি চলার কথা ছিল ১২ মে পর্যন্ত, তবে দর্শকদের ব্যাপক আগ্রহের কারণে তিন দিন সময় বাড়িয়ে ১৫ মে পর্যন্ত করা হয়েছিল ১৫.১৫",
     # "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45",
     # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে"
     # ]
 
     # # solving steps is have number need to give extra space both side
+    # issue = [
+    # # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে.",
+    # # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    # # "আজকের তাপমাত্রা ৪৪°F",
+    # # "আজকের তাপমাত্রা ৪৪°C",
+    # # "যেমন ১৯৬১ সালে দেশটির তৎকালীন প্রেসিডেন্ট ডোয়াইট ডি আইজেনহাওয়ার শিক্ষা খাতে সামরিক শিল্পের প্রবেশের বিপদ নিয়ে সতর্ক করেছিলেন।",
+    # # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    # "উদাহরণস্বরূপ, আপনার মোটরযানের রেজিস্ট্রেশন নাম্বার ঢাকা মেট্রো-গ-12-1212 এবং টাকা জমা রশিদের ট্রানজেকশন নাম্বার 2001011325989"
+    # ]
+
     issue = [
-    # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে.",
+    "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে. 2023-24",
     # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
     # "আজকের তাপমাত্রা ৪৪°F",
     # "আজকের তাপমাত্রা ৪৪°C",
     # "যেমন ১৯৬১ সালে দেশটির তৎকালীন প্রেসিডেন্ট ডোয়াইট ডি আইজেনহাওয়ার শিক্ষা খাতে সামরিক শিল্পের প্রবেশের বিপদ নিয়ে সতর্ক করেছিলেন।",
-    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
-    "উদাহরণস্বরূপ, আপনার মোটরযানের রেজিস্ট্রেশন নাম্বার ঢাকা মেট্রো-গ-12-1212 এবং টাকা জমা রশিদের ট্রানজেকশন নাম্বার 2001011325989"
+    "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    # " বাংলাদেশের পাসপোর্টের অভ্যন্তরে ইস্যু করানোর সময়ে নিয়মিত, জরুরী, এবং অতীব জরুরী বিতরণের ফি নিম্নলিখিত: নিয়মিত বিতরণ (48 পৃষ্ঠা এবং 10 বছর মেয়াদ) পাসপোর্ট ফি: ৪,০২৫ টাকা জরুরী বিতরণ (48 পৃষ্ঠা এবং 10 বছর মেয়াদ) পাসপোর্ট ফি: ৬,৩২৫ টাকা অতীব জরুরী বিতরণ (48 পৃষ্ঠা এবং 10 বছর মেয়াদ) পাসপোর্ট ফি: ৮,৬২৫ টাকা নিয়মিত বিতরণ (64 পৃষ্ঠা এবং 5 বছর মেয়াদ) পাসপোর্ট ফি: ৫,৭৫০ টাকা জরুরী বিতরণ (64 পৃষ্ঠা এবং 5 বছর মেয়াদ) পাসপোর্ট ফি: ৮,০৫০ টাকা অতীব জরুরী বিতরণ (64 পৃষ্ঠা এবং 5 বছর মেয়াদ) পাসপোর্ট ফি: ১০,৩৫০ টাকা",
+    "বাংলাদেশের পাসপোর্টের অভ্যন্তরে ইস্যু করানোর সময় 10/12/1956",
+    # "৬/৯/১৯৯৬ বাংলাদেশের পাসপোর্টের অভ্যন্তরে ইস্যু করানোর সময় 10/12/24",
+    "ডিজিটাল রেজিস্ট্রেশন সার্টিফিকেট সংক্রান্ত যোগাযোগ করতে হলে 01790-540211 অথবা 01790-540210 নম্বরে যোগাযোগ করতে হবে 01790540211",
+    "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
+    # "অর্থাৎ, আবেদনকারীর বয়স ১ বছর হলে জন্ম নিবন্ধন ফি ১০ টাকা, বয়স ২ বছর হলে ২০ টাকা, বয়স ৫ বছর হলে ৫০ টাকা, এবং বয়স ১০ বছর হলে ১০০ টাকা হবে",
+    # "বাংলাদেশের পাসপোর্টের ৪৮ পৃষ্ঠা এবং ১০ বছর মেয়াদের সহ পাসপোর্টের জন্য নিয়মিত বিতরণে ফি ৫,৭৫০ টাকা, জরুরী বিতরণে ফি ৮,০৫০ টাকা, এবং অতীব জরুরী বিতরণের ফি ১০,৩৫০ টাকা",
+    # "বাংলাদেশের পাসপোর্টের ৬৪ পৃষ্ঠা এবং ৫ বছর মেয়াদের সহ পাসপোর্টের জন্য নিয়মিত বিতরণে ফি ৬,৩২৫ টাকা, জরুরী বিতরণে ফি ৮,৬২৫ টাকা, এবং অতীব জরুরী বিতরণের ফি ১২,০৭৫ টাকা"
     ]
 
 
 
     for i in issue:
 
         print("input : ", i)
         text = nrml.text_normalizer(i)
         print("output : ", text)
+        print(nrml.text_diff(i, text))
+        # print()
         print("+"*40)
 
+    number_string = nrml.process_phone_number("01790-540211")
+    print(number_string)
+
```

### Comparing `pybangla-1.3.3/setup.py` & `pybangla-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.3.3',
+    version='1.3.4',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.3.3/tests/test.py` & `pybangla-1.3.4/tests/test.py`

 * *Files identical despite different names*

