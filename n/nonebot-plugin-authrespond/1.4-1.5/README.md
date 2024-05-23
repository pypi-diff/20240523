# Comparing `tmp/nonebot_plugin_authrespond-1.4.tar.gz` & `tmp/nonebot_plugin_authrespond-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_authrespond-1.4.tar", last modified: Wed May 22 09:46:08 2024, max compression
+gzip compressed data, was "nonebot_plugin_authrespond-1.5.tar", last modified: Thu May 23 13:47:49 2024, max compression
```

## Comparing `nonebot_plugin_authrespond-1.4.tar` & `nonebot_plugin_authrespond-1.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:46:08.208589 nonebot_plugin_authrespond-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-22 09:46:08.208589 nonebot_plugin_authrespond-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:46:08.204589 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/cubp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/plugins_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:46:08.208589 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-22 09:46:08.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 09:46:08.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:46:08.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 09:46:08.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 09:46:08.000000 nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-22 09:46:04.000000 nonebot_plugin_authrespond-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:46:08.208589 nonebot_plugin_authrespond-1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:47:49.439965 nonebot_plugin_authrespond-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-23 13:47:49.439965 nonebot_plugin_authrespond-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:47:49.439965 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/cubp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/plugins_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:47:49.439965 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-23 13:47:49.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 13:47:49.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:47:49.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 13:47:49.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 13:47:49.000000 nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-23 13:47:45.000000 nonebot_plugin_authrespond-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:47:49.439965 nonebot_plugin_authrespond-1.5/setup.cfg
```

### Comparing `nonebot_plugin_authrespond-1.4/LICENSE` & `nonebot_plugin_authrespond-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.4/PKG-INFO` & `nonebot_plugin_authrespond-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.4
+Version: 1.5
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.4/README.md` & `nonebot_plugin_authrespond-1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/__init__.py` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from nonebot import require
+require("nonebot_plugin_session")
+require("nonebot_plugin_alconna")
 from nonebot.plugin import PluginMetadata
 from .config import cubplugins_permission
+from nonebot.plugin import inherit_supported_adapters
 
 __plugin_meta__ = PluginMetadata(
     name="插件响应鉴权",
     description="nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局",
     usage='''用户操作模式:  #(全局|插件名称)(拉黑|解黑)(全员|用户id)
 群聊操作模式: #(全局|插件名称)(封禁群|解禁群)(群号|留空封禁所在群)''',
 
@@ -11,28 +15,17 @@
     # 发布必填，当前有效类型有：`library`（为其他插件编写提供功能），`application`（向机器人用户提供功能）。
 
     homepage="https://github.com/cubstaryow/nonebot-plugin-authrespond",
     # 发布必填。
 
     config=cubplugins_permission,
     # 插件配置项类，如无需配置可不填写。
-
-    supported_adapters={
-        "~onebot.v11",
-        "~onebot.v12",
-        "~console",
-        "~kaiheila",
-        "~telegram",
-        "~feishu",
-        "~red",
-        "~discord",
-        "~qq",
-        "~satori",
-        "~dodo"
-        }
+    supported_adapters=inherit_supported_adapters(
+        "nonebot_plugin_alconna"
+    )
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 from .run import *
 
 from .perm import *
```

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/cubp.py` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/cubp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/perm.py` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/perm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot import get_loaded_plugins, on_regex
 
 from nonebot.adapters import Message ,Event
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.params import RegexGroup
 from .cubp import cubp
-from .session import  EventSession
+from nonebot_plugin_session import EventSession
 from nonebot_plugin_alconna import UniMessage , At
 
 turn_push = on_regex(
     r"^#([\S|-]*)(拉黑|解黑|封禁群|解禁群)([\S|-]*)$",
     block=True,
     priority=2,
     permission=SUPERUSER
```

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/plugins_data.py` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond/run.py` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot import get_driver , logger
 from nonebot.matcher import Matcher
 from nonebot.message import run_preprocessor
 from nonebot.exception import IgnoredException
 from .cubp import cubp
-from .session import EventSession
+from nonebot_plugin_session import EventSession
 
 superusers = get_driver().config.superusers
 
 
 @run_preprocessor
 async def pass_run(
     matcher: Matcher,
```

### Comparing `nonebot_plugin_authrespond-1.4/nonebot_plugin_authrespond.egg-info/PKG-INFO` & `nonebot_plugin_authrespond-1.5/nonebot_plugin_authrespond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.4
+Version: 1.5
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.4/pyproject.toml` & `nonebot_plugin_authrespond-1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-authrespond"
-version = "1.4"
+version = "1.5"
 description = "nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

