# Comparing `tmp/lanQ-1.4.3.tar.gz` & `tmp/lanQ-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.4.3.tar", last modified: Thu May  9 02:37:48 2024, max compression
+gzip compressed data, was "lanQ-1.4.4.tar", last modified: Thu May 23 07:46:27 2024, max compression
```

## Comparing `lanQ-1.4.3.tar` & `lanQ-1.4.4.tar`

### file list

```diff
@@ -1,23 +1,41 @@
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-09 02:37:48.803319 lanQ-1.4.3/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     7759 2024-04-30 06:59:30.000000 lanQ-1.4.3/README.md
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ.egg-info/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      400 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       10 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.3/lanQ_rule/__init__.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/base_func/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:11:32.000000 lanQ-1.4.3/lanQ_rule/base_func/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-04-26 08:10:06.000000 lanQ-1.4.3/lanQ_rule/base_func/base.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15682 2024-05-09 02:36:54.000000 lanQ-1.4.3/lanQ_rule/common_rule.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/config/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 05:56:14.000000 lanQ-1.4.3/lanQ_rule/config/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2294 2024-04-19 03:19:55.000000 lanQ-1.4.3/lanQ_rule/config/const.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-04-30 03:33:52.000000 lanQ-1.4.3/lanQ_rule/config/customize.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1872 2024-05-06 06:02:00.000000 lanQ-1.4.3/lanQ_rule/config/rule_map.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      991 2024-04-30 03:33:53.000000 lanQ-1.4.3/lanQ_rule/model_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1153 2024-04-24 03:44:27.000000 lanQ-1.4.3/lanQ_rule/prompt_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-05-09 02:37:48.803319 lanQ-1.4.3/setup.cfg
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-05-09 02:37:07.000000 lanQ-1.4.3/setup.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-23 07:46:27.812489 lanQ-1.4.4/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     9785 2024-05-20 03:00:14.000000 lanQ-1.4.4/README.md
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/convert/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      574 2024-05-22 10:16:37.000000 lanQ-1.4.4/convert/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      324 2024-05-22 10:18:04.000000 lanQ-1.4.4/convert/alpaca.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      300 2024-05-22 07:06:56.000000 lanQ-1.4.4/convert/audio_ar.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      357 2024-05-21 05:51:01.000000 lanQ-1.4.4/convert/json_file.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      305 2024-05-21 08:02:04.000000 lanQ-1.4.4/convert/json_line.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      291 2024-05-21 05:47:42.000000 lanQ-1.4.4/convert/string_line.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ.egg-info/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      779 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       29 2024-05-23 07:46:27.000000 lanQ-1.4.4/lanQ.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_model/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_model/__init__.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_model/base_func/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_model/base_func/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15911 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/base.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15517 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/base_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     8630 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/openai_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     5611 2024-05-10 05:37:15.000000 lanQ-1.4.4/lanQ_model/base_func/turbomind_api.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1528 2024-05-22 07:08:13.000000 lanQ-1.4.4/lanQ_model/gpt.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2757 2024-05-21 02:45:55.000000 lanQ-1.4.4/lanQ_model/llama3.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2104 2024-05-20 08:56:37.000000 lanQ-1.4.4/lanQ_model/perspective.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.808490 lanQ-1.4.4/lanQ_rule/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.4/lanQ_rule/__init__.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/lanQ_rule/base_func/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:11:32.000000 lanQ-1.4.4/lanQ_rule/base_func/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-04-26 08:10:06.000000 lanQ-1.4.4/lanQ_rule/base_func/base.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    14875 2024-05-22 08:18:06.000000 lanQ-1.4.4/lanQ_rule/common_rule.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-23 07:46:27.812489 lanQ-1.4.4/lanQ_rule/config/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-20 06:41:14.000000 lanQ-1.4.4/lanQ_rule/config/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1852 2024-05-20 06:52:10.000000 lanQ-1.4.4/lanQ_rule/config/const.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-04-30 03:33:52.000000 lanQ-1.4.4/lanQ_rule/config/customize.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1117 2024-05-20 06:09:13.000000 lanQ-1.4.4/lanQ_rule/config/rule_map.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      902 2024-05-20 06:54:36.000000 lanQ-1.4.4/lanQ_rule/model_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1040 2024-05-20 06:54:36.000000 lanQ-1.4.4/lanQ_rule/prompt_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-05-23 07:46:27.812489 lanQ-1.4.4/setup.cfg
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-05-23 07:46:01.000000 lanQ-1.4.4/setup.py
```

### Comparing `lanQ-1.4.3/lanQ_rule/base_func/base.py` & `lanQ-1.4.4/lanQ_rule/base_func/base.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.3/lanQ_rule/common_rule.py` & `lanQ-1.4.4/lanQ_rule/common_rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 import textstat
 from hanziconv import HanziConv
 
 sys.path.append(os.path.dirname(__file__))
 
 import lanQ_rule.config.customize as cm
 from lanQ_rule.base_func.base import *
-from lanQ_rule.config.const import *
 
 def common_anti_crawler_zh(content: str) -> dict:
     """from lvkai"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     line_num = 50
     content_lines = [l.strip() for l in content.split("\n") if len(l.strip())]
     max_jieba_ratio = 0
     for line in content_lines:
         line = get_real_text(line)
         char_num = len(line)
         word_num = 0
@@ -25,68 +24,64 @@
             seg_list = jieba.cut(line, cut_all=True)
             for word in seg_list:
                 if len(word) == 1:
                     word_num += 1
             max_jieba_ratio = max(max_jieba_ratio, word_num / char_num)
     if max_jieba_ratio > cm.common_anti_crawler_zh['threshold']:
         res["error_status"] = True
-        res["error_type"] = ERROR_CRAWL_ANTI
         res["error_reason"] = "包含反爬文本"
     return res
 
 def common_bracket_unmatch(content: str) -> dict:
     """check whether bracket matches"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     bracket_types = [("[", "]"), ("{", "}"), ("【", "】"), ("《", "》")]
     for open_bracket, close_bracket in bracket_types:
         if content.count(open_bracket) != content.count(close_bracket):
             res["error_status"] = True
-            res["error_type"] = ERROR_BRACKET_UNMATCH
             res["error_reason"] = "括号数量不一致"
     return res
 
 def common_chaos_en(content: str) -> dict:
     """check whether content has English messy code"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     af_en = delete_punc_en(content)
     af_ch = delte_punc_ch(af_en)
     str_len = len(af_ch)
     language = langid.classify(content)[0]
     if language == "en":
         seg_len = len(list(jieba.cut(af_ch)))
         if str_len == 0 or seg_len == 0 or get_tokens(content, language) < 50:
             return res
         if str_len / seg_len > 1.2:
             return res
         else:
             res["error_status"] = True
-            res["error_type"] = ERROR_CHAOS_EN
             res["error_reason"] = '英文乱码'
             return res
     else:
         return res
 
 def common_chaos_symbol(content: str) -> dict:
     """check whether content has a lot of meaningless words"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r'[0-9a-zA-Z\u4e00-\u9fa5]'
     s = re.sub(pattern, '', content)
     str_len = len(content)
     symbol_len = len(s)
     if str_len == 0 or symbol_len == 0:
         return res
     if symbol_len / str_len > 0.5:
         res["error_status"] = True
-        res["error_type"] = ERROR_CHAOS_SYMBOL
         res['error_reason'] = '大量非正文内容'
     return res
 
 def common_chaos_zh(content: str) -> dict:
     """check whether content has Chinese messy code"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     lan = langid.classify(content)[0]
     if lan != 'zh':
         return res
     s = normalize(content)
     pattern = r'[a-zA-Zāáǎàēéěèīíǐìōóǒòūúǔùǖǘǚǜ\n\s]'
     s = re.sub(pattern, '', s)
     s_simplified = HanziConv.toSimplified(s)
@@ -94,63 +89,58 @@
     seg_len = len(list(jieba.cut(s_simplified)))
     num_bytes = len(content.encode('utf-8'))
     tokens_len = int(num_bytes * 0.248)
     if str_len == 0 or seg_len == 0 or tokens_len < 50:
         return res
     if str_len / seg_len <= 1.1:
         res["error_status"] = True
-        res["error_type"] = ERROR_CHAOS_ZH
         res['error_reason'] = '中文乱码'
     return res
 
 def common_check_photo(content: str) -> dict:
     """check whether content has photo"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = '!\[\]\(http[s]?://.*?jpeg "\n"\)'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_CHECK_PHOTO
         res['error_reason'] = matches
     return res
 
 def common_colon_end(content: str) -> dict:
     """check whether the last char is ':'"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     if len(content) <= 0:
         return res
     if content[-1] == ':':
         res['error_status'] = True
-        res['error_type'] = ERROR_RULE_COLON_END
         res['error_reason'] = '冒号结尾'
     return res
 
 def common_content_null(content: str) -> dict:
     """check whether content is null"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     count = len(content.strip())
     if count == 0:
         res["error_status"] = True
-        res["error_type"] = ERROR_CONTENT_NULL
         res['error_reason'] = '内容为空'
     return res
 
 def common_doc_repeat(content: str) -> dict:
     """check whether content repeats"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     repeat_score = base_rps_frac_chars_in_dupe_ngrams(6, content)
     if repeat_score >= 80:
         res["error_status"] = True
-        res["error_type"] = ERROR_DOC_REPEAT
         res['error_reason'] = '文本重复度过高： ' + str(repeat_score)
     return res
 
 def common_ellipsis_ratio(content: str) -> dict:
     """check whether ratio of lines end with ellipsis is bigger than 75%"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     lines = content.split("\n")
     non_empty_lines = 0
     ellipsis_lines = 0
     for line in lines:
         if line.strip() != "":
             non_empty_lines += 1
             if (
@@ -160,57 +150,53 @@
                 or line.strip().endswith("……")
             ):
                 ellipsis_lines += 1
     if non_empty_lines != 0:
         ellipsis_ratio = ellipsis_lines / non_empty_lines
         if ellipsis_ratio >0.75:
             res["error_status"] = True
-            res['error_type'][ERROR_ELLIPSIS_RATIO] = ERROR_ELLIPSIS_RATIO
-            res["error_reason"][ERROR_ELLIPSIS_RATIO] = "省略号结尾行占比超过75%" 
+            res["error_reason"] = "省略号结尾行占比超过75%"
     return res
 
 def common_emoj_characters(content: str) -> dict:
     """check whether content contains emoji charactors"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     emoj_chars_pattern = r"U\+26[0-F][0-D]|U\+273[3-4]|U\+1F[3-6][0-4][0-F]|U\+1F6[8-F][0-F]"
     matches = re.search(emoj_chars_pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_EMOJ_CHAR
         res["error_reason"] = "包含emoji符号"
     return res
 
 def common_enter_more(content: str) -> dict:
     """check whether content has more than 8 continious enter"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r'\n{8,}|\r{8,}'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_ENTER_MORE
         res['error_reason'] = '存在连续8个回车'
     return res
 
 def common_enter_ratio_more(content: str) -> dict:
     """check whether enter / content is more than 25%"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     enter_count = content.count('\n')
     count = len(content)
     if count == 0:
         return res
     ratio = enter_count / count * 100
     if ratio >= 25:
         res["error_status"] = True
-        res["error_type"] = ERROR_ENTER_RATIO_MORE
         res['error_reason'] = '回车超过正文25%'
     return res
 
 def common_html_entity(content: str) -> dict:
     """check whether content has html entity"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     entities = [
         "nbsp",
         "lt",
         "gt",
         "amp",
         "quot",
         "apos",
@@ -237,192 +223,180 @@
     # maked_entities = [f"{entity}" for entity in entities]
     all_entities = full_entities + half_entities
 
     pattern = '|'.join(all_entities)
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_HTML_ENTITY
         res['error_reason'] = matches
     return res
 
 def common_img_html_tag(content: str) -> dict:
     """check whether content has img or html tag"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r"(<img[^>]*>)|<p[^>]*>(.*?)<\/p>|<o:p[^>]*>(.*?)<\/o:p>"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_IMG_HTML_TAG
         res['error_reason'] = matches
     return res
 
 def common_invalid_web(content: str) -> dict:
     """check whether the content is invalid"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     invalid_list = ["404 - Page not found\nThe requested page does not exist (or has been deleted).\nIf you typed a URL by hand, or used a bookmark, please double check the address that you used.\nIf you see this page, and the error persists, please contact Customer Care and provide details about the action you tried to perform."]
     for item in invalid_list:
         if item in content:
             res["error_status"] = True
-            res["error_type"] = ERROR_INVALID_WEB
             res["error_reason"] = "content内容为404"
     return res
 
 def common_invisible_char(content: str) -> dict:
     """check whether content has invisible char"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r"[\u2000-\u200F\u202F\u205F\u3000\uFEFF\u00A0\u2060-\u206F\uFEFF\xa0]"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_INVISIBLE_CHAR
         res['error_reason'] = matches
     return res
 
 def common_joint_special_symbol(content: str) -> dict:
     """check if there are special symbols composed of multiple symbols spliced together"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r"&#247;|\? :"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_JOINT_SPECIAL_SYMBOL
         res["error_reason"] = "包含多个符号拼接组成的特殊符号"
     return res
 
 def common_language_mixed(content: str) -> dict:
     """check whether content is mixed in Chinese and English"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     s = normalize(content)
     en_len = len(re.findall(r'[a-zA-Z]', s))
     zh_len = len(re.findall(r'[\u4e00-\u9fa5]', s))
     count_len = len(s)
     if count_len == 0:
         return res
     if en_len / count_len >= 0.5 and zh_len / count_len >= 0.1:
         res["error_status"] = True
-        res["error_type"] = ERROR_LANGUAGE_MIXED
         res['error_reason'] = '中英文混杂'
     return res
 
 def common_license_key(content: str) -> dict:
     """check if the content contains license key"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     # 定义三个模式对应于上述的三种格式
     pattern = r"(License|破解)|" + "|".join([
     "[A-Z0-9]{47}",  # 字母数字混合
     "[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}",  # 分段的字母数字混合
     "[A-Z0-9]{4}-\d{8}-[A-Z0-9]{4}"  # 含有特定信息的许可证密钥，例如产品ID和购买日期
     ])
     match = re.search(pattern, content, re.I)  # re.I使匹配对大小写不敏感
     if match:
         res["error_status"] = True
-        res["error_type"] = ERROR_LICENSE_KEY
         res["error_reason"] = "包含license key"
     return res
 
 def common_no_punc(content: str) -> dict:
     """check whether content has paragraph without punctuations"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     paragraphs = content.split('\n')
     max_word_count = 0
     for paragraph in paragraphs:
         if len(paragraph) == 0:
             continue
         sentences = re.split(r'[-–.!?,;•、。！？，；·]', paragraph)
         for sentence in sentences:
             words = sentence.split()
             word_count = len(words)
             if word_count > max_word_count:
                 max_word_count = word_count
     text_stat_res = textstat.flesch_reading_ease(content)
     if int(max_word_count) > 56 and text_stat_res < 20:
         res["error_status"] = True
-        res["error_type"] = ERROR_NO_PUNC
         res['error_reason'] = '段落无标点'
     return res
 
 def common_space_more(content: str) -> dict:
     """check whether content has more than 500 consecutive spaces"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r' {500,}'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_SPACE_MORE
         res['error_reason'] = '存在连续500个空格'
     return res
 
 def common_special_character(content: str) -> dict:
-    res = {'error_status': False}
-    pattern = r"[�□\^]|\{\/U\}"
+    res = {'error_status': False, 'error_reason': ''}
+    pattern = r"[�□]|\{\/U\}"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_SPECIAL_CHARACTER
         res['error_reason'] = matches
     return res
 
 def common_special_mark(content: str) -> dict:
     """check if the content contains special mark"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r'keyboard_arrow_(left|right)'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_SPECIAL_MARK
         res["error_reason"] = "元素包含特殊标记"
     return res
 
 def common_unconverted_symbol(content: str) -> dict:
     """check if the content contains special symbols for conversion failure"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     pattern = r'u200e'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_UNCONVERTED_SYMBOL
         res["error_reason"] = "包含转换失败的特殊符号"
     return res
 
 def common_underscore_length(content: str) -> dict:
     """check whether the content contains underscores whose length is longer than 15"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     max_underscore_count = 0
     for char in content:
         if char == '_':
             underscore_count += 1
             if underscore_count > max_underscore_count:
                 max_underscore_count = underscore_count
         else:
             underscore_count = 0
     if max_underscore_count >= 15:
         res["error_status"] = True
-        res["error_type"] = ERROR_UNDERSCORE_LENGTH
         res["error_reason"] = "下划线长度大于15"
     return res
 
 def common_url_only(content: str) -> dict:
     """check whether content is all urls"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
+    if len(content.strip()) == 0:
+        return res
+
     pattern = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'  # noqa
     s = re.sub(pattern, '', content)
     count = len(s.strip())
     if count == 0:
         res["error_status"] = True
-        res["error_type"] = ERROR_URL_ONLY
         res['error_reason'] = '内容只有url'
     return res
 
 def common_word_stuck(content: str) -> dict:
     """check whether words are stuck"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     words = re.findall(r'[a-zA-Z]+', content)
     max_word_len = 0
     for word in words:
         if len(word) > max_word_len:
             max_word_len = len(word)
     if max_word_len > 45:
         res["error_status"] = True
-        res["error_type"] = ERROR_WORD_STUCK
         res['error_reason'] = '英文单词黏连'
     return res
```

### Comparing `lanQ-1.4.3/lanQ_rule/model_rule.py` & `lanQ-1.4.4/lanQ_rule/model_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import os
 import sys
 
 sys.path.append(os.path.dirname(__file__))
 
 import lanQ_rule.config.customize as cm
 from lanQ_rule.base_func.base import *
-from lanQ_rule.config.const import *
 
 def model_advertisement(content: str) -> dict:
     """check whether content has advertisement"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     ad_list_en = ['deadlinesOrder', 'Kindly click on ORDER NOW to receive an']
     matches = re.findall('|'.join(ad_list_en), content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_ADVERTISEMENT
         res['error_reason'] = matches
     return res
 
 def model_watermark(content: str) -> dict:
     """check whether content has watermark"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     watermark_list = cm.model_watermark['key_list']
     matches = re.findall('|'.join(watermark_list), content)
     if matches:
         res["error_status"] = True
-        res["error_type"] = ERROR_WATERMARK
         res['error_reason'] = '存在水印'
     return res
```

### Comparing `lanQ-1.4.3/lanQ_rule/prompt_rule.py` & `lanQ-1.4.4/lanQ_rule/prompt_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import os
 import sys
 import langid
 
 sys.path.append(os.path.dirname(__file__))
 
 from lanQ_rule.base_func.base import *
-from lanQ_rule.config.const import *
 
 def prompt_chinese_produce_english(prompt: str, prediction: str) -> dict:
     """check whether chinese prompt produce english prediction"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     lan_prompt = langid.classify(prompt)[0]
     lan_prediction = langid.classify(prediction)[0]
     if lan_prompt == 'zh' and lan_prediction == 'en':
         res['error_status'] = True
-        res['error_type'] = ERROR_CHINESE_PRODUCE_ENGLISH
         res['error_reason'] = '中文提示，生成英文内容'
     return res
 
 def prompt_english_produce_chinese(prompt: str, prediction: str) -> dict:
     """check whether english prompt produce chinese prediction"""
-    res = {'error_status': False}
+    res = {'error_status': False, 'error_reason': ''}
     lan_prompt = langid.classify(prompt)[0]
     lan_prediction = langid.classify(prediction)[0]
     if lan_prompt == 'en' and lan_prediction == 'zh':
         res['error_status'] = True
-        res['error_type'] = ERROR_ENGLISH_PRODUCE_CHINESE
         res['error_reason'] = '英文提示，生成中文内容'
     return res
```

