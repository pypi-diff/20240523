# Comparing `tmp/PMPrimer-1.0.6.tar.gz` & `tmp/pmprimer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PMPrimer-1.0.6.tar", last modified: Wed Apr 10 14:48:43 2024, max compression
+gzip compressed data, was "pmprimer-1.0.7.tar", last modified: Thu May 23 03:00:56 2024, max compression
```

## Comparing `PMPrimer-1.0.6.tar` & `pmprimer-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.408625 PMPrimer-1.0.6/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1087 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/LICENSE
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       22 2024-04-10 14:04:14.000000 PMPrimer-1.0.6/MANIFEST.in
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-04-10 14:48:43.392596 PMPrimer-1.0.6/PKG-INFO
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.376972 PMPrimer-1.0.6/PMPrimer.egg-info/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/PKG-INFO
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      502 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/SOURCES.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)        1 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/dependency_links.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       51 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/entry_points.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       47 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/requires.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)        6 2024-04-10 14:48:42.000000 PMPrimer-1.0.6/PMPrimer.egg-info/top_level.txt
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10176 2023-10-14 05:24:11.000000 PMPrimer-1.0.6/README.md
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.187999 PMPrimer-1.0.6/piece/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      211 2024-04-10 14:30:05.000000 PMPrimer-1.0.6/piece/__auxiliary__.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)       15 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/__init__.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    11218 2024-04-10 14:24:08.000000 PMPrimer-1.0.6/piece/piecebase.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     9104 2023-10-14 05:58:30.000000 PMPrimer-1.0.6/piece/piecedataprogress.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1328 2023-10-13 16:04:55.000000 PMPrimer-1.0.6/piece/piecedefine.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10894 2023-11-06 07:57:09.000000 PMPrimer-1.0.6/piece/piecedesign.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    19300 2024-04-10 14:22:33.000000 PMPrimer-1.0.6/piece/pieceevaluate.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)    31580 2023-10-14 04:58:49.000000 PMPrimer-1.0.6/piece/piecemain.py
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)     6819 2023-09-06 06:58:05.000000 PMPrimer-1.0.6/piece/piecentry.py
-drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-04-10 14:48:43.314145 PMPrimer-1.0.6/piece/static/
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)  2920768 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/static/muscle5.1.linux_intel64
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)   832512 2023-07-20 05:53:27.000000 PMPrimer-1.0.6/piece/static/muscle5.1.win64.exe
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      547 2024-04-10 14:48:43.410734 PMPrimer-1.0.6/setup.cfg
--rwxrwxrwx   0 youngers  (1000) youngers  (1000)      836 2024-04-10 14:30:04.000000 PMPrimer-1.0.6/setup.py
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-05-23 03:00:56.082905 pmprimer-1.0.7/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1087 2023-07-20 05:53:27.000000 pmprimer-1.0.7/LICENSE
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       22 2024-04-10 14:04:14.000000 pmprimer-1.0.7/MANIFEST.in
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-05-23 03:00:56.072372 pmprimer-1.0.7/PKG-INFO
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-05-23 03:00:56.052263 pmprimer-1.0.7/PMPrimer.egg-info/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10805 2024-05-23 03:00:54.000000 pmprimer-1.0.7/PMPrimer.egg-info/PKG-INFO
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      502 2024-05-23 03:00:55.000000 pmprimer-1.0.7/PMPrimer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)        1 2024-05-23 03:00:54.000000 pmprimer-1.0.7/PMPrimer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       51 2024-05-23 03:00:54.000000 pmprimer-1.0.7/PMPrimer.egg-info/entry_points.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       47 2024-05-23 03:00:54.000000 pmprimer-1.0.7/PMPrimer.egg-info/requires.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)        6 2024-05-23 03:00:54.000000 pmprimer-1.0.7/PMPrimer.egg-info/top_level.txt
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10176 2023-10-14 05:24:11.000000 pmprimer-1.0.7/README.md
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-05-23 03:00:55.834462 pmprimer-1.0.7/piece/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      211 2024-05-23 02:55:05.000000 pmprimer-1.0.7/piece/__auxiliary__.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)       15 2023-07-20 05:53:27.000000 pmprimer-1.0.7/piece/__init__.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    11431 2024-05-23 02:51:41.000000 pmprimer-1.0.7/piece/piecebase.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     9104 2023-10-14 05:58:30.000000 pmprimer-1.0.7/piece/piecedataprogress.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     1328 2023-10-13 16:04:55.000000 pmprimer-1.0.7/piece/piecedefine.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    10894 2023-11-06 07:57:09.000000 pmprimer-1.0.7/piece/piecedesign.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    19300 2024-04-10 14:22:33.000000 pmprimer-1.0.7/piece/pieceevaluate.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)    31580 2023-10-14 04:58:49.000000 pmprimer-1.0.7/piece/piecemain.py
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)     6819 2023-09-06 06:58:05.000000 pmprimer-1.0.7/piece/piecentry.py
+drwxrwxrwx   0 youngers  (1000) youngers  (1000)        0 2024-05-23 03:00:55.987095 pmprimer-1.0.7/piece/static/
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)  2920768 2023-07-20 05:53:27.000000 pmprimer-1.0.7/piece/static/muscle5.1.linux_intel64
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)   832512 2023-07-20 05:53:27.000000 pmprimer-1.0.7/piece/static/muscle5.1.win64.exe
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      547 2024-05-23 03:00:56.094910 pmprimer-1.0.7/setup.cfg
+-rwxrwxrwx   0 youngers  (1000) youngers  (1000)      836 2024-05-23 02:55:27.000000 pmprimer-1.0.7/setup.py
```

### Comparing `PMPrimer-1.0.6/LICENSE` & `pmprimer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/PKG-INFO` & `pmprimer-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PMPrimer
-Version: 1.0.6
+Version: 1.0.7
 Summary: automated design of multiplex PCR primer pairs for diverse templates
 Home-page: https://github.com/AGIScuipeng/PMPrimer
 Author: Nerium
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `PMPrimer-1.0.6/PMPrimer.egg-info/PKG-INFO` & `pmprimer-1.0.7/PMPrimer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PMPrimer
-Version: 1.0.6
+Version: 1.0.7
 Summary: automated design of multiplex PCR primer pairs for diverse templates
 Home-page: https://github.com/AGIScuipeng/PMPrimer
 Author: Nerium
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `PMPrimer-1.0.6/README.md` & `pmprimer-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/piecebase.py` & `pmprimer-1.0.7/piece/piecebase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 创建人员: Nerium
 创建日期: 2022/08/31
 更改人员: Nerium
-更改日期: 2024/04/10
+更改日期: 2024/05/22
 '''
 
 from .piecedefine import *
 
 from collections import Counter
 import primer3
 import math
@@ -294,26 +294,29 @@
 
     return ret, [seq[0] for seq in sort_seqs[:retidx]]
 
 '''
 创建人员: Nerium
 创建日期: 2023/03/02
 更改人员: Nerium
-更改日期: 2023/03/02
+更改日期: 2024/05/22
 '''
 #把bps简并序列列出所有可能性
 def generate_all(bps, idx) :
+    #没有简并引物
+    if len(bps) == 0 : return []
+    #递归结束条件
     if len(bps)-1 == idx : return GENE_RELEASE[bps[idx]]
     return [rep+bpi for rep in GENE_RELEASE[bps[idx]] for bpi in generate_all(bps, idx+1)]
 
 '''
 创建人员: Nerium
 创建日期: 2023/03/02
 更改人员: Nerium
-更改日期: 2023/03/02
+更改日期: 2024/05/22
 '''
 #挑选出简并位点找到所有可能，再替换出原始序列
 def generate_rep(bps, reverse=False) :
     gall = ''
     for idx in range(len(bps)) :
         if bps[idx] not in DEFAULT_DNA_SINGLE_LIST : gall += bps[idx]
     
@@ -324,14 +327,18 @@
         tidx, tbps = 0, ''
         for idx in range(len(bps)) :
             if bps[idx] not in DEFAULT_DNA_SINGLE_LIST : tbps += rep[tidx]; tidx += 1
             else : tbps += bps[idx]
 
         res_list.append(tbps)
 
+    #如果没有简并引物，那么只有一条引物，加入结果即可
+    if len(rall) == 0 :
+        res_list.append(bps)
+
     if reverse : return [''.join(DEFAULT_DNA_REFLECT_DICT[bp] for bp in res[::-1]) for res in res_list]
     return res_list
 
 '''
 创建人员: Nerium
 创建日期: 2022/08/31
 更改人员: Nerium
```

### Comparing `PMPrimer-1.0.6/piece/piecedataprogress.py` & `pmprimer-1.0.7/piece/piecedataprogress.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/piecedefine.py` & `pmprimer-1.0.7/piece/piecedefine.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/piecedesign.py` & `pmprimer-1.0.7/piece/piecedesign.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/pieceevaluate.py` & `pmprimer-1.0.7/piece/pieceevaluate.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/piecemain.py` & `pmprimer-1.0.7/piece/piecemain.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/piecentry.py` & `pmprimer-1.0.7/piece/piecentry.py`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/static/muscle5.1.linux_intel64` & `pmprimer-1.0.7/piece/static/muscle5.1.linux_intel64`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/piece/static/muscle5.1.win64.exe` & `pmprimer-1.0.7/piece/static/muscle5.1.win64.exe`

 * *Files identical despite different names*

### Comparing `PMPrimer-1.0.6/setup.cfg` & `pmprimer-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PMPrimer
-version = 1.0.6
+version = 1.0.7
 author = Nerium
 long_description = file: README.md # 从文件中读取
 license = MIT
 url = 'https://github.com/AGIScuipeng/PMPrimer'
 classifiers = 
 	Environment :: Console
 	Operating System :: Microsoft :: Windows
```

### Comparing `PMPrimer-1.0.6/setup.py` & `pmprimer-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PMPrimer",
-    version="1.0.6",
+    version="1.0.7",
     author="Nerium",
     description="automated design of multiplex PCR primer pairs for diverse templates",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AGIScuipeng/PMPrimer",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

