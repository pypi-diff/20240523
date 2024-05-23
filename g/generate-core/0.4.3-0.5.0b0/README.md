# Comparing `tmp/generate_core-0.4.3.tar.gz` & `tmp/generate_core-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate_core-0.4.3.tar", max compression
+gzip compressed data, was "generate_core-0.5.0b0.tar", max compression
```

## Comparing `generate_core-0.4.3.tar` & `generate_core-0.5.0b0.tar`

### file list

```diff
@@ -1,80 +1,64 @@
--rw-r--r--   0        0        0     1067 2024-04-12 03:10:53.501705 generate_core-0.4.3/LICENSE
--rw-r--r--   0        0        0    10107 2024-04-12 03:10:53.501705 generate_core-0.4.3/README.md
--rw-r--r--   0        0        0     4411 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/__init__.py
--rw-r--r--   0        0        0      994 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/access_token_manager.py
--rw-r--r--   0        0        0     3884 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/__init__.py
--rw-r--r--   0        0        0     5765 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/base.py
--rw-r--r--   0        0        0      920 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/cost_caculator.py
--rw-r--r--   0        0        0     1071 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/__init__.py
--rw-r--r--   0        0        0     2731 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/core.py
--rw-r--r--   0        0        0      666 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/exception.py
--rw-r--r--   0        0        0     1603 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/message/utils.py
--rw-r--r--   0        0        0      669 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/model_output.py
--rw-r--r--   0        0        0     2522 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/__init__.py
--rw-r--r--   0        0        0     8612 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/anthropic.py
--rw-r--r--   0        0        0     3604 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/azure.py
--rw-r--r--   0        0        0     7067 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/baichuan.py
--rw-r--r--   0        0        0     8648 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/bailian.py
--rw-r--r--   0        0        0     6688 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/dashscope.py
--rw-r--r--   0        0        0     9178 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/dashscope_multimodal.py
--rw-r--r--   0        0        0     2967 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/deepseek.py
--rw-r--r--   0        0        0     8135 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/hunyuan.py
--rw-r--r--   0        0        0     5535 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax.py
--rw-r--r--   0        0        0     7992 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax_legacy.py
--rw-r--r--   0        0        0    15084 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/minimax_pro.py
--rw-r--r--   0        0        0     2609 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/moonshot.py
--rw-r--r--   0        0        0     4424 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/openai.py
--rw-r--r--   0        0        0    13949 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/openai_like.py
--rw-r--r--   0        0        0     2893 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/stepfun.py
--rw-r--r--   0        0        0     3226 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/test.py
--rw-r--r--   0        0        0     9678 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/wenxin.py
--rw-r--r--   0        0        0     2489 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/yi.py
--rw-r--r--   0        0        0    20581 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/models/zhipu.py
--rw-r--r--   0        0        0     2362 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/printer.py
--rw-r--r--   0        0        0     2271 2024-04-12 03:10:53.501705 generate_core-0.4.3/generate/chat_completion/stream_manager.py
--rw-r--r--   0        0        0     3225 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/chat_completion/tool.py
--rw-r--r--   0        0        0     3040 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/highlevel.py
--rw-r--r--   0        0        0    10242 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/http.py
--rw-r--r--   0        0        0     1475 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/__init__.py
--rw-r--r--   0        0        0     1223 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/base.py
--rw-r--r--   0        0        0      710 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/__init__.py
--rw-r--r--   0        0        0     7538 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/baidu.py
--rw-r--r--   0        0        0     7064 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/openai.py
--rw-r--r--   0        0        0     4404 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/qianfan.py
--rw-r--r--   0        0        0     3093 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/image_generation/models/zhipu.py
--rw-r--r--   0        0        0     3400 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/model.py
--rw-r--r--   0        0        0        0 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/__init__.py
--rw-r--r--   0        0        0     9232 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/agent.py
--rw-r--r--   0        0        0     5110 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/hook.py
--rw-r--r--   0        0        0     3935 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/limit.py
--rw-r--r--   0        0        0     2854 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/session.py
--rw-r--r--   0        0        0     8333 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/modifiers/structure.py
--rw-r--r--   0        0        0     1225 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/__init__.py
--rw-r--r--   0        0        0      440 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/anthropic.py
--rw-r--r--   0        0        0      487 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/azure.py
--rw-r--r--   0        0        0      444 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/baichuan.py
--rw-r--r--   0        0        0     3278 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/baidu.py
--rw-r--r--   0        0        0     1434 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/bailian.py
--rw-r--r--   0        0        0      997 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/base.py
--rw-r--r--   0        0        0      423 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/dashscope.py
--rw-r--r--   0        0        0      419 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/deepseek.py
--rw-r--r--   0        0        0      575 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/hunyuan.py
--rw-r--r--   0        0        0      452 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/minimax.py
--rw-r--r--   0        0        0      417 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/moonshot.py
--rw-r--r--   0        0        0      411 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/openai.py
--rw-r--r--   0        0        0      198 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/openai_like.py
--rw-r--r--   0        0        0      411 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/stepfun.py
--rw-r--r--   0        0        0      431 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/yi.py
--rw-r--r--   0        0        0     1216 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/platforms/zhipu.py
--rw-r--r--   0        0        0     1398 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/test.py
--rw-r--r--   0        0        0     1019 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/__init__.py
--rw-r--r--   0        0        0     1099 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/base.py
--rw-r--r--   0        0        0      419 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/__init__.py
--rw-r--r--   0        0        0     8043 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/minimax.py
--rw-r--r--   0        0        0     3690 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/text_to_speech/models/openai.py
--rw-r--r--   0        0        0      450 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/types.py
--rw-r--r--   0        0        0     7200 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/ui.py
--rw-r--r--   0        0        0     2242 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/utils.py
--rw-r--r--   0        0        0       22 2024-04-12 03:10:53.505705 generate_core-0.4.3/generate/version.py
--rw-r--r--   0        0        0     2119 2024-04-12 03:10:53.505705 generate_core-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    11300 1970-01-01 00:00:00.000000 generate_core-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/LICENSE
+-rw-r--r--   0        0        0    10484 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/README.md
+-rw-r--r--   0        0        0     2340 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/__init__.py
+-rw-r--r--   0        0        0      994 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/access_token_manager.py
+-rw-r--r--   0        0        0     2939 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/__init__.py
+-rw-r--r--   0        0        0     7346 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/base.py
+-rw-r--r--   0        0        0     1071 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/message/__init__.py
+-rw-r--r--   0        0        0     3277 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/message/converter.py
+-rw-r--r--   0        0        0     2953 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/message/core.py
+-rw-r--r--   0        0        0      666 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/message/exception.py
+-rw-r--r--   0        0        0     1639 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/message/utils.py
+-rw-r--r--   0        0        0     1041 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/model_output.py
+-rw-r--r--   0        0        0     1587 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/models/__init__.py
+-rw-r--r--   0        0        0    12211 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/models/anthropic.py
+-rw-r--r--   0        0        0     3172 2024-05-23 11:39:15.238616 generate_core-0.5.0b0/generate/chat_completion/models/azure.py
+-rw-r--r--   0        0        0     3797 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/baichuan.py
+-rw-r--r--   0        0        0    11005 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/dashscope.py
+-rw-r--r--   0        0        0     3301 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/deepseek.py
+-rw-r--r--   0        0        0     4900 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/minimax.py
+-rw-r--r--   0        0        0     2643 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/moonshot.py
+-rw-r--r--   0        0        0     1363 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/openai.py
+-rw-r--r--   0        0        0    14280 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/openai_like.py
+-rw-r--r--   0        0        0     5387 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/openrouter.py
+-rw-r--r--   0        0        0     3063 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/stepfun.py
+-rw-r--r--   0        0        0     3226 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/test.py
+-rw-r--r--   0        0        0     2709 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/yi.py
+-rw-r--r--   0        0        0    13734 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/models/zhipu.py
+-rw-r--r--   0        0        0     2362 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/printer.py
+-rw-r--r--   0        0        0     2204 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/stream_manager.py
+-rw-r--r--   0        0        0     4440 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/chat_completion/tool.py
+-rw-r--r--   0        0        0       28 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/constant.py
+-rw-r--r--   0        0        0     1766 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/highlevel.py
+-rw-r--r--   0        0        0    10513 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/http.py
+-rw-r--r--   0        0        0     3367 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/model.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/__init__.py
+-rw-r--r--   0        0        0     9236 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/agent.py
+-rw-r--r--   0        0        0     2643 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/cache.py
+-rw-r--r--   0        0        0     5110 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/hook.py
+-rw-r--r--   0        0        0     3935 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/limit.py
+-rw-r--r--   0        0        0     2854 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/session.py
+-rw-r--r--   0        0        0     8442 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/modifiers/structure.py
+-rw-r--r--   0        0        0     1156 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/anthropic.py
+-rw-r--r--   0        0        0      426 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/azure.py
+-rw-r--r--   0        0        0      375 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/baichuan.py
+-rw-r--r--   0        0        0     3278 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/baidu.py
+-rw-r--r--   0        0        0      997 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/base.py
+-rw-r--r--   0        0        0      488 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/dashscope.py
+-rw-r--r--   0        0        0      419 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/deepseek.py
+-rw-r--r--   0        0        0      452 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/minimax.py
+-rw-r--r--   0        0        0      417 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/moonshot.py
+-rw-r--r--   0        0        0      411 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/openai.py
+-rw-r--r--   0        0        0      198 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/openai_like.py
+-rw-r--r--   0        0        0      412 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/openrouter.py
+-rw-r--r--   0        0        0      411 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/stepfun.py
+-rw-r--r--   0        0        0      413 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/yi.py
+-rw-r--r--   0        0        0     1141 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/platforms/zhipu.py
+-rw-r--r--   0        0        0     1398 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/test.py
+-rw-r--r--   0        0        0      450 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/types.py
+-rw-r--r--   0        0        0     6777 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/ui.py
+-rw-r--r--   0        0        0     2242 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/utils.py
+-rw-r--r--   0        0        0       32 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/generate/version.py
+-rw-r--r--   0        0        0     2127 2024-05-23 11:39:15.242616 generate_core-0.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0    11721 1970-01-01 00:00:00.000000 generate_core-0.5.0b0/PKG-INFO
```

### Comparing `generate_core-0.4.3/LICENSE` & `generate_core-0.5.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/README.md` & `generate_core-0.5.0b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,44 +20,46 @@
 [![Documentation](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://wangyuxinwhy.github.io/generate/)
 [![Made with Love](https://img.shields.io/badge/made%20with-love-red.svg)](#)
 
 </div>
 <br>
 <br>
 
-# 简介
-
+> [!IMPORTANT]  
+> generate v0.5.0 版本的设计思路发生较大变化。由于个人精力有限，generate 不再追求支持更多的平台，而是更多的围绕模型的辅助功能进行开发。另外，国内大部分平台已经提供了适配 OpenAI SDK 的 API，如果你只需要基础的文本生成功能，建议直接使用 OpenAI SDK。
 
+# 简介
 
 Generate 允许用户通过统一的 api 访问多平台的生成式模型，当前支持：
 
-| 平台 🤖           | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
-| ----------------- | ------- | ------- | ------- | --------- | -------- |
-| OpenAI            | ✅      | ✅      | ✅      | ✅        | ✅       |
-| Azure             | ✅      | ✅      | ❌      | ✅        | ✅       |
-| Anthropic         | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 文心 Wenxin       | ✅      | ✅      | ✅      | ❌        | ✅       |
-| 百炼 Bailian      | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 灵积 DashScope    | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 百川智能 Baichuan | ✅      | ✅      | ✅      | ❌        | ❌       |
-| Minimax           | ✅      | ✅      | ✅      | ❌        | ✅       |
-| 混元 Hunyuan      | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 智谱 Zhipu        | ✅      | ✅      | ✅      | ✅        | ✅       |
-| 月之暗面 Moonshot | ✅      | ✅      | ✅      | ❌        | ❌       |
-| DeepSeek          | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 零一万物 Yi       | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 阶跃星辰 StepFun  | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 平台 🤖             | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
+| ------------------- | ------- | ------- | ------- | --------- | -------- |
+| OpenAI              | ✅      | ✅      | ✅      | ✅        | ✅       |
+| Azure               | ✅      | ✅      | ❌      | ✅        | ✅       |
+| Anthropic           | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 文心 Wenxin         | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 灵积/百炼 DashScope | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 百川智能 Baichuan   | ✅      | ✅      | ✅      | ❌        | ✅       |
+| Minimax             | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 混元 Hunyuan        | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 智谱 Zhipu          | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 月之暗面 Moonshot   | ✅      | ✅      | ✅      | ❌        | ✅       |
+| DeepSeek            | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 零一万物 Yi         | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 阶跃星辰 StepFun    | ✅      | ✅      | ✅      | ✅        | ❌       |
+
+> v0.5.0-beta 版本中，混元，文心尚未适配
 
 ## Features
 
 - **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
 - **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
 - **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
 - **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
-- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，_Agent_, _Tool call_ 等
+- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，Disk Cache，_Agent_, _Tool call_ 等
 - **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
 - **高质量代码**，100% typehints，pylance strict, ruff lint & format, test coverage > 85% ...
 
 ## 基础使用
 
 <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
```

### Comparing `generate_core-0.4.3/generate/access_token_manager.py` & `generate_core-0.5.0b0/generate/access_token_manager.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/chat_completion/base.py` & `generate_core-0.5.0b0/generate/chat_completion/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from __future__ import annotations
 
+import json
 import logging
 from abc import ABC, abstractmethod
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, AsyncIterator, ClassVar, Iterator, List, Type, TypeVar, get_type_hints
 
 from pydantic import BaseModel
 from typing_extensions import Self, Unpack, override
 
 from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.converter import MessageConverter
+from generate.chat_completion.message.core import Messages
+from generate.chat_completion.message.utils import ensure_messages
 from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
 from generate.chat_completion.stream_manager import StreamManager
+from generate.chat_completion.tool import SupportToolCall
 from generate.http import HttpClient, HttpxPostKwargs
 from generate.model import GenerateModel, ModelParameters
 from generate.platforms import PlatformSettings
 from generate.utils import sync_aiter
 
 O = TypeVar('O', bound=BaseModel)  # noqa: E741
 
 if TYPE_CHECKING:
     from generate.modifiers.agent import Agent, AgentKwargs
+    from generate.modifiers.cache import CacheChatCompletionModel
     from generate.modifiers.hook import HookChatCompletionModel, HookModelKwargs
     from generate.modifiers.session import SessionChatCompletionModel
     from generate.modifiers.structure import StructureGenerateModel, StructureModelKwargs
 
 
 logger = logging.getLogger(__name__)
 
@@ -59,79 +66,110 @@
         return Agent(model=self, **kwargs)
 
     def hook(self, **kwargs: Unpack['HookModelKwargs']) -> 'HookChatCompletionModel':
         from generate.modifiers.hook import HookChatCompletionModel
 
         return HookChatCompletionModel(model=self, **kwargs)
 
+    def cache(self, cache_dir: Path | str | None = None) -> 'CacheChatCompletionModel':
+        from generate.modifiers.cache import CacheChatCompletionModel
+
+        return CacheChatCompletionModel(model=self, cache_dir=cache_dir)
+
 
 class RemoteChatCompletionModel(ChatCompletionModel, ABC):
     settings: PlatformSettings
     http_client: HttpClient
+    message_converter: MessageConverter
     available_models: ClassVar[List[str]] = []
 
     def __init__(
         self,
         model: str,
         parameters: ModelParameters,
         settings: PlatformSettings,
         http_client: HttpClient,
+        message_converter: MessageConverter,
     ) -> None:
         self.model = model
         self.parameters = parameters
         self.settings = settings
         self.http_client = http_client
+        self.message_converter = message_converter
 
     @abstractmethod
     def _process_reponse(self, response: dict[str, Any]) -> ChatCompletionOutput:
         ...
 
     @abstractmethod
-    def _process_stream_line(self, line: str, stream_manager: StreamManager) -> ChatCompletionStreamOutput | None:
+    def _process_stream_response(
+        self, response: dict[str, Any], stream_manager: StreamManager
+    ) -> ChatCompletionStreamOutput | None:
         ...
 
     @abstractmethod
-    def _get_request_parameters(self, prompt: Prompt, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
+    def _get_request_parameters(self, messages: Messages, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
         ...
 
+    def list_models(self) -> List[str]:
+        return self.available_models
+
+    def process_prompt(self, prompt: Prompt) -> Messages:
+        messages = ensure_messages(prompt)
+        if isinstance(self, SupportToolCall):
+            self.process_messages_for_tool_call(messages)
+        return messages
+
     @override
     def generate(self, prompt: Prompt, **kwargs: Any) -> ChatCompletionOutput:
         timeout = kwargs.pop('timeout') if 'timeout' in kwargs else None
-        request_parameters = self._get_request_parameters(prompt, **kwargs)
+        messages = self.process_prompt(prompt)
+        request_parameters = self._get_request_parameters(messages, **kwargs)
         request_parameters['timeout'] = timeout
         response = self.http_client.post(request_parameters=request_parameters)
         return self._process_reponse(response.json())
 
     @override
     async def async_generate(self, prompt: Prompt, **kwargs: Any) -> ChatCompletionOutput:
         timeout = kwargs.pop('timeout') if 'timeout' in kwargs else None
-        request_parameters = self._get_request_parameters(prompt, **kwargs)
+        messages = self.process_prompt(prompt)
+        request_parameters = self._get_request_parameters(messages, **kwargs)
         request_parameters['timeout'] = timeout
         response = await self.http_client.async_post(request_parameters=request_parameters)
         return self._process_reponse(response.json())
 
     @override
     def stream_generate(self, prompt: Prompt, **kwargs: Any) -> Iterator[ChatCompletionStreamOutput]:
         timeout = kwargs.pop('timeout') if 'timeout' in kwargs else None
-        request_parameters = self._get_request_parameters(prompt, stream=True, **kwargs)
+        messages = self.process_prompt(prompt)
+        request_parameters = self._get_request_parameters(messages, stream=True, **kwargs)
         request_parameters['timeout'] = timeout
         stream_manager = StreamManager(info=self.model_info)
         for line in self.http_client.stream_post(request_parameters=request_parameters):
-            if output := self._process_stream_line(line, stream_manager):
-                yield output
+            try:
+                response = json.loads(line)
+                if (output := self._process_stream_response(response, stream_manager)) and output:
+                    yield output
+            except json.JSONDecodeError:
+                continue
 
     @override
     async def async_stream_generate(self, prompt: Prompt, **kwargs: Any) -> AsyncIterator[ChatCompletionStreamOutput]:
         timeout = kwargs.pop('timeout') if 'timeout' in kwargs else None
-        request_parameters = self._get_request_parameters(prompt, stream=True, **kwargs)
+        messages = self.process_prompt(prompt)
+        request_parameters = self._get_request_parameters(messages, stream=True, **kwargs)
         request_parameters['timeout'] = timeout
         stream_manager = StreamManager(info=self.model_info)
         async for line in self.http_client.async_stream_post(request_parameters=request_parameters):
-            if output := self._process_stream_line(line, stream_manager):
-                yield output
+            try:
+                response = json.loads(line)
+                if (output := self._process_stream_response(response, stream_manager)) and output:
+                    yield output
+            except json.JSONDecodeError:
+                continue
 
     @classmethod
     def how_to_settings(cls) -> str:
         return f'{cls.__name__} Settings\n\n' + get_type_hints(cls)['settings'].how_to_settings()
 
     @property
     def name(self) -> str:
```

### Comparing `generate_core-0.4.3/generate/chat_completion/message/__init__.py` & `generate_core-0.5.0b0/generate/chat_completion/message/__init__.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/chat_completion/message/exception.py` & `generate_core-0.5.0b0/generate/chat_completion/message/exception.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/chat_completion/message/utils.py` & `generate_core-0.5.0b0/generate/chat_completion/message/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any, Literal
 
 from generate.chat_completion.message.core import (
     FunctionCall,
     Message,
     Messages,
     Prompt,
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/azure.py` & `generate_core-0.5.0b0/generate/chat_completion/models/azure.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,81 @@
 from __future__ import annotations
 
-from typing import Any, AsyncIterator, ClassVar, Iterator
+from typing import Any, AsyncIterator, ClassVar, Dict, Iterator
 
 from typing_extensions import Unpack, override
 
-from generate.chat_completion.base import RemoteChatCompletionModel
-from generate.chat_completion.message import Prompt, ensure_messages
-from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
-from generate.chat_completion.models.openai import OpenAIChatParameters, OpenAIChatParametersDict
-from generate.chat_completion.models.openai_like import convert_to_openai_message, process_openai_like_model_reponse
+from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.core import Messages
+from generate.chat_completion.model_output import ChatCompletionStreamOutput
+from generate.chat_completion.models.openai_like import (
+    OpenAIChatParameters,
+    OpenAIChatParametersDict,
+    OpenAILikeChat,
+    OpenAIMessageConverter,
+)
 from generate.chat_completion.stream_manager import StreamManager
 from generate.http import HttpClient, HttpxPostKwargs
 from generate.platforms.azure import AzureSettings
 
 
-class AzureChat(RemoteChatCompletionModel):
+class AzureChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'azure'
 
     parameters: OpenAIChatParameters
     settings: AzureSettings
+    message_converter: OpenAIMessageConverter
 
     def __init__(
         self,
         model: str | None = None,
         parameters: OpenAIChatParameters | None = None,
         settings: AzureSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: OpenAIMessageConverter | None = None,
     ) -> None:
         parameters = parameters or OpenAIChatParameters()
         settings = settings or AzureSettings()  # type: ignore
         http_client = http_client or HttpClient()
         model = model or settings.chat_api_engine
         if model is None:
             raise ValueError('model must be provided or set in settings.chat_api_engine')
-        super().__init__(model, parameters=parameters, settings=settings, http_client=http_client)
-
-    @override
-    def generate(self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]) -> ChatCompletionOutput:
-        return super().generate(prompt, **kwargs)
-
-    @override
-    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]) -> ChatCompletionOutput:
-        return await super().async_generate(prompt, **kwargs)
+        message_converter = message_converter or OpenAIMessageConverter()
+        super().__init__(
+            model=model, parameters=parameters, settings=settings, http_client=http_client, message_converter=message_converter
+        )
 
     @override
     def stream_generate(
         self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]
     ) -> Iterator[ChatCompletionStreamOutput]:
         raise NotImplementedError('Azure does not support streaming')
 
     @override
     def async_stream_generate(
         self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]
     ) -> AsyncIterator[ChatCompletionStreamOutput]:
         raise NotImplementedError('Azure does not support streaming')
 
     @override
-    def _get_request_parameters(self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]) -> HttpxPostKwargs:
-        messages = ensure_messages(prompt)
+    def _get_request_parameters(self, messages: Messages, **kwargs: Unpack[OpenAIChatParametersDict]) -> HttpxPostKwargs:
         parameters = self.parameters.clone_with_changes(**kwargs)
-
-        openai_messages = [convert_to_openai_message(message) for message in messages]
         json_data = {
             'model': self.model,
-            'messages': openai_messages,
+            'messages': self.message_converter.convert_messages(messages),
             **parameters.custom_model_dump(),
         }
         headers = {
             'api-key': self.settings.api_key.get_secret_value(),
         }
         return {
             'url': f'{self.settings.api_base}/openai/deployments/{self.model}/chat/completions',
             'headers': headers,
             'json': json_data,
             'params': {'api-version': self.settings.api_version},
         }
 
     @override
-    def _process_reponse(self, response: dict[str, Any]) -> ChatCompletionOutput:
-        return process_openai_like_model_reponse(response, model_type=self.model_type)
-
-    @override
-    def _process_stream_line(self, line: str, stream_manager: StreamManager) -> ChatCompletionStreamOutput | None:
-        raise NotImplementedError
+    def _process_stream_response(
+        self, response: Dict[str, Any], stream_manager: StreamManager
+    ) -> ChatCompletionStreamOutput | None:
+        raise NotImplementedError('Azure does not support streaming')
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/deepseek.py` & `generate_core-0.5.0b0/generate/chat_completion/models/deepseek.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import AsyncIterator, ClassVar, Iterator, List, Optional, Union
 
 from pydantic import Field, PositiveInt
 from typing_extensions import Annotated, Unpack, override
 
 from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.converter import MessageConverter
 from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
 from generate.chat_completion.models.openai_like import OpenAILikeChat
 from generate.http import HttpClient
 from generate.model import ModelParameters, RemoteModelParametersDict
 from generate.platforms import DeepSeekSettings
 from generate.types import Probability
 
@@ -17,23 +18,27 @@
 class DeepSeekChatParameters(ModelParameters):
     temperature: Optional[Annotated[float, Field(ge=0, le=2)]] = None
     top_p: Optional[Probability] = None
     max_tokens: Optional[PositiveInt] = None
     frequency_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
     presence_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
     stop: Optional[Union[str, List[str]]] = None
+    logprobs: Optional[bool] = None
+    top_logprobs: Optional[Annotated[int, Field(ge=0, le=20)]] = None
 
 
 class DeepSeekParametersDict(RemoteModelParametersDict, total=False):
     temperature: Optional[float]
     top_p: Optional[Probability]
     max_tokens: Optional[PositiveInt]
     frequency_penalty: Optional[float]
     presence_penalty: Optional[float]
     stop: Optional[Union[str, List[str]]]
+    logprobs: Optional[bool]
+    top_logprobs: Optional[int]
 
 
 class DeepSeekChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'deepseek'
     available_models: ClassVar[List[str]] = ['deepseek-chat', 'deepseek-coder']
 
     parameters: DeepSeekChatParameters
@@ -41,20 +46,25 @@
 
     def __init__(
         self,
         model: str = 'deepseek-chat',
         parameters: DeepSeekChatParameters | None = None,
         settings: DeepSeekSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: MessageConverter | None = None,
     ) -> None:
         parameters = parameters or DeepSeekChatParameters()
         settings = settings or DeepSeekSettings()  # type: ignore
-        http_client = http_client or HttpClient()
-        model = model
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            message_converter=message_converter,
+            http_client=http_client,
+        )
 
     @override
     def generate(self, prompt: Prompt, **kwargs: Unpack[DeepSeekParametersDict]) -> ChatCompletionOutput:
         return super().generate(prompt, **kwargs)
 
     @override
     async def async_generate(self, prompt: Prompt, **kwargs: Unpack[DeepSeekParametersDict]) -> ChatCompletionOutput:
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/minimax.py` & `generate_core-0.5.0b0/generate/chat_completion/models/minimax.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 from pydantic import PositiveInt, field_validator
 from typing_extensions import Unpack, override
 
 from generate.chat_completion.message import (
     Prompt,
 )
-from generate.chat_completion.message.core import AssistantMessage, FunctionMessage, Messages, ToolCall, ToolMessage
-from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
-from generate.chat_completion.models.openai_like import OpenAILikeChat, OpenAIMessage, OpenAITool
+from generate.chat_completion.message.converter import MessageConverter
+from generate.chat_completion.message.core import Messages
+from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput, FinishReason, Usage
+from generate.chat_completion.models.openai_like import OpenAILikeChat, OpenAITool
+from generate.chat_completion.tool import SupportToolCall
 from generate.http import (
     HttpClient,
     HttpxPostKwargs,
 )
 from generate.model import ModelParameters, RemoteModelParametersDict
 from generate.platforms.minimax import MinimaxSettings
 from generate.types import Probability, Temperature
@@ -40,93 +42,80 @@
     temperature: Optional[Temperature]
     top_p: Optional[Probability]
     max_tokens: Optional[PositiveInt]
     tool_choice: Optional[str]
     tools: Optional[List[OpenAITool]]
 
 
-class MinimaxChat(OpenAILikeChat):
+class MinimaxChat(OpenAILikeChat, SupportToolCall):
     model_type: ClassVar[str] = 'minimax'
-    available_models: ClassVar[List[str]] = ['abab5.5-chat', 'abab5.5s-chat', 'abab6-chat']
+    available_models: ClassVar[List[str]] = ['abab5.5-chat', 'abab5.5s-chat', 'abab6-chat', 'abab6.5-chat']
     CHAT_COMPLETION_ENDPOINT: ClassVar[str] = '/text/chatcompletion_v2'
 
     parameters: MinimaxChatParameters
     settings: MinimaxSettings
 
     def __init__(
         self,
         model: str = 'abab5.5-chat',
         parameters: MinimaxChatParameters | None = None,
         settings: MinimaxSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: MessageConverter | None = None,
     ) -> None:
         parameters = parameters or MinimaxChatParameters()
         settings = settings or MinimaxSettings()  # type: ignore
         http_client = http_client or HttpClient()
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            http_client=http_client,
+            message_converter=message_converter,
+        )
 
     @override
-    def _get_request_parameters(self, prompt: Prompt, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
-        http_kwargs = super()._get_request_parameters(prompt, stream, **kwargs)
+    def _get_request_parameters(self, messages: Messages, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
+        http_kwargs = super()._get_request_parameters(messages, stream, **kwargs)
         http_kwargs['url'] = self.settings.api_base + self.CHAT_COMPLETION_ENDPOINT
         if 'tools' in http_kwargs['json']:
             # Serialize jsonschema dict to JSON string for Minimax compatibility
             for tool in http_kwargs['json']['tools']:
                 if 'function' in tool:
                     tool['function']['parameters'] = json.dumps(tool['function']['parameters'])
             if http_kwargs['json'].get('tool_choice', None):
                 http_kwargs['json']['tool_choice'] = 'auto'
         return http_kwargs
 
     @override
-    def _determine_finish_reason(self, response: Dict[str, Any]) -> str | None:
+    def _parse_finish_reason(self, response: Dict[str, Any]) -> FinishReason | None:
         choice = response['choices'][0]
         if 'finish_reason' in choice and 'delta' not in choice:
-            return choice['finish_reason']
+            return FinishReason(choice['finish_reason'])
         return None
 
     @override
-    def _convert_to_openai_messages(self, messages: Messages) -> List[OpenAIMessage]:
-        converted_messages = []
-        temp_tool_call_id = self.generate_tool_call_id()
-        for message in messages:
-            # Convert FunctionMessage to ToolMessage with self-generated tool_call_id
-            if isinstance(message, AssistantMessage):
-                if message.function_call is not None:
-                    tool_call = ToolCall(
-                        id=temp_tool_call_id,
-                        function=message.function_call,
-                    )
-                    message.tool_calls = [tool_call]
-                    message.function_call = None
-            elif isinstance(message, FunctionMessage):
-                tool_message = ToolMessage(
-                    name=message.name,
-                    content=message.content,
-                    tool_call_id=temp_tool_call_id,
-                )
-                temp_tool_call_id = self.generate_tool_call_id()
-                converted_messages.append(tool_message)
-                continue
-            converted_messages.append(message.model_copy(deep=True))
-        return super()._convert_to_openai_messages(converted_messages)
+    def _parse_usage(self, response: dict[str, Any]) -> Usage:
+        if usage := response.get('usage'):
+            return Usage(input_tokens=0, output_tokens=usage['total_tokens'])
+        return Usage()
 
     @override
     def generate(self, prompt: Prompt, **kwargs: Unpack[MinimaxChatParametersDict]) -> ChatCompletionOutput:
-        return super().generate(prompt, **kwargs)
+        return super().generate(prompt, **kwargs)  # type: ignore
 
     @override
     async def async_generate(self, prompt: Prompt, **kwargs: Unpack[MinimaxChatParametersDict]) -> ChatCompletionOutput:
-        return await super().async_generate(prompt, **kwargs)
+        return await super().async_generate(prompt, **kwargs)  # type: ignore
 
     @override
     def stream_generate(
         self, prompt: Prompt, **kwargs: Unpack[MinimaxChatParametersDict]
     ) -> Iterator[ChatCompletionStreamOutput]:
-        yield from super().stream_generate(prompt, **kwargs)
+        yield from super().stream_generate(prompt, **kwargs)  # type: ignore
 
     @override
     async def async_stream_generate(
         self, prompt: Prompt, **kwargs: Unpack[MinimaxChatParametersDict]
     ) -> AsyncIterator[ChatCompletionStreamOutput]:
-        async for stream_output in super().async_stream_generate(prompt, **kwargs):
+        async for stream_output in super().async_stream_generate(prompt, **kwargs):  # type: ignore
             yield stream_output
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/minimax_pro.py` & `generate_core-0.5.0b0/generate/chat_completion/models/openai_like.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,381 +1,371 @@
 from __future__ import annotations
 
-import json
-from typing import Any, AsyncIterator, ClassVar, Dict, Iterator, List, Literal, Optional, cast
+import base64
+from typing import Any, AsyncIterator, Dict, Iterator, List, Literal, Optional, Union, cast
 
-from pydantic import Field, PositiveInt, model_validator
-from typing_extensions import Annotated, NotRequired, Self, TypedDict, Unpack, override
+from pydantic import Field, PositiveInt
+from typing_extensions import Annotated, NotRequired, TypedDict, override
 
 from generate.chat_completion.base import RemoteChatCompletionModel
 from generate.chat_completion.message import (
     AssistantMessage,
     FunctionCall,
     FunctionMessage,
-    Message,
-    MessageTypeError,
-    MessageValueError,
-    Prompt,
+    ImagePart,
     SystemMessage,
+    TextPart,
+    ToolCall,
+    ToolMessage,
     UserMessage,
-    ensure_messages,
+    UserMultiPartMessage,
 )
-from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput, Stream
+from generate.chat_completion.message.converter import MessageConverter
+from generate.chat_completion.message.core import Messages, Prompt
+from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput, FinishReason, Usage
 from generate.chat_completion.stream_manager import StreamManager
-from generate.chat_completion.tool import FunctionJsonSchema, Tool, ToolCallMixin
+from generate.chat_completion.tool import FunctionJsonSchema, SupportToolCall, Tool
 from generate.http import (
     HttpClient,
+    HttpGetKwargs,
     HttpxPostKwargs,
-    ResponseValue,
-    UnexpectedResponseError,
 )
 from generate.model import ModelInfo, ModelParameters, RemoteModelParametersDict
-from generate.platforms.minimax import MinimaxSettings
+from generate.platforms.openai_like import OpenAILikeSettings
 from generate.types import OrIterable, Probability, Temperature
 from generate.utils import ensure_iterable
 
 
-class BotSettingDict(TypedDict):
-    bot_name: str
-    content: str
+class FunctionCallName(TypedDict):
+    name: str
 
 
-class GlyphDict(TypedDict):
-    type: str
-    raw_glpyh: str
-    json_properties: Dict[str, Any]
+class OpenAIFunctionCall(TypedDict):
+    name: str
+    arguments: str
 
 
-class ReplyConstrainsDict(TypedDict):
-    sender_type: str
-    sender_name: str
-    glyph: NotRequired[GlyphDict]
+class OpenAITool(TypedDict):
+    type: Literal['function']
+    function: FunctionJsonSchema
 
 
-class MinimaxFunctionCall(TypedDict):
-    name: str
-    arguments: str
+class OpenAIToolChoice(TypedDict):
+    type: Literal['function']
+    function: FunctionCallName
 
 
-class MinimaxProMessage(TypedDict):
-    sender_type: Literal['USER', 'BOT', 'FUNCTION']
-    sender_name: str
-    text: str
-    function_call: NotRequired[MinimaxFunctionCall]
+class OpenAIToolCall(TypedDict):
+    id: str
+    type: Literal['function']
+    function: OpenAIFunctionCall
 
 
-class MinimaxProChatParameters(ModelParameters):
-    reply_constraints: ReplyConstrainsDict = {'sender_type': 'BOT', 'sender_name': 'MM智能助理'}
-    bot_setting: List[BotSettingDict] = [
-        {
-            'bot_name': 'MM智能助理',
-            'content': 'MM智能助理是一款由MiniMax自研的，没有调用其他产品的接口的大型语言模型。MiniMax是一家中国科技公司，一直致力于进行大模型相关的研究。',
-        }
-    ]
+class OpenAIMessage(TypedDict):
+    role: str
+    content: Union[str, None, List[Dict[str, Any]]]
+    name: NotRequired[str]
+    function_call: NotRequired[OpenAIFunctionCall]
+    tool_call_id: NotRequired[str]
+    tool_calls: NotRequired[List[OpenAIToolCall]]
+
+
+class OpenAIResponseFormat(TypedDict):
+    type: Literal['json_object', 'text']
+
+
+class OpenAIChatParameters(ModelParameters):
     temperature: Optional[Temperature] = None
     top_p: Optional[Probability] = None
-    max_tokens: Annotated[Optional[PositiveInt], Field(serialization_alias='tokens_to_generate')] = None
-    mask_sensitive_info: Optional[bool] = None
-    sample_messages: Optional[List[MinimaxProMessage]] = None
+    max_tokens: Optional[PositiveInt] = None
     functions: Optional[List[FunctionJsonSchema]] = None
-    search: Optional[bool] = None
-    plugins: Optional[List[str]] = None
+    function_call: Union[Literal['auto'], FunctionCallName, None] = None
+    stop: Union[str, List[str], None] = None
+    presence_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
+    frequency_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
+    logit_bias: Optional[Dict[int, Annotated[int, Field(ge=-100, le=100)]]] = None
+    logprobs: Optional[bool] = None
+    top_logprobs: Optional[Annotated[int, Field(ge=0, le=20)]] = None
+    user: Optional[str] = None
+    response_format: Optional[OpenAIResponseFormat] = None
+    seed: Optional[int] = None
+    tools: Optional[List[OpenAITool]] = None
+    tool_choice: Union[Literal['auto', 'none'], OpenAIToolChoice, None] = None
 
-    @model_validator(mode='after')
-    def check_bot_name(self) -> Self:
-        names: set[str] = {bot_setting['bot_name'] for bot_setting in self.bot_setting}
-        if (sender_name := self.reply_constraints['sender_name']) not in names:
-            raise ValueError(f'reply_constraints sender_name {sender_name} must be in bot_setting names: {names}')
-        return self
-
-    @property
-    def bot_name(self) -> str | None:
-        if len(self.bot_setting) == 1:
-            return self.bot_setting[0]['bot_name']
-        return None
-
-    def set_system_prompt(self, system_prompt: str) -> None:
-        if len(self.bot_setting) == 1:
-            self.bot_setting[0]['content'] = system_prompt
-        else:
-            raise ValueError('set system_prompt is not supported when bot_setting has more than one bot')
-
-    def set_bot_name(self, bot_name: str) -> None:
-        if len(self.bot_setting) == 1:
-            self.bot_setting[0]['bot_name'] = bot_name
-            self.reply_constraints['sender_name'] = bot_name
-        else:
-            raise ValueError('set bot_name is not supported when bot_setting has more than one bot')
 
-    def custom_model_dump(self) -> dict[str, Any]:
-        output = super().custom_model_dump()
-        if 'temperature' in output:
-            output['temperature'] = max(0.01, output['temperature'])
-        if 'top_p' in output:
-            output['top_p'] = max(0.01, output['top_p'])
-        if 'search' in output:
-            original_plugins = output.get('plugins', [])
-            output['plugins'] = list(set(original_plugins + ['plugin_web_search']))
-        return output
-
-
-class MinimaxProChatParametersDict(RemoteModelParametersDict, total=False):
-    reply_constraints: ReplyConstrainsDict
-    bot_setting: List[BotSettingDict]
+class OpenAIChatParametersDict(RemoteModelParametersDict, total=False):
     temperature: Optional[Temperature]
     top_p: Optional[Probability]
     max_tokens: Optional[PositiveInt]
-    mask_sensitive_info: Optional[bool]
-    sample_messages: Optional[List[MinimaxProMessage]]
     functions: Optional[List[FunctionJsonSchema]]
-    search: Optional[bool]
-    plugins: Optional[List[str]]
+    function_call: Union[Literal['auto'], FunctionCallName, None]
+    stop: Union[str, List[str], None]
+    presence_penalty: Optional[float]
+    frequency_penalty: Optional[float]
+    logit_bias: Optional[Dict[int, int]]
+    logprobs: Optional[bool]
+    top_logprobs: Optional[int]
+    user: Optional[str]
+    response_format: Optional[OpenAIResponseFormat]
+    seed: Optional[int]
+    tools: Optional[List[OpenAITool]]
+    tool_choice: Union[Literal['auto'], OpenAIToolChoice, None]
 
 
-def _convert_to_minimax_pro_message(
-    message: Message, default_bot_name: str | None = None, default_user_name: str = '用户'
-) -> MinimaxProMessage:
-    if isinstance(message, UserMessage):
-        sender_name = message.name or default_user_name
-        return {'sender_type': 'USER', 'sender_name': sender_name, 'text': message.content}
-
-    if isinstance(message, AssistantMessage):
-        sender_name = message.name or default_bot_name
-        if sender_name is None:
-            raise MessageValueError(message, 'bot name is required')
-        if message.function_call is None:
-            return {
-                'sender_type': 'BOT',
-                'sender_name': sender_name,
-                'text': message.content,
-            }
+class SupportOpenAIToolCall(SupportToolCall):
+    parameters: ModelParameters
+
+    @override
+    def add_tools(self, tools: OrIterable[Tool]) -> None:
+        new_tools = [OpenAITool(type='function', function=tool.json_schema) for tool in ensure_iterable(tools)]
+        if not hasattr(self.parameters, 'tools'):
+            raise ValueError('The parameters must have a tools attribute')
+        self.parameters = cast(OpenAIChatParameters, self.parameters)
+        if self.parameters.tools is None:
+            self.parameters.tools = new_tools
+        else:
+            self.parameters.tools.extend(new_tools)
+
+
+class OpenAIMessageConverter(MessageConverter):
+    allowed_message_types = [SystemMessage, UserMessage, UserMultiPartMessage, ToolMessage, AssistantMessage, FunctionMessage]
+
+    def convert_system_message(self, message: SystemMessage) -> Dict[str, Any]:
         return {
-            'sender_type': 'BOT',
-            'sender_name': sender_name,
-            'text': message.content,
-            'function_call': {
-                'name': message.function_call.name,
-                'arguments': message.function_call.arguments,
-            },
+            'role': 'system',
+            'content': message.content,
         }
 
-    if isinstance(message, FunctionMessage):
+    def convert_user_message(self, message: UserMessage) -> Dict[str, Any]:
         return {
-            'sender_type': 'FUNCTION',
-            'sender_name': message.name,
-            'text': message.content,
+            'role': 'user',
+            'content': message.content,
         }
 
-    raise MessageTypeError(message, allowed_message_type=(UserMessage, AssistantMessage, FunctionMessage))
-
-
-def _convert_to_message(message: MinimaxProMessage) -> AssistantMessage | FunctionMessage:
-    if 'function_call' in message:
-        return AssistantMessage(
-            name=message['sender_name'],
-            content=message['text'],
-            function_call=FunctionCall(name=message['function_call']['name'], arguments=message['function_call']['arguments']),
-        )
-    if message['sender_type'] == 'BOT':
-        return AssistantMessage(
-            name=message['sender_name'],
-            content=message['text'],
-        )
-    if message['sender_type'] == 'FUNCTION':
-        return FunctionMessage(
-            name=message['sender_name'],
-            content=message['text'],
-        )
-    raise ValueError(f'unknown sender_type: {message["sender_type"]}')
+    def convert_user_multi_part_message(self, message: UserMultiPartMessage) -> Dict[str, Any]:
+        content = []
+        for part in message.content:
+            if isinstance(part, TextPart):
+                content.append({'type': 'text', 'text': part.text})
+            else:
+                if isinstance(part, ImagePart):
+                    url: str = f'data:image/{part.image_format};base64,{base64.b64encode(part.image).decode()}'
+                    image_url_dict = {'url': url}
+                else:
+                    image_url_dict = {}
+                    image_url_dict['url'] = part.image_url.url
+                    if part.image_url.detail:
+                        image_url_dict['detail'] = part.image_url.detail
+                image_url_part_dict: dict[str, Any] = {
+                    'type': 'image_url',
+                    'image_url': image_url_dict,
+                }
+                content.append(image_url_part_dict)
+        return {
+            'role': 'user',
+            'content': content,
+        }
 
+    def convert_tool_message(self, message: ToolMessage) -> Dict[str, Any]:
+        return {
+            'role': 'tool',
+            'tool_call_id': message.tool_call_id,
+            'content': message.content,
+        }
 
-class _StreamResponseProcessor:
-    def __init__(self, model_info: ModelInfo) -> None:
-        self.message: AssistantMessage | None = None
-        self.model_info = model_info
-
-    def process(self, response: ResponseValue) -> ChatCompletionStreamOutput:
-        if response.get('usage'):
-            assert self.message is not None
-            return ChatCompletionStreamOutput(
-                model_info=self.model_info,
-                message=self.message,
-                finish_reason=response['choices'][0]['finish_reason'],
-                cost=minimax_calculate_cost(model_name=self.model_info.name, usage=response['usage']),
-                extra={
-                    'input_sensitive': response['input_sensitive'],
-                    'output_sensitive': response['output_sensitive'],
-                    'usage': response['usage'],
-                },
-                stream=Stream(delta='', control='finish'),
-            )
+    def convert_assistant_message(self, message: AssistantMessage) -> Dict[str, Any]:
+        base_dict = {
+            'role': 'assistant',
+            'content': message.content or None,
+        }
+        if message.tool_calls:
+            tool_calls = [
+                {
+                    'id': tool_call.id,
+                    'type': 'function',
+                    'function': {
+                        'name': tool_call.function.name,
+                        'arguments': tool_call.function.arguments,
+                    },
+                }
+                for tool_call in message.tool_calls
+            ]
+            base_dict['tool_calls'] = tool_calls
+        if message.function_call:
+            base_dict['function_call'] = {
+                'name': message.function_call.name,
+                'arguments': message.function_call.arguments,
+            }
+        return base_dict
 
-        if self.message is None:
-            self.message = self.initial_message(response)
-            delta = self.message.content if isinstance(self.message, AssistantMessage) else ''
-            control = 'start'
-        else:
-            delta = self.update_existing_message(response)
-            control = 'continue'
+    def convert_function_message(self, message: FunctionMessage) -> Dict[str, Any]:
+        return {
+            'role': 'function',
+            'name': message.name,
+            'content': message.content,
+        }
 
-        return ChatCompletionStreamOutput(
-            model_info=self.model_info,
-            message=self.message,
-            finish_reason=None,
-            stream=Stream(delta=delta, control=control),
-        )
 
-    def initial_message(self, response: ResponseValue) -> AssistantMessage:
-        output_messages = [_convert_to_message(i) for i in response['choices'][0]['messages']]
-        message = output_messages[-1]
-        return cast(AssistantMessage, message)
-
-    def update_existing_message(self, response: ResponseValue) -> str:
-        output_messages = [_convert_to_message(i) for i in response['choices'][0]['messages']]
-        message = output_messages[-1]
-        if not isinstance(message, AssistantMessage):
-            return ''
-
-        if message.function_call is not None:
-            delta = ''
-            self.message = message
-            return delta
-
-        delta = message.content
-        self.message.content += message.content  # type: ignore
-        return delta
-
-
-def minimax_calculate_cost(model_name: str, usage: dict[str, int], num_web_search: int = 0) -> float | None:
-    if model_name == 'abab6-chat':
-        model_cost = 0.1 * (usage['total_tokens'] / 1000)
-    elif model_name == 'abab5.5-chat':
-        model_cost = 0.015 * (usage['total_tokens'] / 1000)
-    elif model_name == 'abab5.5s-chat':
-        model_cost = 0.005 * (usage['total_tokens'] / 1000)
-    else:
-        return None
-    return model_cost + (0.03 * num_web_search)
-
-
-class MinimaxProChat(RemoteChatCompletionModel, ToolCallMixin):
-    model_type: ClassVar[str] = 'minimax_pro'
-    available_models: ClassVar[List[str]] = ['abab5.5-chat', 'abab5.5s-chat', 'abab6-chat']
+class OpenAILikeChat(RemoteChatCompletionModel):
+    settings: OpenAILikeSettings
 
-    parameters: MinimaxProChatParameters
-    settings: MinimaxSettings
+    message_converter: OpenAIMessageConverter
+    parameters: ModelParameters
+    settings: OpenAILikeSettings
 
     def __init__(
         self,
-        model: str = 'abab5.5-chat',
-        parameters: MinimaxProChatParameters | None = None,
-        settings: MinimaxSettings | None = None,
+        model: str,
+        parameters: ModelParameters | None = None,
+        settings: OpenAILikeSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: MessageConverter | None = None,
     ) -> None:
-        parameters = parameters or MinimaxProChatParameters()
-        settings = settings or MinimaxSettings()  # type: ignore
         http_client = http_client or HttpClient()
-        if not settings.group_id:
-            raise ValueError(
-                'group_id is required for MinimaxProChat, you can set it in settings or environment variable MINIMAX_GROUP_ID'
-            )
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
-
-        self.default_user_name = '用户'
+        message_converter = message_converter or OpenAIMessageConverter()
+        parameters = parameters or OpenAIChatParameters()
+        if settings is None:
+            raise ValueError('settings is required')
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            http_client=http_client,
+            message_converter=message_converter,
+        )
 
     @override
-    def generate(self, prompt: Prompt, **kwargs: Unpack[MinimaxProChatParametersDict]) -> ChatCompletionOutput:
+    def generate(self, prompt: Prompt, **kwargs: Any) -> ChatCompletionOutput:
         return super().generate(prompt, **kwargs)
 
     @override
-    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[MinimaxProChatParametersDict]) -> ChatCompletionOutput:
+    async def async_generate(self, prompt: Prompt, **kwargs: Any) -> ChatCompletionOutput:
         return await super().async_generate(prompt, **kwargs)
 
     @override
-    def stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[MinimaxProChatParametersDict]
-    ) -> Iterator[ChatCompletionStreamOutput]:
-        request_parameters = self._get_request_parameters(prompt, stream=True, **kwargs)
-        stream_processor = _StreamResponseProcessor(model_info=self.model_info)
-        for line in self.http_client.stream_post(request_parameters=request_parameters):
-            yield stream_processor.process(json.loads(line))
+    def stream_generate(self, prompt: Prompt, **kwargs: Any) -> Iterator[ChatCompletionStreamOutput]:
+        yield from super().stream_generate(prompt, **kwargs)
 
     @override
-    async def async_stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[MinimaxProChatParametersDict]
-    ) -> AsyncIterator[ChatCompletionStreamOutput]:
-        request_parameters = self._get_request_parameters(prompt, stream=True, **kwargs)
-        stream_processor = _StreamResponseProcessor(model_info=self.model_info)
-        async for line in self.http_client.async_stream_post(request_parameters=request_parameters):
-            yield stream_processor.process(json.loads(line))
-
-    def add_tools(self, tools: OrIterable[Tool]) -> None:
-        new_functions = [tool.json_schema for tool in ensure_iterable(tools)]
-        if self.parameters.functions is None:
-            self.parameters.functions = new_functions
-        else:
-            self.parameters.functions.extend(new_functions)
+    async def async_stream_generate(self, prompt: Prompt, **kwargs: Any) -> AsyncIterator[ChatCompletionStreamOutput]:
+        async for stream_output in super().async_stream_generate(prompt, **kwargs):
+            yield stream_output
 
     @override
-    def _process_reponse(self, response: ResponseValue) -> ChatCompletionOutput:
-        try:
-            messages: list[AssistantMessage | FunctionMessage] = [
-                _convert_to_message(i) for i in response['choices'][0]['messages']
-            ]
-            message = cast(AssistantMessage, messages[-1])
-            finish_reason = response['choices'][0]['finish_reason']
-            num_web_search = sum([1 for i in response['choices'][0]['messages'] if i['sender_name'] == 'plugin_web_search'])
-            return ChatCompletionOutput(
-                model_info=self.model_info,
-                message=message,
-                finish_reason=finish_reason,
-                cost=minimax_calculate_cost(model_name=self.name, usage=response['usage'], num_web_search=num_web_search),
-                extra={
-                    'input_sensitive': response['input_sensitive'],
-                    'output_sensitive': response['output_sensitive'],
-                    'usage': response['usage'],
-                },
-            )
-        except (KeyError, IndexError, TypeError) as e:
-            raise UnexpectedResponseError(response) from e
-
-    @override
-    def _get_request_parameters(
-        self, prompt: Prompt, stream: bool = False, **kwargs: Unpack[MinimaxProChatParametersDict]
-    ) -> HttpxPostKwargs:
-        messages = ensure_messages(prompt)
+    def _get_request_parameters(self, messages: Messages, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
         parameters = self.parameters.clone_with_changes(**kwargs)
-        if isinstance(messages[0], SystemMessage):
-            system_message = messages[0]
-            parameters.set_system_prompt(system_message.content)
-            messages = messages[1:]
-
-        minimax_pro_messages = [
-            _convert_to_minimax_pro_message(
-                message, default_bot_name=parameters.bot_name, default_user_name=self.default_user_name
-            )
-            for message in messages
-        ]
-        json_data = {'model': self.model, 'messages': minimax_pro_messages, **parameters.custom_model_dump()}
-        if stream:
-            json_data['stream'] = True
-
         headers = {
             'Authorization': f'Bearer {self.settings.api_key.get_secret_value()}',
-            'Content-Type': 'application/json',
         }
+        json_data = {
+            'model': self.model,
+            'messages': self.message_converter.convert_messages(messages),
+            **parameters.custom_model_dump(),
+        }
+        if stream:
+            json_data['stream'] = True
+
         return {
-            'url': self.settings.api_base + '/text/chatcompletion_pro',
-            'json': json_data,
+            'url': f'{self.settings.api_base}/chat/completions',
             'headers': headers,
-            'params': {'GroupId': self.settings.group_id},
+            'json': json_data,
         }
 
     @override
-    def _process_stream_line(self, line: str, stream_manager: StreamManager) -> ChatCompletionStreamOutput | None:
-        # TODO: implement this
-        raise NotImplementedError
+    def _process_reponse(self, response: dict[str, Any]) -> ChatCompletionOutput:
+        return ChatCompletionOutput(
+            model_info=ModelInfo(task='chat_completion', type=self.model_type, name=response['model']),
+            message=self._parse_assistant_message(response['choices'][0]['message']),
+            finish_reason=self._parse_finish_reason(response),
+            usage=self._parse_usage(response),
+            extra=self._parse_extra(response),
+        )
+
+    @override
+    def _process_stream_response(
+        self, response: Dict[str, Any], stream_manager: StreamManager
+    ) -> ChatCompletionStreamOutput | None:
+        delta_dict = response['choices'][0].get('delta', {})
+        self._update_delta(delta_dict, stream_manager=stream_manager)
+        stream_manager.extra = self._parse_extra(response)
+        stream_manager.usage = self._parse_usage(response)
+        stream_manager.finish_reason = self._parse_finish_reason(response)
+        return stream_manager.build_stream_output()
+
+    def _parse_assistant_message(self, message: dict[str, Any]) -> AssistantMessage:
+        if function_call_dict := message.get('function_call'):
+            function_call = FunctionCall(
+                name=function_call_dict.get('name') or '',
+                arguments=function_call_dict['arguments'],
+            )
+        else:
+            function_call = None
+
+        if tool_calls_dict := message.get('tool_calls'):
+            tool_calls = [
+                ToolCall(
+                    id=tool_call['id'],
+                    function=FunctionCall(
+                        name=tool_call['function'].get('name') or '',
+                        arguments=tool_call['function']['arguments'],
+                    ),
+                )
+                for tool_call in tool_calls_dict
+            ]
+        else:
+            tool_calls = None
+        return AssistantMessage(content=message.get('content') or '', function_call=function_call, tool_calls=tool_calls)
 
-    @classmethod
     @override
-    def from_name(cls, name: str) -> Self:
-        return cls(model=name)
+    def list_models(self) -> List[str]:
+        headers = {
+            'Accept': 'application/json',
+            'Authorization': f'Bearer {self.settings.api_key.get_secret_value()}',
+        }
+        parameters: HttpGetKwargs = {
+            'url': f'{self.settings.api_base}/models',
+            'headers': headers,
+        }
+        response = self.http_client.get(parameters)
+        self.http_client.raise_for_status(response)
+        return [i['id'] for i in response.json()['data'] if i['object'] == 'model']
+
+    def _parse_finish_reason(self, response: dict[str, Any]) -> FinishReason | None:
+        choice = response['choices'][0]
+        finish_reason = choice.get('finish_reason') or None
+        if finish_reason is None:
+            finish_reason: str | None = finish_details['type'] if (finish_details := choice.get('finish_details')) else None
+        if finish_reason is not None:
+            finish_reason = FinishReason(finish_reason)
+        return finish_reason
+
+    def _parse_usage(self, response: dict[str, Any]) -> Usage:
+        if usage := response.get('usage'):
+            input_tokens = usage['prompt_tokens']
+            output_tokens = usage['completion_tokens']
+            return Usage(input_tokens=input_tokens, output_tokens=output_tokens)
+        return Usage()
+
+    def _parse_extra(self, response: dict[str, Any]) -> dict[str, Any]:
+        return {'response': response}
+
+    def _update_delta(self, delta_dict: dict[str, Any], stream_manager: StreamManager) -> None:
+        delta_content: str = delta_dict.get('content') or ''
+        stream_manager.delta = delta_content
+
+        if delta_dict.get('tool_calls'):
+            tool_calls = delta_dict['tool_calls'][0]
+            index = tool_calls['index']
+            if index >= len(stream_manager.tool_calls or []):
+                new_tool_calls_message = self._parse_assistant_message(delta_dict).tool_calls
+                if new_tool_calls_message:
+                    stream_manager.tool_calls.append(new_tool_calls_message[0])
+            else:
+                stream_manager.tool_calls[index].function.arguments += tool_calls['function']['arguments']
+
+        if delta_dict.get('function_call'):
+            if stream_manager.function_call is None:
+                stream_manager.function_call = FunctionCall(name='', arguments='')
+            function_name = delta_dict['function_call'].get('name', '')
+            stream_manager.function_call.name += function_name
+            arguments = delta_dict['function_call'].get('arguments', '')
+            stream_manager.function_call.arguments += arguments
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/moonshot.py` & `generate_core-0.5.0b0/generate/chat_completion/models/moonshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class MoonshotChatParameters(ModelParameters):
     temperature: Optional[Temperature] = None
     top_p: Optional[Probability] = None
     max_tokens: Optional[PositiveInt] = None
 
 
-class MoonshotParametersDict(RemoteModelParametersDict, total=False):
+class MoonshotChatParametersDict(RemoteModelParametersDict, total=False):
     temperature: Temperature
     top_p: Probability
     max_tokens: PositiveInt
 
 
 class MoonshotChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'moonshot'
@@ -43,24 +43,26 @@
         parameters = parameters or MoonshotChatParameters()
         settings = settings or MoonshotSettings()  # type: ignore
         http_client = http_client or HttpClient()
         model = model
         super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
 
     @override
-    def generate(self, prompt: Prompt, **kwargs: Unpack[MoonshotParametersDict]) -> ChatCompletionOutput:
+    def generate(self, prompt: Prompt, **kwargs: Unpack[MoonshotChatParametersDict]) -> ChatCompletionOutput:
         return super().generate(prompt, **kwargs)
 
     @override
-    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[MoonshotParametersDict]) -> ChatCompletionOutput:
+    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[MoonshotChatParametersDict]) -> ChatCompletionOutput:
         return await super().async_generate(prompt, **kwargs)
 
     @override
-    def stream_generate(self, prompt: Prompt, **kwargs: Unpack[MoonshotParametersDict]) -> Iterator[ChatCompletionStreamOutput]:
+    def stream_generate(
+        self, prompt: Prompt, **kwargs: Unpack[MoonshotChatParametersDict]
+    ) -> Iterator[ChatCompletionStreamOutput]:
         yield from super().stream_generate(prompt, **kwargs)
 
     @override
     async def async_stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[MoonshotParametersDict]
+        self, prompt: Prompt, **kwargs: Unpack[MoonshotChatParametersDict]
     ) -> AsyncIterator[ChatCompletionStreamOutput]:
         async for stream_output in super().async_stream_generate(prompt, **kwargs):
             yield stream_output
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/openai.py` & `generate_core-0.5.0b0/generate/chat_completion/models/openrouter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,132 @@
 from __future__ import annotations
 
-from typing import AsyncIterator, ClassVar, Dict, Iterator, List, Literal, Optional, Union
+from typing import Any, AsyncIterator, ClassVar, Dict, Iterator, List, Literal, Optional, Union
 
-from pydantic import Field, PositiveInt
+from pydantic import BaseModel, Field, PositiveInt
 from typing_extensions import Annotated, Unpack, override
 
 from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.core import Messages
 from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
 from generate.chat_completion.models.openai_like import (
-    FunctionCallName,
     OpenAILikeChat,
     OpenAIResponseFormat,
     OpenAITool,
     OpenAIToolChoice,
-    convert_to_openai_tool,
-)
-from generate.chat_completion.tool import FunctionJsonSchema, Tool, ToolCallMixin
-from generate.http import (
-    HttpClient,
+    SupportOpenAIToolCall,
 )
+from generate.http import HttpClient, HttpxPostKwargs
 from generate.model import ModelParameters, RemoteModelParametersDict
-from generate.platforms.openai import OpenAISettings
-from generate.types import OrIterable, Probability, Temperature
-from generate.utils import ensure_iterable
+from generate.platforms import OpenRouterSettings
+from generate.types import Probability, Temperature
+
+
+class ProviderParameters(BaseModel):
+    allow_fallbacks: bool = True
+    require_parameters: bool = False
+    data_collection: str = 'allow'
+    order: Optional[List[str]] = None
 
 
-class OpenAIChatParameters(ModelParameters):
+class OpenRouterChatParameters(ModelParameters):
     temperature: Optional[Temperature] = None
     top_p: Optional[Probability] = None
+    top_k: Optional[PositiveInt] = None
     max_tokens: Optional[PositiveInt] = None
-    functions: Optional[List[FunctionJsonSchema]] = None
-    function_call: Union[Literal['auto'], FunctionCallName, None] = None
     stop: Union[str, List[str], None] = None
     presence_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
     frequency_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
+    repetition_penalty: Optional[Annotated[float, Field(ge=0.0, le=2.0)]] = None
     logit_bias: Optional[Dict[int, Annotated[int, Field(ge=-100, le=100)]]] = None
     user: Optional[str] = None
     response_format: Optional[OpenAIResponseFormat] = None
     seed: Optional[int] = None
     tools: Optional[List[OpenAITool]] = None
-    tool_choice: Union[Literal['auto'], OpenAIToolChoice, None] = None
+    tool_choice: Union[Literal['auto', 'none'], OpenAIToolChoice, None] = None
+    route: Optional[str] = None
+    transforms: Optional[List[str]] = None
+    provider: Optional[ProviderParameters] = None
 
 
-class OpenAIChatParametersDict(RemoteModelParametersDict, total=False):
+class OpenRouterParametersDict(RemoteModelParametersDict, total=False):
     temperature: Optional[Temperature]
     top_p: Optional[Probability]
+    top_k: Optional[PositiveInt]
     max_tokens: Optional[PositiveInt]
-    functions: Optional[List[FunctionJsonSchema]]
-    function_call: Union[Literal['auto'], FunctionCallName, None]
     stop: Union[str, List[str], None]
     presence_penalty: Optional[float]
     frequency_penalty: Optional[float]
+    repetition_penalty: Optional[float]
     logit_bias: Optional[Dict[int, int]]
     user: Optional[str]
     response_format: Optional[OpenAIResponseFormat]
     seed: Optional[int]
     tools: Optional[List[OpenAITool]]
-    tool_choice: Union[Literal['auto'], OpenAIToolChoice, None]
+    tool_choice: Union[Literal['auto', 'none'], OpenAIToolChoice, None]
+    route: Optional[str]
+    transforms: Optional[List[str]]
+    provider: ProviderParameters
 
 
-class OpenAIChat(OpenAILikeChat, ToolCallMixin):
-    model_type: ClassVar[str] = 'openai'
-    available_models: ClassVar[List[str]] = [
-        'gpt-4-turbo-preview',
-        'gpt-3.5-turbo',
-        'gpt-4-vision-preview',
-    ]
+class OpenRouterChat(OpenAILikeChat, SupportOpenAIToolCall):
+    model_type: ClassVar[str] = 'openrouter'
+    available_models: ClassVar[List[str]] = ['auto']
 
-    parameters: OpenAIChatParameters
-    settings: OpenAISettings
+    parameters: OpenRouterChatParameters
+    settings: OpenRouterSettings
 
     def __init__(
         self,
-        model: str = 'gpt-3.5-turbo',
-        parameters: OpenAIChatParameters | None = None,
-        settings: OpenAISettings | None = None,
+        model: str | list[str] = 'auto',
+        parameters: OpenRouterChatParameters | None = None,
+        settings: OpenRouterSettings | None = None,
         http_client: HttpClient | None = None,
+        app_name: str | None = None,
+        site_url: str | None = None,
     ) -> None:
-        parameters = parameters or OpenAIChatParameters()
-        settings = settings or OpenAISettings()  # type: ignore
+        parameters = parameters or OpenRouterChatParameters()
+        settings = settings or OpenRouterSettings()  # type: ignore
         http_client = http_client or HttpClient()
+        if isinstance(model, list):
+            self.models = model
+            model = '-'.join(model[:3])
+            if len(model) > 3:
+                model += '-etc'
+        else:
+            self.models = None
         super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
+        self.app_name = app_name
+        self.site_url = site_url
 
     @override
-    def generate(self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]) -> ChatCompletionOutput:
-        return super().generate(prompt, **kwargs)
+    def generate(self, prompt: Prompt, **kwargs: Unpack[OpenRouterParametersDict]) -> ChatCompletionOutput:
+        return super().generate(prompt, **kwargs)  # type: ignore
 
     @override
-    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]) -> ChatCompletionOutput:
-        return await super().async_generate(prompt, **kwargs)
+    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[OpenRouterParametersDict]) -> ChatCompletionOutput:
+        return await super().async_generate(prompt, **kwargs)  # type: ignore
 
     @override
     def stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]
+        self, prompt: Prompt, **kwargs: Unpack[OpenRouterParametersDict]
     ) -> Iterator[ChatCompletionStreamOutput]:
-        yield from super().stream_generate(prompt, **kwargs)
+        yield from super().stream_generate(prompt, **kwargs)  # type: ignore
 
     @override
     async def async_stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[OpenAIChatParametersDict]
+        self, prompt: Prompt, **kwargs: Unpack[OpenRouterParametersDict]
     ) -> AsyncIterator[ChatCompletionStreamOutput]:
-        async for stream_output in super().async_stream_generate(prompt, **kwargs):
+        async for stream_output in super().async_stream_generate(prompt, **kwargs):  # type: ignore
             yield stream_output
 
     @override
-    def add_tools(self, tools: OrIterable[Tool]) -> None:
-        new_tools = [convert_to_openai_tool(tool) for tool in ensure_iterable(tools)]
-        if self.parameters.tools is None:
-            self.parameters.tools = new_tools
-        else:
-            self.parameters.tools.extend(new_tools)
+    def _get_request_parameters(self, messages: Messages, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
+        request_parameters: HttpxPostKwargs = super()._get_request_parameters(messages, stream=stream, **kwargs)
+        if self.app_name:
+            request_parameters['headers']['X-Title'] = self.app_name
+        if self.site_url:
+            request_parameters['headers']['HTTP-Referer'] = self.site_url
+        if self.models:
+            request_parameters['json']['models'] = self.models
+            request_parameters['json'].pop('model')
+        return request_parameters
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/openai_like.py` & `generate_core-0.5.0b0/generate/chat_completion/models/zhipu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,376 +1,381 @@
 from __future__ import annotations
 
 import base64
-import json
-import uuid
-from abc import ABC
-from functools import partial
-from typing import Any, Callable, Dict, List, Literal, Type, Union, cast
+from typing import Any, AsyncIterator, ClassVar, Dict, Iterator, List, Literal, Optional, Union
 
-from typing_extensions import NotRequired, TypedDict, override
+from pydantic import field_validator
+from typing_extensions import NotRequired, TypedDict, Unpack, override
 
 from generate.chat_completion.base import RemoteChatCompletionModel
-from generate.chat_completion.cost_caculator import GeneralCostCalculator
 from generate.chat_completion.message import (
     AssistantMessage,
     FunctionCall,
-    FunctionMessage,
     ImagePart,
-    Message,
-    MessageTypeError,
+    ImageUrlPart,
+    Messages,
     Prompt,
     SystemMessage,
     TextPart,
     ToolCall,
     ToolMessage,
     UserMessage,
     UserMultiPartMessage,
-    ensure_messages,
 )
-from generate.chat_completion.message.core import Messages
-from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
+from generate.chat_completion.message.converter import MessageConverter
+from generate.chat_completion.message.core import FunctionMessage
+from generate.chat_completion.message.exception import MessageTypeError
+from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput, FinishReason, Usage
 from generate.chat_completion.stream_manager import StreamManager
-from generate.chat_completion.tool import FunctionJsonSchema, Tool
+from generate.chat_completion.tool import SupportToolCall, Tool
 from generate.http import (
+    HttpClient,
     HttpxPostKwargs,
     ResponseValue,
 )
-from generate.model import ModelInfo
-from generate.platforms.openai_like import OpenAILikeSettings
+from generate.model import ModelParameters, RemoteModelParametersDict
+from generate.platforms.zhipu import ZhipuSettings, generate_zhipu_token
+from generate.types import JsonSchema, OrIterable, Probability, Temperature
+from generate.utils import ensure_iterable
+
+ZhipuModelPrice = {
+    'glm-4v': (100, 100),
+    'glm-4': (100, 100),
+    'glm-3-turbo': (5, 5),
+}
 
 
-class FunctionCallName(TypedDict):
+class Function(TypedDict):
     name: str
+    description: str
+    parameters: NotRequired[JsonSchema]
 
 
-class OpenAIFunctionCall(TypedDict):
-    name: str
-    arguments: str
+class Retrieval(TypedDict):
+    knowledge_id: str
+    prompt_template: NotRequired[str]
 
 
-class OpenAITool(TypedDict):
-    type: Literal['function']
-    function: FunctionJsonSchema
+class WebSearch(TypedDict):
+    enable: NotRequired[bool]
+    search_query: NotRequired[str]
 
 
-class OpenAIToolChoice(TypedDict):
+class ZhipuFunctionTool(TypedDict):
     type: Literal['function']
-    function: FunctionCallName
+    function: Function
+
+
+class ZhipuRetrievalTool(TypedDict):
+    type: Literal['retrieval']
+    retrieval: Retrieval
+
+
+class ZhipuWebSearchTool(TypedDict):
+    type: Literal['web_search']
+    web_search: WebSearch
+
+
+ZhipuTool = Union[ZhipuFunctionTool, ZhipuRetrievalTool, ZhipuWebSearchTool]
+
 
+class ZhipuChatParameters(ModelParameters):
+    temperature: Optional[Temperature] = None
+    top_p: Optional[Probability] = None
+    do_sample: Optional[bool] = None
+    request_id: Optional[str] = None
+    max_tokens: Optional[int] = None
+    stop: Optional[List[str]] = None
+    tools: Optional[List[ZhipuTool]] = None
+    tool_choice: Optional[str] = None
 
-class OpenAIToolCall(TypedDict):
+    @field_validator('temperature')
+    @classmethod
+    def can_not_equal_zero(cls, v: Optional[Temperature]) -> Optional[Temperature]:
+        if v == 0:
+            return 0.01
+        if v == 1:
+            return 0.99
+        return v
+
+
+class ZhipuChatParametersDict(RemoteModelParametersDict, total=False):
+    temperature: Optional[Temperature]
+    top_p: Optional[Probability]
+    request_id: Optional[str]
+    max_tokens: Optional[int]
+    stop: Optional[list[str]]
+    tools: Optional[list[ZhipuTool]]
+    tool_choice: Optional[str]
+
+
+class ZhipuToolCall(TypedDict):
     id: str
-    type: Literal['function']
-    function: OpenAIFunctionCall
+    type: str
+    index: int
+    function: NotRequired[ZhipuFunctionCall]
 
 
-class OpenAIMessage(TypedDict):
-    role: str
-    content: Union[str, None, List[Dict[str, Any]]]
-    name: NotRequired[str]
-    function_call: NotRequired[OpenAIFunctionCall]
-    tool_call_id: NotRequired[str]
-    tool_calls: NotRequired[List[OpenAIToolCall]]
+class ZhipuFunctionCall(TypedDict):
+    name: str
+    arguments: str
 
 
-class OpenAIResponseFormat(TypedDict):
-    type: Literal['json_object', 'text']
+class ZhipuMessage(TypedDict):
+    role: Literal['user', 'assistant', 'system', 'tool']
+    content: NotRequired[Union[str, List[Dict[str, str]]]]
+    tool_calls: NotRequired[list[ZhipuToolCall]]
+    tool_call_id: NotRequired[str]
 
 
-def _to_text_message_dict(role: str, message: Message) -> OpenAIMessage:
-    if not isinstance(message.content, str):
-        raise TypeError(f'Unexpected message content: {type(message.content)}')
-    return {
-        'role': role,
-        'content': message.content,
-    }
+class ZhipuMessageConverter(MessageConverter):
+    allowed_message_types = [SystemMessage, UserMessage, AssistantMessage, ToolMessage, UserMultiPartMessage]
 
+    def convert_system_message(self, message: SystemMessage) -> Dict[str, Any]:
+        return {
+            'role': 'system',
+            'content': message.content,
+        }
 
-def _to_user_multipart_message_dict(message: UserMultiPartMessage) -> OpenAIMessage:
-    content = []
-    for part in message.content:
-        if isinstance(part, TextPart):
-            content.append({'type': 'text', 'text': part.text})
-        else:
-            if isinstance(part, ImagePart):
-                image_format = part.image_format or 'png'
-                url: str = f'data:image/{image_format};base64,{base64.b64encode(part.image).decode()}'
-                image_url_dict = {'url': url}
-            else:
-                image_url_dict = {}
-                image_url_dict['url'] = part.image_url.url
-                if part.image_url.detail:
-                    image_url_dict['detail'] = part.image_url.detail
-            image_url_part_dict: dict[str, Any] = {
-                'type': 'image_url',
-                'image_url': image_url_dict,
-            }
-            content.append(image_url_part_dict)
-    return {
-        'role': 'user',
-        'content': content,
-    }
-
-
-def _to_tool_message_dict(message: ToolMessage) -> OpenAIMessage:
-    return {
-        'role': 'tool',
-        'tool_call_id': message.tool_call_id,
-        'content': message.content,
-    }
-
-
-def _to_asssistant_message_dict(message: AssistantMessage) -> OpenAIMessage:
-    base_dict = {
-        'role': 'assistant',
-        'content': message.content or None,
-    }
-    if message.tool_calls:
-        tool_calls = [
-            {
-                'id': tool_call.id,
-                'type': 'function',
-                'function': {
-                    'name': tool_call.function.name,
-                    'arguments': tool_call.function.arguments,
-                },
+    def convert_user_message(self, message: UserMessage) -> Dict[str, Any]:
+        return {
+            'role': 'user',
+            'content': message.content,
+        }
+
+    def convert_assistant_message(self, message: AssistantMessage) -> Dict[str, Any]:
+        if message.tool_calls is not None:
+            dict_format_toll_calls: list[ZhipuToolCall] = []
+            for index, tool_call in enumerate(message.tool_calls):
+                tool_type = tool_call.type
+                if tool_type not in {'function', 'retrieval', 'web_search'}:
+                    raise ValueError(f'invalid tool type: {tool_type}, should be one of function, retrieval, web_search')
+                dict_format_toll_call: ZhipuToolCall = {
+                    'id': tool_call.id,
+                    'type': tool_type,
+                    'index': index,
+                }
+                if tool_type == 'function':
+                    function_dict: ZhipuFunctionCall = {
+                        'name': tool_call.function.name,
+                        'arguments': tool_call.function.arguments,
+                    }
+                    dict_format_toll_call['function'] = function_dict
+                dict_format_toll_calls.append(dict_format_toll_call)
+            return {
+                'role': 'assistant',
+                'tool_calls': dict_format_toll_calls,
             }
-            for tool_call in message.tool_calls
-        ]
-        base_dict['tool_calls'] = tool_calls
-    if message.function_call:
-        base_dict['function_call'] = {
-            'name': message.function_call.name,
-            'arguments': message.function_call.arguments,
+        return {
+            'role': 'assistant',
+            'content': message.content,
         }
-    return cast(OpenAIMessage, base_dict)
 
+    def convert_tool_message(self, message: ToolMessage) -> Dict[str, Any]:
+        return {
+            'role': 'tool',
+            'content': message.content or '',
+            'tool_call_id': message.tool_call_id,
+        }
 
-def _to_function_message_dict(message: FunctionMessage) -> OpenAIMessage:
-    return {
-        'role': 'function',
-        'name': message.name,
-        'content': message.content,
-    }
-
-
-def convert_to_openai_message(message: Message) -> OpenAIMessage:
-    to_function_map: dict[Type[Message], Callable[[Any], OpenAIMessage]] = {
-        SystemMessage: partial(_to_text_message_dict, 'system'),
-        UserMessage: partial(_to_text_message_dict, 'user'),
-        AssistantMessage: partial(_to_asssistant_message_dict),
-        UserMultiPartMessage: _to_user_multipart_message_dict,
-        ToolMessage: _to_tool_message_dict,
-        FunctionMessage: _to_function_message_dict,
-    }
-    if to_function := to_function_map.get(type(message)):
-        return to_function(message)
-
-    raise MessageTypeError(message, allowed_message_type=tuple(to_function_map.keys()))
-
-
-def openai_calculate_cost(model_name: str, input_tokens: int, output_tokens: int) -> float | None:
-    dollar_to_yuan = 7
-    if model_name in ('gpt-4-1106-preview', 'gpt-4-1106-vision-preview'):
-        return (0.01 * dollar_to_yuan) * (input_tokens / 1000) + (0.03 * dollar_to_yuan) * (output_tokens / 1000)
-    if 'gpt-4-turbo' in model_name:
-        return (0.01 * dollar_to_yuan) * (input_tokens / 1000) + (0.03 * dollar_to_yuan) * (output_tokens / 1000)
-    if 'gpt-4-32k' in model_name:
-        return (0.06 * dollar_to_yuan) * (input_tokens / 1000) + (0.12 * dollar_to_yuan) * (output_tokens / 1000)
-    if 'gpt-4' in model_name:
-        return (0.03 * dollar_to_yuan) * (input_tokens / 1000) + (0.06 * dollar_to_yuan) * (output_tokens / 1000)
-    if 'gpt-3.5-turbo' in model_name:
-        return (0.001 * dollar_to_yuan) * (input_tokens / 1000) + (0.002 * dollar_to_yuan) * (output_tokens / 1000)
-    if 'moonshot' in model_name:
-        if '8k' in model_name:
-            return 0.012 * (input_tokens / 1000) + 0.012 * (output_tokens / 1000)
-        if '32k' in model_name:
-            return 0.024 * (input_tokens / 1000) + 0.024 * (output_tokens / 1000)
-        if '128k' in model_name:
-            return 0.06 * (input_tokens / 1000) + 0.06 * (output_tokens / 1000)
-    return None
-
-
-def _convert_to_assistant_message(message: dict[str, Any]) -> AssistantMessage:
-    if function_call_dict := message.get('function_call'):
-        function_call = FunctionCall(
-            name=function_call_dict.get('name') or '',
-            arguments=function_call_dict['arguments'],
+    def convert_function_message(self, message: FunctionMessage) -> Dict[str, Any]:
+        raise MessageTypeError(message, allowed_message_type=self.allowed_message_types)
+
+    def convert_user_multi_part_message(self, message: UserMultiPartMessage) -> Dict[str, Any]:
+        content = []
+        for part in message.content:
+            if isinstance(part, TextPart):
+                content.append(
+                    {
+                        'type': 'text',
+                        'text': part.text,
+                    }
+                )
+            elif isinstance(part, ImageUrlPart):
+                content.append(
+                    {
+                        'type': 'image_url',
+                        'image_url': {
+                            'url': part.image_url.url,
+                        },
+                    }
+                )
+            elif isinstance(part, ImagePart):
+                content.append(
+                    {
+                        'type': 'image_url',
+                        'image_url': {
+                            'url': base64.b64encode(part.image).decode(),
+                        },
+                    }
+                )
+        return {'role': 'user', 'content': content}
+
+
+class ZhipuChat(RemoteChatCompletionModel, SupportToolCall):
+    model_type: ClassVar[str] = 'zhipu'
+    available_models: ClassVar[List[str]] = ['glm-4', 'glm-3-turbo', 'glm-4v']
+
+    parameters: ZhipuChatParameters
+    settings: ZhipuSettings
+
+    def __init__(
+        self,
+        model: str = 'glm-4',
+        parameters: ZhipuChatParameters | None = None,
+        settings: ZhipuSettings | None = None,
+        http_client: HttpClient | None = None,
+        message_converter: ZhipuMessageConverter | None = None,
+    ) -> None:
+        parameters = parameters or ZhipuChatParameters()
+        settings = settings or ZhipuSettings()  # type: ignore
+        http_client = http_client or HttpClient()
+        message_converter = message_converter or ZhipuMessageConverter()
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            http_client=http_client,
+            message_converter=message_converter,
         )
-    else:
-        function_call = None
 
-    if tool_calls_dict := message.get('tool_calls'):
-        tool_calls = [
-            ToolCall(
-                id=tool_call['id'],
-                function=FunctionCall(
-                    name=tool_call['function'].get('name') or '',
-                    arguments=tool_call['function']['arguments'],
-                ),
-            )
-            for tool_call in tool_calls_dict
-        ]
-    else:
-        tool_calls = None
-    return AssistantMessage(content=message.get('content') or '', function_call=function_call, tool_calls=tool_calls)
-
-
-def convert_to_openai_tool(tool: Tool) -> OpenAITool:
-    return OpenAITool(type='function', function=tool.json_schema)
-
-
-def process_openai_like_model_reponse(response: ResponseValue, model_type: str) -> ChatCompletionOutput:
-    message = _convert_to_assistant_message(response['choices'][0]['message'])
-    extra = {'usage': response['usage']}
-    if system_fingerprint := response.get('system_fingerprint'):
-        extra['system_fingerprint'] = system_fingerprint
-
-    choice = response['choices'][0]
-    if (finish_reason := choice.get('finish_reason')) is None:
-        finish_reason = finish_details['type'] if (finish_details := choice.get('finish_details')) else None
-
-    try:
-        if model_type == 'openai':
-            cost = openai_calculate_cost(
-                model_name=response['model'],
-                input_tokens=response['usage']['prompt_tokens'],
-                output_tokens=response['usage']['completion_tokens'],
-            )
-        else:
-            cost_calculator = GeneralCostCalculator()
-            cost = cost_calculator.calculate(
-                model_type=model_type,
-                model_name=response['model'],
-                input_tokens=response['usage']['prompt_tokens'],
-                output_tokens=response['usage']['completion_tokens'],
-            )
-    except Exception:
-        cost = None
+    @override
+    def generate(self, prompt: Prompt, **kwargs: Unpack[ZhipuChatParametersDict]) -> ChatCompletionOutput:
+        return super().generate(prompt, **kwargs)
 
-    return ChatCompletionOutput(
-        model_info=ModelInfo(task='chat_completion', type=model_type, name=response['model']),
-        message=message,
-        finish_reason=finish_reason,
-        cost=cost,
-        extra=extra,
-    )
+    @override
+    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[ZhipuChatParametersDict]) -> ChatCompletionOutput:
+        return await super().async_generate(prompt, **kwargs)
 
+    @override
+    def stream_generate(
+        self, prompt: Prompt, **kwargs: Unpack[ZhipuChatParametersDict]
+    ) -> Iterator[ChatCompletionStreamOutput]:
+        yield from super().stream_generate(prompt, **kwargs)
 
-class OpenAILikeChat(RemoteChatCompletionModel, ABC):
-    settings: OpenAILikeSettings
+    @override
+    async def async_stream_generate(
+        self, prompt: Prompt, **kwargs: Unpack[ZhipuChatParametersDict]
+    ) -> AsyncIterator[ChatCompletionStreamOutput]:
+        async for stream_output in super().async_stream_generate(prompt, **kwargs):
+            yield stream_output
 
     @override
-    def _get_request_parameters(self, prompt: Prompt, stream: bool = False, **kwargs: Any) -> HttpxPostKwargs:
-        messages = ensure_messages(prompt)
+    def _get_request_parameters(
+        self, messages: Messages, stream: bool = False, **kwargs: Unpack[ZhipuChatParametersDict]
+    ) -> HttpxPostKwargs:
         parameters = self.parameters.clone_with_changes(**kwargs)
-        openai_messages = self._convert_to_openai_messages(messages)
         headers = {
-            'Authorization': f'Bearer {self.settings.api_key.get_secret_value()}',
+            'Authorization': generate_zhipu_token(self.settings.api_key.get_secret_value()),
         }
         params = {
+            'messages': self.message_converter.convert_messages(messages),
             'model': self.model,
-            'messages': openai_messages,
+            'stream': stream,
             **parameters.custom_model_dump(),
         }
-        if stream:
-            params['stream'] = True
-
         return {
-            'url': f'{self.settings.api_base}/chat/completions',
+            'url': self.settings.api_base + '/chat/completions',
             'headers': headers,
             'json': params,
         }
 
-    def _convert_to_openai_messages(self, messages: Messages) -> List[OpenAIMessage]:
-        return [convert_to_openai_message(message) for message in messages]
-
-    @staticmethod
-    def generate_tool_call_id() -> str:
-        return f'call_{uuid.uuid4()}'
-
     @override
-    def _process_reponse(self, response: Dict[str, Any]) -> ChatCompletionOutput:
-        return process_openai_like_model_reponse(response, model_type=self.model_type)
+    def _process_reponse(self, response: ResponseValue) -> ChatCompletionOutput:
+        return ChatCompletionOutput(
+            model_info=self.model_info,
+            message=self._parse_assistant_message(response['choices'][0]['message']),
+            usage=self._parse_usage(response),
+            extra=self._parse_extra(response),
+            finish_reason=self._parse_finish_reason(response),
+        )
 
     @override
-    def _process_stream_line(self, line: str, stream_manager: StreamManager) -> ChatCompletionStreamOutput | None:
+    def _process_stream_response(
+        self, response: Dict[str, Any], stream_manager: StreamManager
+    ) -> ChatCompletionStreamOutput | None:
+        delta_dict = response['choices'][0]['delta']
+        self._update_delta(delta_dict, stream_manager)
+        stream_manager.finish_reason = self._parse_finish_reason(response)
+        stream_manager.extra = self._parse_extra(response)
+        stream_manager.usage = self._parse_usage(response)
+        return stream_manager.build_stream_output()
+
+    def add_tools(self, tools: OrIterable[Tool]) -> None:
+        new_tools: list[ZhipuTool] = [
+            {
+                'type': 'function',
+                'function': {
+                    'name': tool.name,
+                    'description': tool.description,
+                    'parameters': tool.parameters,
+                },
+            }
+            for tool in ensure_iterable(tools)
+        ]
+        if self.parameters.tools is None:
+            self.parameters.tools = new_tools
+        else:
+            self.parameters.tools.extend(new_tools)
+
+    def _parse_assistant_message(self, message: dict[str, Any]) -> AssistantMessage:
+        if 'tool_calls' in message:
+            dict_format_tool_calls = message['tool_calls']
+            dict_format_tool_calls.sort(key=lambda x: x['index'])
+            tool_calls = []
+            for tool_call_dict in message['tool_calls']:
+                if tool_call_dict['type'] != 'function':
+                    raise ValueError(f'invalid tool type: {tool_call_dict["type"]}, should be function')
+                tool_calls.append(
+                    ToolCall(
+                        id=tool_call_dict['id'],
+                        type='function',
+                        function=FunctionCall(
+                            name=tool_call_dict['function']['name'],
+                            arguments=tool_call_dict['function']['arguments'],
+                        ),
+                    )
+                )
+            return AssistantMessage(
+                role='assistant',
+                content=message.get('content') or '',
+                tool_calls=tool_calls,
+            )
+        return AssistantMessage(
+            role='assistant',
+            content=message['content'],
+        )
+
+    def _parse_usage(self, response: dict[str, Any]) -> Usage:
+        usage = response.get('usage')
+        if usage is not None:
+            input_tokens = usage['prompt_tokens']
+            output_tokens = usage['completion_tokens']
+            return Usage(input_tokens=input_tokens, output_tokens=output_tokens)
+        return Usage()
+
+    def _parse_finish_reason(self, response: dict[str, Any]) -> FinishReason | None:
         try:
-            data = json.loads(line)
-        except json.JSONDecodeError:
+            choice = response['choices'][0]
+            if finish_reason := choice.get('finish_reason'):
+                return FinishReason(finish_reason)
+        except (KeyError, IndexError, ValueError):
             return None
 
-        delta_dict = data['choices'][0].get('delta', {})
-        self._update_delta(delta_dict, stream_manager=stream_manager)
-        stream_manager.extra = self._extract_extra_info(data)
-        stream_manager.cost = self._calculate_cost(data)
-        stream_manager.finish_reason = self._determine_finish_reason(data)
-        return stream_manager.build_stream_output()
+    def _parse_extra(self, response: dict[str, Any]) -> dict[str, Any]:
+        return {'response': response}
 
     def _update_delta(self, delta_dict: dict[str, Any], stream_manager: StreamManager) -> None:
         delta_content: str = delta_dict.get('content') or ''
         stream_manager.delta = delta_content
 
         if delta_dict.get('tool_calls'):
             index = delta_dict['tool_calls'][0]['index']
             if index >= len(stream_manager.tool_calls or []):
-                new_tool_calls_message = _convert_to_assistant_message(delta_dict).tool_calls
+                new_tool_calls_message = self._parse_assistant_message(delta_dict).tool_calls
                 assert new_tool_calls_message is not None
                 if stream_manager.tool_calls is None:
                     stream_manager.tool_calls = []
                 stream_manager.tool_calls.append(new_tool_calls_message[0])
             else:
                 assert stream_manager.tool_calls is not None
                 stream_manager.tool_calls[index].function.arguments += delta_dict['tool_calls'][0]['function']['arguments']
-
-        if delta_dict.get('function_call'):
-            if stream_manager.function_call is None:
-                stream_manager.function_call = FunctionCall(name='', arguments='')
-            function_name = delta_dict['function_call'].get('name', '')
-            stream_manager.function_call.name += function_name
-            arguments = delta_dict['function_call'].get('arguments', '')
-            stream_manager.function_call.arguments += arguments
-
-    def _extract_extra_info(self, response: ResponseValue) -> dict[str, Any]:
-        extra = {
-            'id': response['id'],
-        }
-        choice = response['choices'][0]
-        if usage := response.get('usage'):
-            extra['usage'] = usage
-        if usage := choice.get('usage'):
-            extra['usage'] = usage
-        if system_fingerprint := response.get('system_fingerprint'):
-            extra['system_fingerprint'] = system_fingerprint
-        return extra
-
-    def _calculate_cost(self, response: ResponseValue) -> float | None:
-        if response.get('usage') is None:
-            return None
-
-        if self.model_type == 'openai':
-            return openai_calculate_cost(
-                model_name=response['model'],
-                input_tokens=response['usage']['prompt_tokens'],
-                output_tokens=response['usage']['completion_tokens'],
-            )
-
-        cost_calculator = GeneralCostCalculator()
-        input_tokens = response['usage'].get('prompt_tokens', 0)
-        output_tokens = response['usage'].get('completion_tokens', 0)
-        if 'total_tokens' in response['usage']:
-            input_tokens = 0
-            output_tokens = response['usage']['total_tokens']
-        return cost_calculator.calculate(
-            model_type=self.model_type,
-            model_name=response['model'],
-            input_tokens=input_tokens,
-            output_tokens=output_tokens,
-        )
-
-    def _determine_finish_reason(self, response: ResponseValue) -> str | None:
-        choice = response['choices'][0]
-        finish_reason = choice.get('finish_reason') or None
-        if finish_reason is None:
-            finish_reason: str | None = finish_details['type'] if (finish_details := choice.get('finish_details')) else None
-        return finish_reason
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/stepfun.py` & `generate_core-0.5.0b0/generate/chat_completion/models/stepfun.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 
 from typing import AsyncIterator, ClassVar, Iterator, List, Optional
 
 from pydantic import Field, PositiveInt
 from typing_extensions import Annotated, Unpack, override
 
 from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.converter import MessageConverter
 from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
 from generate.chat_completion.models.openai_like import OpenAILikeChat
 from generate.http import HttpClient
 from generate.model import ModelParameters, RemoteModelParametersDict
 from generate.platforms import StepFunSettings
 from generate.types import Probability
 
-Temperature = Annotated[float, Field(ge=0, le=2)]
-
 
 class StepFunChatParameters(ModelParameters):
-    temperature: Optional[Temperature] = None
+    temperature: Optional[Annotated[float, Field(ge=0, le=2)]] = None
     top_p: Optional[Probability] = None
     max_tokens: Optional[PositiveInt] = None
     presence_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
     frequency_penalty: Optional[Annotated[float, Field(ge=-2, le=2)]] = None
 
 
 class StepFunParametersDict(RemoteModelParametersDict, total=False):
-    temperature: Optional[Temperature]
-    top_p: Optional[Probability]
-    max_tokens: Optional[PositiveInt]
+    temperature: Optional[float]
+    top_p: Optional[float]
+    max_tokens: Optional[int]
     presence_penalty: Optional[float]
     frequency_penalty: Optional[float]
 
 
 class StepFunChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'stepfun'
     available_models: ClassVar[List[str]] = ['step-1-32k', 'step-1v-32k', 'step-1-200k']
@@ -41,20 +40,26 @@
 
     def __init__(
         self,
         model: str = 'step-1-32k',
         parameters: StepFunChatParameters | None = None,
         settings: StepFunSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: MessageConverter | None = None,
     ) -> None:
         parameters = parameters or StepFunChatParameters()
         settings = settings or StepFunSettings()  # type: ignore
         http_client = http_client or HttpClient()
-        model = model
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            message_converter=message_converter,
+            http_client=http_client,
+        )
 
     @override
     def generate(self, prompt: Prompt, **kwargs: Unpack[StepFunParametersDict]) -> ChatCompletionOutput:
         return super().generate(prompt, **kwargs)
 
     @override
     async def async_generate(self, prompt: Prompt, **kwargs: Unpack[StepFunParametersDict]) -> ChatCompletionOutput:
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/test.py` & `generate_core-0.5.0b0/generate/chat_completion/models/test.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/chat_completion/models/wenxin.py` & `generate_core-0.5.0b0/generate/modifiers/structure.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,260 +1,234 @@
 from __future__ import annotations
 
 import json
-from typing import Any, AsyncIterator, ClassVar, Dict, Iterator, List, Literal, Optional
+import re
+from copy import deepcopy
+from typing import Any, ClassVar, Dict, Generic, Iterable, List, Optional, Type, TypeVar
 
-from pydantic import Field, model_validator
-from typing_extensions import Annotated, NotRequired, Self, TypedDict, Unpack, override
+from pydantic import BaseModel, TypeAdapter
+from typing_extensions import Self, TypedDict, Unpack
 
-from generate.chat_completion.base import RemoteChatCompletionModel
+from generate.chat_completion import ChatCompletionModel
 from generate.chat_completion.message import (
     AssistantMessage,
-    FunctionCall,
-    FunctionMessage,
-    Message,
-    Messages,
-    MessageTypeError,
     Prompt,
     SystemMessage,
+    UnionMessage,
     UserMessage,
     ensure_messages,
 )
-from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
-from generate.chat_completion.stream_manager import StreamManager
-from generate.chat_completion.tool import Tool, ToolCallMixin
-from generate.http import (
-    HttpClient,
-    HttpxPostKwargs,
-    ResponseValue,
-    UnexpectedResponseError,
-)
-from generate.model import ModelParameters, RemoteModelParametersDict
-from generate.platforms.baidu import QianfanSettings, QianfanTokenManager
-from generate.types import JsonSchema, OrIterable, Probability, Temperature
-from generate.utils import ensure_iterable
-
-
-class WenxinMessage(TypedDict):
-    role: Literal['user', 'assistant', 'function']
-    content: str
-    name: NotRequired[str]
-    function_call: NotRequired[WenxinFunctionCall]
-
-
-class WenxinFunctionCall(TypedDict):
-    name: str
-    arguments: str
-    thoughts: NotRequired[str]
-
-
-class WenxinFunction(TypedDict):
-    name: str
-    description: str
-    parameters: JsonSchema
-    responses: NotRequired[JsonSchema]
-    examples: NotRequired[List[WenxinMessage]]
-
-
-def convert_to_wenxin_function(tool: Tool) -> WenxinFunction:
-    return {
-        'name': tool.name,
-        'description': tool.description,
-        'parameters': tool.parameters,
-    }
-
-
-def convert_to_wenxin_message(message: Message) -> WenxinMessage:
-    if isinstance(message, UserMessage):
-        return {
-            'role': 'user',
-            'content': message.content,
-        }
-
-    if isinstance(message, AssistantMessage):
-        if message.function_call:
-            return {
-                'role': 'assistant',
-                'function_call': {
-                    'name': message.function_call.name,
-                    'arguments': message.function_call.arguments,
-                    'thoughts': message.function_call.thoughts or '',
-                },
-                'content': message.content,
-            }
-        return {
-            'role': 'assistant',
-            'content': message.content,
-        }
-
-    if isinstance(message, FunctionMessage):
-        return {
-            'role': 'function',
-            'name': message.name,
-            'content': message.content,
-        }
-
-    raise MessageTypeError(message, allowed_message_type=(UserMessage, AssistantMessage, FunctionMessage))
-
-
-def _convert_messages(messages: Messages) -> list[WenxinMessage]:
-    if isinstance(system_message := messages[0], SystemMessage):
-        prepend_messages = [UserMessage(content=system_message.content), AssistantMessage(content='好的')]
-        messages = prepend_messages + messages[1:]
-    return [convert_to_wenxin_message(message) for message in messages]
-
-
-class WenxinChatParameters(ModelParameters):
-    temperature: Optional[Temperature] = None
-    top_p: Optional[Probability] = None
-    functions: Optional[List[WenxinFunction]] = None
-    penalty_score: Optional[Annotated[float, Field(ge=1, le=2)]] = None
-    system: Optional[str] = None
-    user: Optional[str] = Field(default=None, serialization_alias='user_id')
-
-    @model_validator(mode='after')
-    def system_function_conflict(self) -> Self:
-        if self.system is not None and self.functions is not None:
-            raise ValueError('system and functions cannot be used together')
-        return self
-
-    def custom_model_dump(self) -> dict[str, Any]:
-        output = super().custom_model_dump()
-        if 'temperature' in output:
-            output['temperature'] = max(0.01, output['temperature'])
-        return output
-
-
-class WenxinChatParametersDict(RemoteModelParametersDict, total=False):
-    temperature: Optional[Temperature]
-    top_p: Optional[Probability]
-    functions: Optional[List[WenxinFunction]]
-    penalty_score: Optional[float]
-    system: Optional[str]
-    user: Optional[str]
-
-
-class WenxinChat(RemoteChatCompletionModel, ToolCallMixin):
-    model_type: ClassVar[str] = 'wenxin'
-    model_name_entrypoint_map: ClassVar[Dict[str, str]] = {
-        'ERNIE-Bot': 'completions',
-        'ERNIE-Bot-turbo': 'eb-instant',
-        'ERNIE-Bot-4': 'completions_pro',
-    }
-    available_models: ClassVar[List[str]] = ['ERNIE-Bot', 'ERNIE-Bot-turbo', 'ERNIE-Bot-4']
+from generate.model import GenerateModel, ModelOutput, RemoteModelParametersDict
+
+system_template = """\
+# Instruction
+{instruction}
+# JSON Schema
+{json_schema}
+"""
+
+
+I = TypeVar('I', BaseModel, str, Dict[str, Any])  # noqa: E741
+O = TypeVar('O')  # noqa: E741
+M = TypeVar('M', bound=ChatCompletionModel)
+
+
+class Example(BaseModel, Generic[O]):
+    prompt: Prompt
+    output: O
+
+
+def is_valid_json(json_str: str) -> bool:
+    try:
+        json.loads(json_str, strict=False)
+    except json.JSONDecodeError:
+        return False
+    return True
+
+
+def is_valid_python_code(code_str: str) -> bool:
+    try:
+        eval(code_str)
+    except SyntaxError:
+        return False
+    return True
+
+
+def extract_json(json_str: str) -> str | None:
+    # markdown code pattern
+    json_code_pattern = r'```json\n(.*?)```'
+    match = re.search(json_code_pattern, json_str, re.DOTALL)
+    if match and is_valid_json(match.group(1)):
+        return match.group(1)
+
+    code_pattern = r'```(.*?)```'
+    match = re.search(code_pattern, json_str, re.DOTALL)
+    if match and is_valid_json(match.group(1)):
+        return match.group(1)
+
+    inline_code_pattern = r'`(.*?)`'
+    match = re.search(inline_code_pattern, json_str, re.DOTALL)
+    if match and is_valid_json(match.group(1)):
+        return match.group(1)
+
+    return None
 
-    parameters: WenxinChatParameters
-    settings: QianfanSettings
+
+def extract_python_code(code_str: str) -> str | None:
+    # markdown code pattern
+    json_code_pattern = r'```python\n(.*?)```'
+    match = re.search(json_code_pattern, code_str, re.DOTALL)
+    if match and is_valid_python_code(match.group(1)):
+        return match.group(1)
+
+    code_pattern = r'```(.*?)```'
+    match = re.search(code_pattern, code_str, re.DOTALL)
+    if match and is_valid_python_code(match.group(1)):
+        return match.group(1)
+
+    inline_code_pattern = r'`(.*?)`'
+    match = re.search(inline_code_pattern, code_str, re.DOTALL)
+    if match and is_valid_python_code(match.group(1)):
+        return match.group(1)
+
+    return None
+
+
+def ensure_valid_json(json_str: str) -> str:
+    if is_valid_json(json_str):
+        return json_str
+    if is_valid_python_code(json_str):
+        return json.dumps(eval(json_str))
+    if (valid_json := extract_json(json_str)) is not None:
+        return valid_json
+    if (valid_code := extract_python_code(json_str)) is not None:
+        return json.dumps(eval(valid_code))
+    raise ValueError(f'Invalid JSON, output should be a valid JSON string. Got: {json_str}')
+
+
+class StructureModelOutput(ModelOutput, Generic[O]):
+    structure: O
+
+
+class StructureModelKwargs(TypedDict, Generic[O], total=False):
+    instruction: Optional[str]
+    examples: Optional[Iterable[Example[O]]]
+    system_template: str
+    max_num_reask: int
+    output_exclude_none: bool
+
+
+class StructureGenerateModel(GenerateModel[str, StructureModelOutput[O]], Generic[M, O]):
+    model_task: ClassVar[str] = 'text_to_structure'
 
     def __init__(
         self,
-        model: str = 'ERNIE-Bot',
-        parameters: WenxinChatParameters | None = None,
-        settings: QianfanSettings | None = None,
-        http_client: HttpClient | None = None,
+        model: M,
+        output_structure_type: Type[O] | TypeAdapter[O],
+        instruction: str | None = None,
+        examples: Optional[Iterable[Example[O]]] = None,
+        system_template: str = system_template,
+        output_exclude_none: bool = False,
+        max_num_reask: int = 2,
     ) -> None:
-        parameters = parameters or WenxinChatParameters()
-        settings = settings or QianfanSettings()  # type: ignore
-        http_client = http_client or HttpClient()
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
-        self.token_manager = QianfanTokenManager(self.settings, self.http_client)
-
-    @override
-    def generate(self, prompt: Prompt, **kwargs: Unpack[WenxinChatParametersDict]) -> ChatCompletionOutput:
-        return super().generate(prompt, **kwargs)
-
-    @override
-    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[WenxinChatParametersDict]) -> ChatCompletionOutput:
-        return await super().async_generate(prompt, **kwargs)
-
-    @override
-    def stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[WenxinChatParametersDict]
-    ) -> Iterator[ChatCompletionStreamOutput]:
-        yield from super().stream_generate(prompt, **kwargs)
-
-    @override
-    async def async_stream_generate(
-        self, prompt: Prompt, **kwargs: Unpack[WenxinChatParametersDict]
-    ) -> AsyncIterator[ChatCompletionStreamOutput]:
-        async for output in super().async_stream_generate(prompt, **kwargs):
-            yield output
-
-    def _get_request_parameters(
-        self, prompt: Prompt, stream: bool = False, **kwargs: Unpack[WenxinChatParametersDict]
-    ) -> HttpxPostKwargs:
-        messages = ensure_messages(prompt)
-        parameters = self.parameters.clone_with_changes(**kwargs)
-        wenxin_messages: list[WenxinMessage] = _convert_messages(messages)
-        parameters_dict = parameters.custom_model_dump()
-        if 'temperature' in parameters_dict:
-            parameters_dict['temperature'] = max(0.01, parameters_dict['temperature'])
-        json_data = {'messages': wenxin_messages, **parameters_dict}
-        if stream:
-            json_data['stream'] = True
-
-        return {
-            'url': self.settings.comlpetion_api_base + self.model_name_entrypoint_map[self.model],
-            'json': json_data,
-            'params': {'access_token': self.token_manager.token},
-            'headers': {'Content-Type': 'application/json'},
-        }
-
-    @override
-    def _process_reponse(self, response: ResponseValue) -> ChatCompletionOutput:
-        if response.get('error_msg'):
-            raise UnexpectedResponseError(response)
-        if response.get('function_call'):
-            function_call = FunctionCall(
-                name=response['function_call']['name'],
-                arguments=response['function_call']['arguments'],
-                thoughts=response['function_call']['thoughts'],
-            )
+        self.model = model
+
+        if isinstance(output_structure_type, TypeAdapter):
+            default_instruction = 'Extract Information'
         else:
-            function_call = None
-        message = AssistantMessage(content=response['result'], function_call=function_call)
-        return ChatCompletionOutput(
-            model_info=self.model_info,
-            message=message,
-            cost=self._calculate_cost(response['usage']),
-            extra={
-                'is_truncated': response['is_truncated'],
-                'need_clear_history': response['need_clear_history'],
-                'usage': response['usage'],
-            },
-            finish_reason=response['finish_reason'],
+            default_instruction = f'Extract {output_structure_type.__name__}'
+        default_instruction = 'According to the JSON Schema below, parse the input text.'
+        self.instruction = instruction or default_instruction
+
+        self.output_structure_type = output_structure_type
+        self.examples = examples or []
+        self.system_template = system_template
+        self.max_num_reask = max_num_reask
+        self.output_exclude_none = output_exclude_none
+
+        self.model_type = self.model.model_type  # type: ignore
+
+    @property
+    def is_typeadapter(self) -> bool:
+        return isinstance(self.output_structure_type, TypeAdapter)
+
+    @property
+    def name(self) -> str:
+        return self.model.name
+
+    @classmethod
+    def from_name(cls, name: str) -> Self:
+        raise ValueError('Structure model cannot be created from name')
+
+    @property
+    def messages(self) -> List[UnionMessage]:
+        messages = []
+        messages.append(self.system_message)
+        for example in self.examples:
+            messages.extend(ensure_messages(example.prompt))
+            messages.append(AssistantMessage(content=self.model_dump_json(example.output)))
+        return messages
+
+    @property
+    def system_message(self) -> SystemMessage:
+        system_content = self.system_template.format(
+            instruction=self.instruction,
+            json_schema=json.dumps(self.model_json_schema(), indent=2, ensure_ascii=False),
         )
+        return SystemMessage(content=system_content)
 
-    @override
-    def _process_stream_line(self, line: str, stream_manager: StreamManager) -> ChatCompletionStreamOutput | None:
-        try:
-            data = json.loads(line)
-        except json.JSONDecodeError:
-            return None
-
-        stream_manager.delta = data['result']
-        if data['is_end']:
-            stream_manager.cost = self._calculate_cost(data['usage'])
-            stream_manager.finish_reason = 'stop'
-            extra = {
-                'is_truncated': data['is_truncated'],
-                'need_clear_history': data['need_clear_history'],
-                'usage': data['usage'],
-            }
-            stream_manager.extra.update(extra)
-        return stream_manager.build_stream_output()
-
-    def _calculate_cost(self, usage: dict[str, Any]) -> float | None:
-        if self.name == 'ERNIE-Bot':
-            return 0.012 * (usage['total_tokens'] / 1000)
-        if self.name == 'ERNIE-Bot-turbo':
-            return 0.008 * (usage['total_tokens'] / 1000)
-        if self.name == 'ERNIE-Bot-4':
-            return 0.12 * (usage['total_tokens'] / 1000)
-        return None
-
-    def add_tools(self, tools: OrIterable[Tool]) -> None:
-        new_functions = [convert_to_wenxin_function(tool) for tool in ensure_iterable(tools)]
-        if self.parameters.functions is None:
-            self.parameters.functions = new_functions
-        else:
-            self.parameters.functions.extend(new_functions)
+    def model_dump_json(self, item: O) -> str:
+        if self.is_typeadapter:
+            assert isinstance(self.output_structure_type, TypeAdapter)
+            return self.output_structure_type.dump_json(item, exclude_none=self.output_exclude_none).decode('utf-8')
+        assert isinstance(item, BaseModel)
+        return item.model_dump_json(exclude_none=self.output_exclude_none)
+
+    def model_json_schema(self) -> dict[str, Any]:
+        if self.is_typeadapter:
+            assert isinstance(self.output_structure_type, TypeAdapter)
+            return self.output_structure_type.json_schema()
+        return self.output_structure_type.model_json_schema()  # type: ignore
+
+    def model_validate_json(self, json_string: str) -> O:
+        if self.is_typeadapter:
+            assert isinstance(self.output_structure_type, TypeAdapter)
+            return self.output_structure_type.validate_json(json_string)
+        return self.output_structure_type.model_validate_json(json_string)  # type: ignore
+
+    def generate(self, prompt: Prompt, **kwargs: Unpack[RemoteModelParametersDict]) -> StructureModelOutput[O]:
+        messages = deepcopy(self.messages)
+        messages.extend(ensure_messages(prompt))
+        num_reask = 0
+        while num_reask <= self.max_num_reask:
+            model_output = self.model.generate(messages, **kwargs)
+            messages.append(model_output.message)
+            try:
+                json_string = ensure_valid_json(model_output.reply)
+                structure = self.model_validate_json(json_string)
+                return StructureModelOutput(model_info=model_output.model_info, structure=structure, extra=model_output.extra)
+            except Exception as e:
+                num_reask += 1
+                messages.append(
+                    UserMessage(content=f'I got an error, please try to fix your output based on the error message. Error: {e}')
+                )
+
+        raise ValueError(f'Failed to generate valid JSON after {self.max_num_reask} reasks.')
+
+    async def async_generate(self, prompt: Prompt, **kwargs: Unpack[RemoteModelParametersDict]) -> StructureModelOutput[O]:
+        messages = deepcopy(self.messages)
+        messages.extend(ensure_messages(prompt))
+        num_reask = 0
+        while num_reask <= self.max_num_reask:
+            model_output = await self.model.async_generate(messages, **kwargs)
+            messages.append(model_output.message)
+            try:
+                json_string = ensure_valid_json(model_output.reply)
+                structure = self.model_validate_json(json_string)
+                return StructureModelOutput(model_info=model_output.model_info, structure=structure, extra=model_output.extra)
+            except Exception as e:
+                num_reask += 1
+                messages.append(
+                    UserMessage(content=f'I got an error, please try to fix your output based on the error message. Error: {e}')
+                )
+
+        raise ValueError(f'Failed to generate valid JSON after {self.max_num_reask} reasks.')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `generate_core-0.4.3/generate/chat_completion/models/yi.py` & `generate_core-0.5.0b0/generate/chat_completion/models/yi.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 
 from typing import AsyncIterator, ClassVar, Iterator, List, Optional
 
 from pydantic import Field, PositiveInt
 from typing_extensions import Annotated, Unpack, override
 
 from generate.chat_completion.message import Prompt
+from generate.chat_completion.message.converter import MessageConverter
 from generate.chat_completion.model_output import ChatCompletionOutput, ChatCompletionStreamOutput
 from generate.chat_completion.models.openai_like import OpenAILikeChat
 from generate.http import HttpClient
 from generate.model import ModelParameters, RemoteModelParametersDict
 from generate.platforms import YiSettings
 
 
 class YiChatParameters(ModelParameters):
     temperature: Optional[Annotated[float, Field(ge=0, lt=2)]] = None
     max_tokens: Optional[PositiveInt] = None
+    top_p: Optional[Annotated[float, Field(ge=0, lt=1)]] = None
 
 
 class YiParametersDict(RemoteModelParametersDict, total=False):
-    temperature: Optional[Annotated[float, Field(ge=0, lt=2)]]
-    max_tokens: Optional[PositiveInt]
+    temperature: Optional[float]
+    max_tokens: Optional[int]
+    top_p: Optional[float]
 
 
 class YiChat(OpenAILikeChat):
     model_type: ClassVar[str] = 'yi'
     available_models: ClassVar[List[str]] = ['yi-34b-chat-0205', 'yi-34b-chat-200k', 'yi-vl-plus']
 
     parameters: YiChatParameters
@@ -32,20 +35,25 @@
 
     def __init__(
         self,
         model: str = 'yi-34b-chat-0205',
         parameters: YiChatParameters | None = None,
         settings: YiSettings | None = None,
         http_client: HttpClient | None = None,
+        message_converter: MessageConverter | None = None,
     ) -> None:
         parameters = parameters or YiChatParameters()
         settings = settings or YiSettings()  # type: ignore
-        http_client = http_client or HttpClient()
-        model = model
-        super().__init__(model=model, parameters=parameters, settings=settings, http_client=http_client)
+        super().__init__(
+            model=model,
+            parameters=parameters,
+            settings=settings,
+            message_converter=message_converter,
+            http_client=http_client,
+        )
 
     @override
     def generate(self, prompt: Prompt, **kwargs: Unpack[YiParametersDict]) -> ChatCompletionOutput:
         return super().generate(prompt, **kwargs)
 
     @override
     async def async_generate(self, prompt: Prompt, **kwargs: Unpack[YiParametersDict]) -> ChatCompletionOutput:
```

### Comparing `generate_core-0.4.3/generate/chat_completion/printer.py` & `generate_core-0.5.0b0/generate/chat_completion/printer.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/chat_completion/stream_manager.py` & `generate_core-0.5.0b0/generate/chat_completion/stream_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Any, Dict, List, Literal, Optional
 
 from pydantic import BaseModel
 
 from generate.chat_completion.message.core import AssistantMessage, FunctionCall, ToolCall
-from generate.chat_completion.model_output import ChatCompletionStreamOutput, Stream
+from generate.chat_completion.model_output import ChatCompletionStreamOutput, FinishReason, Stream, Usage
 from generate.model import ModelInfo
 
 
 class StreamManager(BaseModel):
     info: ModelInfo
     delta: Optional[str] = None
-    cost: Optional[float] = None
+    usage: Usage = Usage()
     history_streams: List[Stream] = []
-    finish_reason: Optional[str] = None
+    finish_reason: Optional[FinishReason] = None
     function_call: Optional[FunctionCall] = None
-    tool_calls: Optional[List[ToolCall]] = None
+    tool_calls: List[ToolCall] = []
     close: bool = False
     extra: Dict[str, Any] = {}
 
     @property
     def already_start(self) -> bool:
         return bool(self.history_streams)
 
@@ -46,28 +46,25 @@
 
     def build_stream_output(self) -> Optional[ChatCompletionStreamOutput]:
         if self.close:
             return None
 
         stream = self.current_stream
         if stream:
-            if not self.history_streams:
-                assert self.control == 'start'
-
             self.history_streams.append(stream)
             self.delta = None
             output = ChatCompletionStreamOutput(
                 model_info=self.info,
-                cost=self.cost,
+                usage=self.usage,
                 extra=self.extra,
                 finish_reason=self.finish_reason,
                 message=AssistantMessage(
                     content=self.content,
                     function_call=self.function_call,
-                    tool_calls=self.tool_calls,
+                    tool_calls=self.tool_calls or None,
                 ),
                 stream=stream,
             )
 
             if output.is_finish:
                 self.close = True
             return output
```

### Comparing `generate_core-0.4.3/generate/chat_completion/tool.py` & `generate_core-0.5.0b0/generate/chat_completion/tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from __future__ import annotations
 
+import uuid
 from collections import UserDict
-from typing import Any, Callable, Generic, MutableMapping, TypeVar
+from typing import Any, Callable, Generic, MutableMapping, Protocol, TypeVar, runtime_checkable
 
 from docstring_parser import parse
 from pydantic import TypeAdapter, validate_call
 from typing_extensions import NotRequired, ParamSpec, Self, TypedDict
 
+from generate.chat_completion.message.core import (
+    AssistantMessage,
+    FunctionCall,
+    FunctionMessage,
+    Messages,
+    ToolCall,
+    ToolMessage,
+)
 from generate.types import JsonSchema, OrIterable
 from generate.utils import ensure_iterable
 
 P = ParamSpec('P')
 T = TypeVar('T')
 
 
@@ -93,10 +102,27 @@
         return self.data[name](*args, **kwargs)
 
     @classmethod
     def from_iterable(cls, tools: OrIterable[Tool]) -> Self:
         return cls({tool.name: tool for tool in ensure_iterable(tools)})
 
 
-class ToolCallMixin:
+@runtime_checkable
+class SupportToolCall(Protocol):
     def add_tools(self, tools: OrIterable[Tool]) -> None:
-        raise NotImplementedError
+        ...
+
+    def generate_tool_call_id(self, function_call: FunctionCall) -> str:
+        return f'tool_{uuid.uuid4().hex}'
+
+    def process_messages_for_tool_call(self, messages: Messages) -> None:
+        for index in range(len(messages)):
+            current_message = messages[index]
+            if isinstance(current_message, AssistantMessage) and current_message.function_call is not None:
+                tool_call_id = self.generate_tool_call_id(current_message.function_call)
+                messages[index].tool_calls = [ToolCall(id=tool_call_id, function=current_message.function_call)]
+                messages[index].function_call = None
+                next_message = messages[index + 1] if index + 1 < len(messages) else None
+                if next_message is not None and isinstance(next_message, FunctionMessage):
+                    messages[index + 1] = ToolMessage(
+                        tool_call_id=tool_call_id, name=next_message.name, content=next_message.content
+                    )
```

### Comparing `generate_core-0.4.3/generate/http.py` & `generate_core-0.5.0b0/generate/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     min_wait_seconds: int = 2
     max_wait_seconds: int = 20
     max_attempt: int = 3
 
 
 class HttpGetKwargs(TypedDict, total=False):
     url: Required[str]
-    params: QueryParams
-    headers: Headers
+    params: Optional[QueryParams]
+    headers: Optional[Headers]
     timeout: Optional[int]
 
 
 class HttpxPostKwargs(TypedDict, total=False):
     url: Required[str]
     json: Required[Any]
     headers: Required[Headers]
@@ -186,37 +186,44 @@
         wait = wait_random_exponential(min=self.retry.min_wait_seconds, max=self.retry.max_wait_seconds)
         stop = stop_after_attempt(self.retry.max_attempt)
         return retry(wait=wait, stop=stop)(self._async_stream_post)(request_parameters)
 
     def _post(self, request_parameters: HttpxPostKwargs) -> Response:
         logger.debug(f'POST {request_parameters}')
         http_response = self.client.post(**request_parameters)  # type: ignore
-        http_response.raise_for_status()
+        self.raise_for_status(http_response)
         logger.debug(f'Response {http_response}')
         return http_response
 
     async def _async_post(self, request_parameters: HttpxPostKwargs) -> Response:
         logger.debug(f'POST {request_parameters}')
         http_response = await self.async_client.post(**request_parameters)  # type: ignore
-        http_response.raise_for_status()
+        self.raise_for_status(http_response)
         logger.debug(f'Response {http_response}')
         return http_response
 
     def _get(self, request_parameters: HttpGetKwargs) -> Response:
         logger.debug(f'GET {request_parameters}')
         http_response = self.client.get(**request_parameters)
-        http_response.raise_for_status()
+        self.raise_for_status(http_response)
         return http_response
 
     async def _async_get(self, request_parameters: HttpGetKwargs) -> Response:
         logger.debug(f'GET {request_parameters}')
         http_response = await self.async_client.get(**request_parameters)
-        http_response.raise_for_status()
+        self.raise_for_status(http_response)
         return http_response
 
+    @staticmethod
+    def raise_for_status(response: Response) -> None:
+        try:
+            response.raise_for_status()
+        except httpx.HTTPStatusError as e:
+            raise UnexpectedResponseError(response.json()) from e
+
     def _stream_post(self, request_parameters: HttpxPostKwargs) -> Generator[str, None, None]:
         logger.debug(f'POST {request_parameters}')
         if self.stream_strategy == 'sse':
             return self._generate_data_from_sse_stream(request_parameters)
         return self._generate_data_from_basic_stream(request_parameters)
 
     def _generate_data_from_sse_stream(self, request_parameters: HttpxPostKwargs) -> Generator[str, None, None]:
```

### Comparing `generate_core-0.4.3/generate/model.py` & `generate_core-0.5.0b0/generate/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         return f'{self.type}/{self.name}'
 
 
 class ModelOutput(BaseModel):
     model_config = ConfigDict(protected_namespaces=())
 
     model_info: ModelInfo
-    cost: Optional[float] = None
     extra: Dict[str, Any] = {}
 
 
 I = TypeVar('I')  # noqa: E741
 O = TypeVar('O', bound=ModelOutput)  # noqa: E741
```

### Comparing `generate_core-0.4.3/generate/modifiers/agent.py` & `generate_core-0.5.0b0/generate/modifiers/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Messages,
     Prompt,
     ToolCall,
     ToolMessage,
 )
 from generate.chat_completion.message.utils import ensure_messages
 from generate.chat_completion.model_output import ChatCompletionOutput
-from generate.chat_completion.tool import Tool, ToolCallMixin, ToolDict
+from generate.chat_completion.tool import SupportToolCall, Tool, ToolDict
 from generate.types import OrIterable
 
 AgentMessage = Union[AssistantMessage, FunctionMessage, ToolMessage]
 
 
 class AgentKwargs(TypedDict, total=False):
     tools: ToolDict | OrIterable[Tool] | None
@@ -43,15 +43,15 @@
             self.tools = ToolDict()
         elif isinstance(tools, ToolDict):
             self.tools = tools
         else:
             self.tools = ToolDict.from_iterable(tools)
 
         if self.tools:
-            if isinstance(model, ToolCallMixin):
+            if isinstance(model, SupportToolCall):
                 model.add_tools(self.tools.values())
             else:
                 raise ValueError('Model does not support tools')
 
         self.tool_call_raise_error = tool_call_raise_error
         self.max_num_tool_calls_per_turn = max_num_tool_calls_per_turn
```

### Comparing `generate_core-0.4.3/generate/modifiers/hook.py` & `generate_core-0.5.0b0/generate/modifiers/hook.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/modifiers/limit.py` & `generate_core-0.5.0b0/generate/modifiers/limit.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/modifiers/session.py` & `generate_core-0.5.0b0/generate/modifiers/session.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/platforms/__init__.py` & `generate_core-0.5.0b0/generate/platforms/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from generate.platforms.anthropic import AnthropicSettings
 from generate.platforms.azure import AzureSettings
 from generate.platforms.baichuan import BaichuanSettings
 from generate.platforms.baidu import BaiduCreationSettings, QianfanSettings
-from generate.platforms.bailian import BailianSettings
 from generate.platforms.base import PlatformSettings
 from generate.platforms.dashscope import DashScopeSettings
 from generate.platforms.deepseek import DeepSeekSettings
-from generate.platforms.hunyuan import HunyuanSettings
 from generate.platforms.minimax import MinimaxSettings
 from generate.platforms.moonshot import MoonshotSettings
 from generate.platforms.openai import OpenAISettings
+from generate.platforms.openrouter import OpenRouterSettings
 from generate.platforms.stepfun import StepFunSettings
 from generate.platforms.yi import YiSettings
 from generate.platforms.zhipu import ZhipuSettings
 
 __all__ = [
     'AzureSettings',
     'AnthropicSettings',
     'BaichuanSettings',
     'BaiduCreationSettings',
     'MinimaxSettings',
     'ZhipuSettings',
     'OpenAISettings',
     'QianfanSettings',
-    'BailianSettings',
-    'HunyuanSettings',
     'DashScopeSettings',
     'MoonshotSettings',
     'DeepSeekSettings',
     'YiSettings',
     'PlatformSettings',
     'StepFunSettings',
+    'OpenRouterSettings',
 ]
```

### Comparing `generate_core-0.4.3/generate/platforms/baidu.py` & `generate_core-0.5.0b0/generate/platforms/baidu.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/platforms/base.py` & `generate_core-0.5.0b0/generate/platforms/base.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/platforms/zhipu.py` & `generate_core-0.5.0b0/generate/platforms/zhipu.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 CACHE_TTL_SECONDS = API_TOKEN_TTL_SECONDS - 30
 
 
 class ZhipuSettings(PlatformSettings):
     model_config = SettingsConfigDict(extra='ignore', env_prefix='zhipu_', env_file='.env')
 
     api_key: SecretStr
-    v3_api_base: str = 'https://open.bigmodel.cn/api/paas/v3/model-api'
-    v4_api_base: str = 'https://open.bigmodel.cn/api/paas/v4'
+    api_base: str = 'https://open.bigmodel.cn/api/paas/v4'
     platform_url: str = 'https://open.bigmodel.cn/dev/howuse/introduction'
 
 
 @cachetools.func.ttl_cache(ttl=CACHE_TTL_SECONDS)
 def generate_zhipu_token(api_key: str) -> str:
     try:
         api_key, secret = api_key.split('.')
```

### Comparing `generate_core-0.4.3/generate/test.py` & `generate_core-0.5.0b0/generate/test.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/generate/ui.py` & `generate_core-0.5.0b0/generate/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, List, Optional, Type, cast
 
 from pydantic import BaseModel
 
 from generate.chat_completion.base import RemoteChatCompletionModel
-from generate.chat_completion.models.dashscope_multimodal import DashScopeMultiModalChat
 from generate.model import ModelInfo
 
 try:
     import chainlit as cl
     import typer
     from chainlit.element import Avatar
     from chainlit.input_widget import Select, Slider, TextInput
@@ -129,23 +128,18 @@
         for element in message.elements:
             mime = element.mime or ''
             if mime.startswith('image'):
                 image_format = mime.split('/')[1]
                 if element.path is not None:
                     with open(element.path, 'rb') as image_file:
                         image_content = image_file.read()
-                    if isinstance(state.chat_model, DashScopeMultiModalChat):
-                        url = state.chat_model.upload_image(image_content, image_format)
-                        image_url = ImageUrl(url=url)
-                        image_part = ImageUrlPart(image_url=image_url)
-                    else:
-                        image_part = ImagePart(
-                            image=image_content,
-                            image_format=image_format,
-                        )
+                    image_part = ImagePart(
+                        image=image_content,
+                        image_format=image_format,
+                    )
                     image_parts.append(image_part)
                 elif element.url is not None:
                     image_url = ImageUrl(url=element.url)
                     image_url_part = ImageUrlPart(image_url=image_url)
                     image_parts.append(image_url_part)
 
         if image_parts:
```

### Comparing `generate_core-0.4.3/generate/utils.py` & `generate_core-0.5.0b0/generate/utils.py`

 * *Files identical despite different names*

### Comparing `generate_core-0.4.3/pyproject.toml` & `generate_core-0.5.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generate-core"
-version = "0.4.3"
+version = "0.5.0-beta"
 description = "文本生成，图像生成，语音生成"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "generate" }]
 repository = "https://github.com/wangyuxinwhy/generate"
 keywords = ["openai", "text generation", "image generation", "text to speech"]
@@ -18,33 +18,33 @@
 pyjwt = "^2.8.0"
 cachetools = "^5.3.1"
 tqdm = "^4.66.1"
 pydantic = "^2.0"
 docstring-parser = "^0.15"
 httpx-sse = "^0.4.0"
 pydantic-settings = "^2.1.0"
+diskcache = "^5.6.3"
 
 [tool.ruff]
 line-length = 128
 lint.select = [
-    "E",    # pycodestyle errors
-    "W",    # pycodestyle warnings
-    "F",    # pyflakes
-    "I",    # isort
-    "C",    # flake8-comprehensions
-    "B",    # flake8-bugbear
+    "E",   # pycodestyle errors
+    "W",   # pycodestyle warnings
+    "F",   # pyflakes
+    "I",   # isort
+    "C",   # flake8-comprehensions
+    "B",   # flake8-bugbear
     "N",
     "SIM",
     "ANN",
     "A",
     "T",
     "PT",
     "RET",
     "TRY",
-    "PERF",
 ]
 lint.ignore = [
     "E501",    # line too long, handled by black
     "B008",    # do not perform function calls in argument defaults
     "B905",    # zip strict
     "C901",    # too complex
     "A003",    # shadow builtin
```

### Comparing `generate_core-0.4.3/PKG-INFO` & `generate_core-0.5.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-core
-Version: 0.4.3
+Version: 0.5.0b0
 Summary: 文本生成，图像生成，语音生成
 Home-page: https://github.com/wangyuxinwhy/generate
 License: MIT
 Keywords: openai,text generation,image generation,text to speech
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncer (==0.0.2)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
+Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
@@ -50,44 +51,46 @@
 [![Documentation](https://img.shields.io/badge/docs-latest-brightgreen.svg)](https://wangyuxinwhy.github.io/generate/)
 [![Made with Love](https://img.shields.io/badge/made%20with-love-red.svg)](#)
 
 </div>
 <br>
 <br>
 
-# 简介
-
+> [!IMPORTANT]  
+> generate v0.5.0 版本的设计思路发生较大变化。由于个人精力有限，generate 不再追求支持更多的平台，而是更多的围绕模型的辅助功能进行开发。另外，国内大部分平台已经提供了适配 OpenAI SDK 的 API，如果你只需要基础的文本生成功能，建议直接使用 OpenAI SDK。
 
+# 简介
 
 Generate 允许用户通过统一的 api 访问多平台的生成式模型，当前支持：
 
-| 平台 🤖           | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
-| ----------------- | ------- | ------- | ------- | --------- | -------- |
-| OpenAI            | ✅      | ✅      | ✅      | ✅        | ✅       |
-| Azure             | ✅      | ✅      | ❌      | ✅        | ✅       |
-| Anthropic         | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 文心 Wenxin       | ✅      | ✅      | ✅      | ❌        | ✅       |
-| 百炼 Bailian      | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 灵积 DashScope    | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 百川智能 Baichuan | ✅      | ✅      | ✅      | ❌        | ❌       |
-| Minimax           | ✅      | ✅      | ✅      | ❌        | ✅       |
-| 混元 Hunyuan      | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 智谱 Zhipu        | ✅      | ✅      | ✅      | ✅        | ✅       |
-| 月之暗面 Moonshot | ✅      | ✅      | ✅      | ❌        | ❌       |
-| DeepSeek          | ✅      | ✅      | ✅      | ❌        | ❌       |
-| 零一万物 Yi       | ✅      | ✅      | ✅      | ✅        | ❌       |
-| 阶跃星辰 StepFun  | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 平台 🤖             | 同步 🔄 | 异步 ⏳ | 流式 🌊 | Vision 👀 | Tools 🛠️ |
+| ------------------- | ------- | ------- | ------- | --------- | -------- |
+| OpenAI              | ✅      | ✅      | ✅      | ✅        | ✅       |
+| Azure               | ✅      | ✅      | ❌      | ✅        | ✅       |
+| Anthropic           | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 文心 Wenxin         | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 灵积/百炼 DashScope | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 百川智能 Baichuan   | ✅      | ✅      | ✅      | ❌        | ✅       |
+| Minimax             | ✅      | ✅      | ✅      | ❌        | ✅       |
+| 混元 Hunyuan        | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 智谱 Zhipu          | ✅      | ✅      | ✅      | ✅        | ✅       |
+| 月之暗面 Moonshot   | ✅      | ✅      | ✅      | ❌        | ✅       |
+| DeepSeek            | ✅      | ✅      | ✅      | ❌        | ❌       |
+| 零一万物 Yi         | ✅      | ✅      | ✅      | ✅        | ❌       |
+| 阶跃星辰 StepFun    | ✅      | ✅      | ✅      | ✅        | ❌       |
+
+> v0.5.0-beta 版本中，混元，文心尚未适配
 
 ## Features
 
 - **多模态**，支持文本生成，多模态文本生成，结构体生成，图像生成，语音生成...
 - **跨平台**，支持 OpenAI，Azure，Minimax，智谱，月之暗面，文心一言 在内的国内外 10+ 平台
 - **One API**，统一了不同平台的消息格式，推理参数，接口封装，返回解析，让用户无需关心不同平台的差异
 - **异步，流式和并发**，提供流式调用，非流式调用，同步调用，异步调用，异步批量并发调用，适配不同的应用场景
-- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，_Agent_, _Tool call_ 等
+- **自带电池**，提供 chainlit UI，输入检查，参数检查，计费，速率控制，Disk Cache，_Agent_, _Tool call_ 等
 - **轻量**，最小化依赖，不同平台的请求和鉴权逻辑均为原生内置功能
 - **高质量代码**，100% typehints，pylance strict, ruff lint & format, test coverage > 85% ...
 
 ## 基础使用
 
 <a target="_blank" href="https://colab.research.google.com/github/wangyuxinwhy/generate/blob/main/examples/tutorial.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
```

