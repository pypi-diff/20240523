# Comparing `tmp/dspawpy-1.3.0.tar.gz` & `tmp/dspawpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.3.0.tar", last modified: Fri May 17 09:31:09 2024, max compression
+gzip compressed data, was "dspawpy-1.3.1.tar", last modified: Thu May 23 06:52:09 2024, max compression
```

## Comparing `dspawpy-1.3.0.tar` & `dspawpy-1.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.927343 dspawpy-1.3.0/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1055 2024-05-16 07:21:06.000000 dspawpy-1.3.0/LICENSE.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13057 2024-05-17 09:31:09.926342 dspawpy-1.3.0/PKG-INFO
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    12869 2024-05-17 02:08:20.000000 dspawpy-1.3.0/README.md
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.894337 dspawpy-1.3.0/dspawpy/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      727 2024-05-17 09:31:08.000000 dspawpy-1.3.0/dspawpy/__init__.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.905368 dspawpy-1.3.0/dspawpy/analysis/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/analysis/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30293 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/analysis/aimdtools.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17645 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/analysis/vacf.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.910338 dspawpy-1.3.0/dspawpy/cli/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/cli/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    47124 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/aux.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     8493 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/cli.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17882 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/cli/menu_prompts.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.915337 dspawpy-1.3.0/dspawpy/diffusion/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/diffusion/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     3551 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/neb.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63167 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/nebtools.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    10751 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/diffusion/pathfinder.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.923341 dspawpy-1.3.0/dspawpy/io/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.0/dspawpy/io/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63584 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/read.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    26571 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/structure.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30750 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/utils.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    27382 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/io/write.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    53586 2024-05-17 02:08:20.000000 dspawpy-1.3.0/dspawpy/plot.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-17 09:31:09.924343 dspawpy-1.3.0/dspawpy.egg-info/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13057 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/PKG-INFO
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      651 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/SOURCES.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        1 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/dependency_links.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       76 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/entry_points.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       67 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/requires.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        8 2024-05-17 09:31:09.000000 dspawpy-1.3.0/dspawpy.egg-info/top_level.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       38 2024-05-17 09:31:09.928338 dspawpy-1.3.0/setup.cfg
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1016 2024-05-17 09:31:08.000000 dspawpy-1.3.0/setup.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.074069 dspawpy-1.3.1/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1055 2024-05-16 07:21:06.000000 dspawpy-1.3.1/LICENSE.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13314 2024-05-23 06:52:09.073069 dspawpy-1.3.1/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13132 2024-05-23 06:46:23.000000 dspawpy-1.3.1/README.md
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.041685 dspawpy-1.3.1/dspawpy/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      727 2024-05-23 06:52:06.000000 dspawpy-1.3.1/dspawpy/__init__.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.053143 dspawpy-1.3.1/dspawpy/analysis/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/analysis/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30293 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/analysis/aimdtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17645 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/analysis/vacf.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.057463 dspawpy-1.3.1/dspawpy/cli/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/cli/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    47125 2024-05-21 10:46:53.000000 dspawpy-1.3.1/dspawpy/cli/aux.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     8493 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/cli/cli.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17882 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/cli/menu_prompts.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.062409 dspawpy-1.3.1/dspawpy/diffusion/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/diffusion/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     3551 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/diffusion/neb.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63177 2024-05-21 10:39:47.000000 dspawpy-1.3.1/dspawpy/diffusion/nebtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    10751 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/diffusion/pathfinder.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.069069 dspawpy-1.3.1/dspawpy/io/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/io/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63596 2024-05-21 10:32:07.000000 dspawpy-1.3.1/dspawpy/io/read.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    26595 2024-05-21 09:41:42.000000 dspawpy-1.3.1/dspawpy/io/structure.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30761 2024-05-21 10:30:01.000000 dspawpy-1.3.1/dspawpy/io/utils.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    27382 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/io/write.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    55240 2024-05-21 10:37:48.000000 dspawpy-1.3.1/dspawpy/plot.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.071070 dspawpy-1.3.1/dspawpy.egg-info/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13314 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      651 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        1 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       76 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/entry_points.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       67 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/requires.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        8 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/top_level.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       38 2024-05-23 06:52:09.075070 dspawpy-1.3.1/setup.cfg
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1016 2024-05-23 06:52:06.000000 dspawpy-1.3.1/setup.py
```

### Comparing `dspawpy-1.3.0/LICENSE.txt` & `dspawpy-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/PKG-INFO` & `dspawpy-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -37,14 +37,20 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.1
+
+- BUG修复： 修复userscripts和cli中的一些问题
+- BUG修复： 修复json文件读取函数中的导包语句缺失问题
+- 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
+
 ### 1.3.0
 
 - 重要变更： 不再支持python3.8（不含）以下版本
 - 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
 - 重构： 命令行交互程序增加静默运行模式，便于编程调用
 - 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
 - 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
```

### Comparing `dspawpy-1.3.0/README.md` & `dspawpy-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.1
+
+- BUG修复： 修复userscripts和cli中的一些问题
+- BUG修复： 修复json文件读取函数中的导包语句缺失问题
+- 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
+
 ### 1.3.0
 
 - 重要变更： 不再支持python3.8（不含）以下版本
 - 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
 - 重构： 命令行交互程序增加静默运行模式，便于编程调用
 - 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
 - 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
```

### Comparing `dspawpy-1.3.0/dspawpy/__init__.py` & `dspawpy-1.3.1/dspawpy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 from loguru import logger
 import os
 import sys
 
 # check python version must be 3.6+
 assert sys.version_info >= (3, 6)
```

### Comparing `dspawpy-1.3.0/dspawpy/analysis/aimdtools.py` & `dspawpy-1.3.1/dspawpy/analysis/aimdtools.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/analysis/vacf.py` & `dspawpy-1.3.1/dspawpy/analysis/vacf.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/cli/aux.py` & `dspawpy-1.3.1/dspawpy/cli/aux.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import threading
 from ruamel.yaml import YAML
 import os
 
 from .menu_prompts import Dcheck, Dio, Dresponse, Dselect, Dparameter
 from loguru import logger
-from typing import Optional, Tuple
+from typing import Optional, List
 from prompt_toolkit import prompt
 from prompt_toolkit.completion import PathCompleter, WordCompleter, FuzzyCompleter
 
 pc = FuzzyCompleter(PathCompleter(expanduser=True))  # path completion
 
 yaml = YAML()
 yaml.explicit_start = True
@@ -93,15 +93,15 @@
             if valid:
                 return user_inputs
             else:
                 continue
 
 
 @logger.catch()
-def get_lims(user_prompt, lan) -> Optional[Tuple[float, float]]:
+def get_lims(user_prompt, lan) -> Optional[List[float]]:
     """get lower and higher limits from user input"""
 
     while True:
         userInput = input(user_prompt).strip()
         if userInput == "":
             return None
         else:
@@ -377,15 +377,15 @@
     import_thread.start()
 
     D = {}
     D["menu"] = 31
     D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
     _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
     D["task"] = get_input(
-        str(_list),
+        f"{_list}: ",
         _list,
         completer=WordCompleter(_list),
     )
 
     subtype = None
     if D["task"] == "potential":
         if D["inf"].endswith(".h5"):
@@ -396,15 +396,15 @@
 
             if len(keys) == 0:
                 raise ValueError(f"{Dresponse[lan][3]}{D['infile']}")
             elif len(keys) == 1:
                 subtype = keys[0]
             else:
                 subtype = get_input(
-                    f"{Dselect[lan][0]} {keys}",
+                    f"{Dselect[lan][0]} {keys}: ",
                     keys,
                     completer=WordCompleter(keys),
                 )
 
         elif D["inf"].endswith(".json"):
             from json import load
 
@@ -647,15 +647,16 @@
     D["menu"] = 43
 
     banddatastructure = band_data.structure
     assert banddatastructure is not None
     logger.info(banddatastructure)
     es = banddatastructure.composition.elements
     D["dictio"] = {}
-    from pymatgen import Element
+
+    from pymatgen.core import Element
 
     while True:
         _e = get_input(Dselect[lan][4], [str(e) for e in es], allow_empty=True)
         if _e == "":
             break
         e = Element(_e)
```

### Comparing `dspawpy-1.3.0/dspawpy/cli/cli.py` & `dspawpy-1.3.1/dspawpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/cli/menu_prompts.py` & `dspawpy-1.3.1/dspawpy/cli/menu_prompts.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/diffusion/neb.py` & `dspawpy-1.3.1/dspawpy/diffusion/neb.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/diffusion/nebtools.py` & `dspawpy-1.3.1/dspawpy/diffusion/nebtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     datafile: str = "neb.h5",
     directory: Optional[str] = None,
     ri: Optional[float] = None,
     rf: Optional[float] = None,
     ei: Optional[float] = None,
     ef: Optional[float] = None,
     method: str = "PchipInterpolator",
-    figname: str = "neb_barrier.png",
+    figname: Optional[str] = "neb_barrier.png",
     show: bool = True,
     raw: bool = False,
     **kwargs,
 ):
     r"""调用 scipy.interpolate 插值算法，拟合NEB能垒并绘图
 
     Parameters
```

### Comparing `dspawpy-1.3.0/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.3.1/dspawpy/diffusion/pathfinder.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/io/read.py` & `dspawpy-1.3.1/dspawpy/io/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if TYPE_CHECKING:
     from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 
 
 @logger.catch
 def get_band_data(
     band_dir: str,
-    syst_dir: str = "",
+    syst_dir: Optional[str] = None,
     efermi: Optional[float] = None,
     zero_to_efermi: bool = False,
 ) -> "BandStructureSymmLine":
     """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
 
     Parameters
     ----------
```

### Comparing `dspawpy-1.3.0/dspawpy/io/structure.py` & `dspawpy-1.3.1/dspawpy/io/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,17 @@
         try:
             from dspawpy.io.read import get_sinfo
 
             Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
                 datafile=absfile, si=si, ele=ele, ai=ai
             )  # returned positions, not scaled-positions
             # remove _ from elements
+
+            import re
+
             elements = [re.sub(r"_", "", e) for e in elements]
 
             strs = []
             from pymatgen.core import Structure
 
             for i in range(Nstep):
                 if D_mag_fix:
```

### Comparing `dspawpy-1.3.0/dspawpy/io/utils.py` & `dspawpy-1.3.1/dspawpy/io/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,15 @@
         return G
 
 
 @logger.catch
 def getTSgas(
     fretxt="frequency.txt",
     datafile=".",
-    potentialenergy=0,  # eV
+    potentialenergy: float = 0.0,  # eV
     elements=None,
     geometry="linear",
     positions=None,  # Angstrom
     symmetrynumber=1,
     spin=1,
     temperature=298.15,
     pressure: float = 101325,
```

### Comparing `dspawpy-1.3.0/dspawpy/io/write.py` & `dspawpy-1.3.1/dspawpy/io/write.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/dspawpy/plot.py` & `dspawpy-1.3.1/dspawpy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,22 +259,30 @@
     flags = [x for x in flags_str if x not in temp and (temp.add(x) or True)]
     if " " in flags:  # remove space
         flags.remove(" ")
 
     for flag in flags:
         assert flag in ["1", "2", "3", "4", "5"], "flag must be in '12345'"
 
+    if datafile.endswith("json"):
+        # delete 3 from flags
+        flags = [f for f in flags if f != "3"]
+        logger.warning(
+            "PressureKinetic array is not written in json file, so dspawapy can not read it!\nYou may try aimd.h5 file, which contains that info"
+        )
+
     # 开始画组合图
     N_figs = len(flags)
     import matplotlib.pyplot as plt
 
     fig, axes = plt.subplots(N_figs, 1, sharex=True, figsize=(6, 2 * N_figs))
     if N_figs == 1:  # 'AxesSubplot' object is not subscriptable
         axes = [axes]  # 避免上述类型错误
     fig.suptitle("DSPAW AIMD")
+
     for i, flag in enumerate(flags):
         print("For subfigure " + flag)
         # 读取数据
         xs, ys = _read_aimd_converge_data(datafile, flag)
         if raw:
             try:
                 import polars as pl
@@ -918,15 +926,15 @@
     for i, x in enumerate(Z2):
         if x > Z2_half:
             Z2[i] = Z2_half
 
     return X2, Y2, Z2, emin
 
 
-@logger.catch
+@logger.catch(exception=ValueError)
 def _read_aimd_converge_data(datafile: str, index: Optional[str] = None):
     """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
 
     Parameters
     ----------
     datafile : str or list
         hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
@@ -952,72 +960,107 @@
             ys.extend(y)
         xs = np.linspace(1, len(xs), len(xs))
         return xs, ys
 
     # search datafile in the given directory
     elif isinstance(datafile, str):
         from dspawpy.io.utils import get_absfile
-        from h5py import File
 
-        absfile = get_absfile(datafile, task="aimd", only_h5=True)
-        hf = File(absfile)  # 加载h5文件
-        print(f"Reading {absfile}...")
-        Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
-        ys = np.full(Nstep, np.nan)  # 准备一个空数组
-        # 开始读取
-        if index == "5":
-            for i in range(1, Nstep + 1):
-                ys[i - 1] = np.linalg.det(
-                    np.array(hf.get("/Structures/Step-%d/Lattice" % i))
-                )
-        else:
-            map = {
-                "1": "IonsKineticEnergy",
-                "2": "TotalEnergy0",
-                "3": "PressureKinetic",
-                "4": "Temperature",
-            }
-            if index == "3" and "PressureKinetic" not in np.array(
-                hf.get("/AimdInfo/Step-1")
-            ):
-                logger.warning(
-                    "Ensemble is neither NPT nor NPH, no PressureKinetic found for subfigure 3!"
-                )
-            else:
+        absfile = get_absfile(datafile, task="aimd")
+
+        if datafile.endswith("h5"):
+            from h5py import File
+
+            hf = File(absfile)  # 加载h5文件
+            print(f"Reading {absfile}...")
+            Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
+            ys = np.full(Nstep, np.nan)  # 准备一个空数组
+            # 开始读取
+            if index == "5":
                 for i in range(1, Nstep + 1):
-                    assert index is not None
-                    try:
-                        ys[i - 1] = np.array(
-                            hf.get("/AimdInfo/Step-%d/%s" % (i, map[index]))
-                        )
-                    except Exception:
-                        ys[i - 1] = 0
-                        ys = np.delete(ys, -1)
-                        logger.warning(
-                            "-> AIMD task stopped at Nstep=%s, failed to read its %s value"
-                            % (Nstep, map[index])
-                        )
-                        break
+                    ys[i - 1] = np.linalg.det(
+                        np.array(hf.get("/Structures/Step-%d/Lattice" % i))
+                    )
+            else:
+                map = {
+                    "1": "IonsKineticEnergy",
+                    "2": "TotalEnergy0",
+                    "3": "PressureKinetic",
+                    "4": "Temperature",
+                }
+                if index == "3" and "PressureKinetic" not in np.array(
+                    hf.get("/AimdInfo/Step-1")
+                ):
+                    logger.warning(
+                        "Ensemble is neither NPT nor NPH, no PressureKinetic found for subfigure 3!"
+                    )
+                else:
+                    for i in range(1, Nstep + 1):
+                        assert index is not None
+                        try:
+                            ys[i - 1] = np.array(
+                                hf.get("/AimdInfo/Step-%d/%s" % (i, map[index]))
+                            )
+                        except Exception:
+                            ys[i - 1] = 0
+                            ys = np.delete(ys, -1)
+                            logger.warning(
+                                "-> AIMD task stopped at Nstep=%s, failed to read its %s value"
+                                % (Nstep, map[index])
+                            )
+                            break
+
+            Nstep = len(ys)  # 步数更新为实际完成的步数
+        elif datafile.endswith("json"):
+            from json import load
+
+            with open(absfile, "r") as f:
+                data = load(f)
+            Nstep = len(data["Structures"])
+            ys = np.zeros(Nstep)
+
+            if index == "5":
+                for i in range(Nstep):
+                    ys[i] = np.linalg.det(
+                        np.array(data["Structures"][i]["Lattice"]).reshape(3, 3)
+                    )
+            else:
+                map = {
+                    "1": "IonsKineticEnergy",
+                    "2": "TotalEnergy0",
+                    "3": "PressureKinetic",
+                    "4": "Temperature",
+                }
+                assert index is not None
+                if index in ["1", "2"]:
+                    ys = data["AimdInfo"]["Energy"][map[index]]
+
+                elif index == "3":
+                    raise ValueError(
+                        "PressureKinetic array is not written in json file, so dspawapy can not read it!"
+                    )
+                else:
+                    ys = data["AimdInfo"][map[index]]
 
-        Nstep = len(ys)  # 步数更新为实际完成的步数
+            Nstep = len(ys)  # 步数更新为实际完成的步数
 
         # 返回xs，ys两个数组
-        return np.linspace(1, Nstep, Nstep), np.array(ys)
+        return np.linspace(1, Nstep, Nstep), np.array(ys)  # type: ignore
 
     else:
         raise TypeError("datafile must be str or list")
 
 
 @logger.catch
 def pltbd(
     bdp: "BSDOSPlotter",
     bs: "BandStructureSymmLine",
     dos: Optional["CompleteDos"] = None,
     demax: float = 0.1,
-    ylim: Optional[Tuple[float, float]] = None,
+    ylim: Optional[List[float]] = None,
     alpha: float = 0.3,
     colors: Optional[List[str]] = None,
     filename: str = "banddos.png",
     dpi: int = 300,
 ):
     """基于BSDOSPlotter类的get_plot()优化而来，可绘制（投影）能带态密度图。
 
@@ -1387,16 +1430,16 @@
 
     return plt
 
 
 @logger.catch
 def plot_dos(
     dosplotter,
-    xlim: Optional[Tuple[float, float]] = None,
-    ylim: Optional[Tuple[float, float]] = None,
+    xlim: Optional[List[float]] = None,
+    ylim: Optional[List[float]] = None,
     invert_axes: bool = False,
     beta_dashed: bool = False,
     raw: bool = False,
 ):
     """Get a matplotlib plot showing the DOS.
 
     Args:
```

### Comparing `dspawpy-1.3.0/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.3.1/dspawpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -37,14 +37,20 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.1
+
+- BUG修复： 修复userscripts和cli中的一些问题
+- BUG修复： 修复json文件读取函数中的导包语句缺失问题
+- 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
+
 ### 1.3.0
 
 - 重要变更： 不再支持python3.8（不含）以下版本
 - 重要变更： 合并cli.py和cli_en.py，通过命令行选项 -l 或 --language 切换交互提示语言
 - 重构： 命令行交互程序增加静默运行模式，便于编程调用
 - 重构： 命令行交互程序大幅提高可读性，在等待用户输入同时多线程动态载入最终调用的函数
 - 重构： 懒导入——将导包语句从文件开头尽量移入函数中，避免导入不必要模块，减少导包耗时
```

### Comparing `dspawpy-1.3.0/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.3.1/dspawpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.0/setup.py` & `dspawpy-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         encoding="utf-8",
     ) as fin:
         return fin.read()
 
 
 setup(
     name="dspawpy",
-    version="1.3.0",
+    version="1.3.1",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
```

