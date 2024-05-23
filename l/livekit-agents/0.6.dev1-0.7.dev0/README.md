# Comparing `tmp/livekit_agents-0.6.dev1.tar.gz` & `tmp/livekit_agents-0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_agents-0.6.dev1.tar", last modified: Wed May  1 00:52:12 2024, max compression
+gzip compressed data, was "livekit_agents-0.7.dev0.tar", last modified: Thu May 23 15:56:19 2024, max compression
```

## Comparing `livekit_agents-0.6.dev1.tar` & `livekit_agents-0.7.dev0.tar`

### file list

```diff
@@ -1,76 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.590407 livekit_agents-0.6.dev1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.594407 livekit_agents-0.6.dev1/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.598407 livekit_agents-0.6.dev1/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tokenize/sentence_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/tts/tts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/exp_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/utils/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30755 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/voice_assistant/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    16319 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 00:52:12.000000 livekit_agents-0.6.dev1/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:52:12.602407 livekit_agents-0.6.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-01 00:52:08.000000 livekit_agents-0.6.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.781198 livekit_agents-0.7.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36820 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_hyphenator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_sent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/token_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/transcription/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/stt_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/tts_forwarder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/exp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32625 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/setup.py
```

### Comparing `livekit_agents-0.6.dev1/PKG-INFO` & `livekit_agents-0.7.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.6.dev1
+Version: 0.7.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import aio, codecs, ipc, llm, stt, tokenize, tts, utils, vad, voice_assistant
+from . import (
+    aio,
+    codecs,
+    ipc,
+    llm,
+    stt,
+    tokenize,
+    transcription,
+    tts,
+    utils,
+    vad,
+    voice_assistant,
+)
 from .apipe import AsyncPipe  # noqa
 from .ipc.protocol import IPC_MESSAGES, Log, StartJobRequest, StartJobResponse  # noqa
 from .job_context import JobContext
 from .job_request import AutoDisconnect, AutoSubscribe, JobRequest
 from .plugin import Plugin
 from .version import __version__
 from .worker import Worker, WorkerOptions
@@ -36,8 +48,9 @@
     "vad",
     "utils",
     "tts",
     "aio",
     "tokenize",
     "llm",
     "voice_assistant",
+    "transcription",
 ]
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/channel.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/channel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 from collections import deque
 from typing import Generic, Protocol, Tuple, TypeVar
 
 T = TypeVar("T")
 T_co = TypeVar("T_co", covariant=True)
@@ -144,17 +146,17 @@
 
         while self._gets:
             self._wakeup_next(self._gets)
 
     #        if self.empty():
     #            self._finished_ev.set()
 
-    @property
-    def closed(self) -> bool:
-        return self._closed
+    # @property
+    # def closed(self) -> bool:
+    #    return self._closed
 
     #    async def join(self) -> None:
     #        await self._finished_ev.wait()
 
     def qsize(self) -> int:
         return len(self._queue)
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/debug.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/interval.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/select.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/select.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/sleep.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/sleep.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 
 
 def _finish_fut(fut: asyncio.Future):
     if fut.cancelled():
         return
     fut.set_result(None)
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/aio/wait_group.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/apipe.py` & `livekit_agents-0.7.dev0/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/cli/cli.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,116 @@
 import asyncio
 import functools
 import pathlib
 import signal
 import sys
 
 import click
+from livekit.protocol import models
 
 from .. import aio
 from ..log import logger
 from ..plugin import Plugin
 from ..worker import Worker, WorkerOptions
 from . import protocol
 from .log import setup_logging
 
 
-def run_app(opts: WorkerOptions) -> None:
-    """Run the CLI to interact with the worker"""
+def shared_args(func):
+    @click.option(
+        "--log-level",
+        default="INFO",
+        type=click.Choice(
+            ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
+        ),
+        help="Set the logging level",
+    )
+    @click.option(
+        "--url",
+        envvar="LIVEKIT_URL",
+        help="LiveKit server or Cloud project's websocket URL",
+    )
+    @click.option(
+        "--api-key",
+        envvar="LIVEKIT_API_KEY",
+        help="LiveKit server or Cloud project's API key",
+    )
+    @click.option(
+        "--api-secret",
+        envvar="LIVEKIT_API_SECRET",
+        help="LiveKit server or Cloud project's API secret",
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
 
-    def shared_args(func):
-        @click.option(
-            "--log-level",
-            default="INFO",
-            type=click.Choice(
-                ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
-            ),
-            help="Set the logging level",
-        )
-        @click.option(
-            "--url",
-            envvar="LIVEKIT_URL",
-            help="LiveKit server or Cloud project's websocket URL",
-        )
-        @click.option(
-            "--api-key",
-            envvar="LIVEKIT_API_KEY",
-            help="LiveKit server or Cloud project's API key",
-        )
-        @click.option(
-            "--api-secret",
-            envvar="LIVEKIT_API_SECRET",
-            help="LiveKit server or Cloud project's API secret",
-        )
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            return func(*args, **kwargs)
+    return wrapper
 
-        return wrapper
+
+def shared_dev_args(func):
+    @click.option(
+        "--asyncio-debug/--no-asyncio-debug",
+        default=False,
+        help="Enable debugging feature of asyncio",
+    )
+    @click.option(
+        "--watch/--no-watch",
+        default=True,
+        help="Watch for changes in the current directory and plugins in editable mode",
+    )
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def _run_dev(
+    opts: WorkerOptions,
+    log_level: str,
+    url: str,
+    api_key: str,
+    api_secret: str,
+    asyncio_debug: bool,
+    watch: bool,
+    room: str = "",
+    participant_identity: str = "",
+):
+    opts.ws_url = url or opts.ws_url
+    opts.api_key = api_key or opts.api_key
+    opts.api_secret = api_secret or opts.api_secret
+    args = protocol.CliArgs(
+        opts=opts,
+        log_level=log_level,
+        production=False,
+        asyncio_debug=asyncio_debug,
+        watch=watch,
+        drain_timeout=0,
+        room=room,
+        participant_identity=participant_identity,
+    )
+
+    if watch:
+        from .watcher import WatchServer
+
+        setup_logging(log_level, args.production)
+
+        main_file = pathlib.Path(sys.argv[0]).parent
+        server = WatchServer(run_worker, main_file, args, watch_plugins=True)
+        server.run()
+    else:
+        run_worker(args)
+
+
+def run_app(opts: WorkerOptions) -> None:
+    """Run the CLI to interact with the worker"""
 
     cli = click.Group()
 
-    @cli.command(
-        help="Start the worker in production mode. Use a json logger by default."
-    )
+    @cli.command(help="Start the worker in production mode.")
     @shared_args
     @click.option(
         "--drain-timeout",
         default=60,
         help="Time in seconds to wait for jobs to finish before shutting down",
     )
     def start(
@@ -72,78 +127,94 @@
             watch=False,
             drain_timeout=drain_timeout,
         )
         run_worker(args)
 
     @cli.command(help="Start the worker in development mode")
     @shared_args
+    @shared_dev_args
+    def dev(
+        log_level: str,
+        url: str,
+        api_key: str,
+        api_secret: str,
+        asyncio_debug: bool,
+        watch: bool,
+    ) -> None:
+        _run_dev(opts, log_level, url, api_key, api_secret, asyncio_debug, watch)
+
+    @cli.command(help="Connect to a specific room")
+    @shared_args
+    @shared_dev_args
+    @click.option("--room", help="Room name to connect to", required=True)
     @click.option(
-        "--asyncio-debug/--no-asyncio-debug",
-        default=False,
-        help="Enable debugging feature of asyncio",
-    )
-    @click.option(
-        "--watch/--no-watch",
-        default=True,
-        help="Watch for changes in the current directory and plugins in editable mode",
+        "--participant-identity", help="Participant identity (JobType.JT_PUBLISHER)"
     )
-    def dev(
+    def connect(
         log_level: str,
         url: str,
         api_key: str,
         api_secret: str,
         asyncio_debug: bool,
         watch: bool,
+        room: str,
+        participant_identity: str,
     ) -> None:
-        opts.ws_url = url or opts.ws_url
-        opts.api_key = api_key or opts.api_key
-        opts.api_secret = api_secret or opts.api_secret
-        args = protocol.CliArgs(
-            opts=opts,
-            log_level=log_level,
-            production=False,
-            asyncio_debug=asyncio_debug,
-            watch=watch,
-            drain_timeout=0,
+        _run_dev(
+            opts,
+            log_level,
+            url,
+            api_key,
+            api_secret,
+            asyncio_debug,
+            watch,
+            room,
+            participant_identity,
         )
 
-        if watch:
-            from .watcher import WatchServer
-
-            setup_logging(log_level, args.production)
-
-            main_file = pathlib.Path(sys.argv[0]).parent
-            server = WatchServer(run_worker, main_file, args, watch_plugins=True)
-            server.run()
-        else:
-            run_worker(args)
+    @cli.command(help="Download plugin dependency files (i.e. model weights, ...)")
+    @click.option(
+        "--log-level",
+        default="INFO",
+        type=click.Choice(
+            ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
+        ),
+        help="Set the logging level",
+    )
+    def download_files(log_level: str) -> None:
+        setup_logging(log_level, True)
 
-    @cli.command(help="Download plugin dependency files (i.e. model weights)")
-    def download_files() -> None:
         for plugin in Plugin.registered_plugins:
             logger.info(f"Downloading files for {plugin}")
             plugin.download_files()
-            logger.info(f"Finished Downloading files for {plugin}")
+            logger.info(f"Finished downloading files for {plugin}")
 
     cli()
 
 
 def run_worker(args: protocol.CliArgs) -> None:
     class Shutdown(SystemExit):
         pass
 
     setup_logging(args.log_level, args.production)
 
     loop = asyncio.get_event_loop()
     worker = Worker(args.opts, loop=loop)
 
     loop.set_debug(args.asyncio_debug)
-    loop.slow_callback_duration = 0.02  # 20ms
+    loop.slow_callback_duration = 0.03  # 30ms
     aio.debug.hook_slow_callbacks(0.75)
 
+    if args.room:
+        # directly connect to a specific roomj
+        @worker.once("worker_registered")
+        def _connect_on_register(worker_id: str, server_info: models.ServerInfo):
+            logger.info("connecting to room %s", args.room)
+            loop.create_task(worker.simulate_job(args.room, args.participant_identity))
+
     try:
 
         def _signal_handler():
             raise Shutdown
 
         for sig in (signal.SIGINT, signal.SIGTERM):
             loop.add_signal_handler(sig, _signal_handler)
@@ -162,15 +233,15 @@
         from .watcher import WatchClient
 
         assert args.cch is not None
 
         watch_client = WatchClient(worker, args.cch, loop=loop)
         watch_client.start()
 
-    main_task = loop.create_task(_worker_run(worker))
+    main_task = loop.create_task(_worker_run(worker), name="agent_runner")
     try:
         loop.run_until_complete(main_task)
     except (Shutdown, KeyboardInterrupt):
         pass
 
     if args.production:
         loop.run_until_complete(worker.drain(timeout=args.drain_timeout))
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/cli/log.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/log.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/cli/protocol.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/protocol.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 class CliArgs:
     opts: WorkerOptions
     log_level: str
     production: bool
     asyncio_debug: bool
     watch: bool
     drain_timeout: int
+    room: str = ""
+    participant_identity: str = ""
     cch: ipc_enc.ProcessPipe | None = None  # None when watch is disabled
 
 
 @define(kw_only=True)
 class ActiveJobsRequest:
     MSG_ID: ClassVar[int] = 1
 
@@ -35,31 +37,29 @@
 
 @define(kw_only=True)
 class ActiveJobsResponse:
     MSG_ID: ClassVar[int] = 2
     jobs: list[ActiveJob] = Factory(list)
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.jobs).to_bytes(4, "big"))
+        ipc_enc._write_int(b, len(self.jobs))
         for aj in self.jobs:
             job_s = aj.job.SerializeToString()
-            b.write(len(job_s).to_bytes(4, "big"))
-            b.write(job_s)
+            ipc_enc._write_bytes(b, job_s)
             accept_s = pickle.dumps(aj.accept_data)
-            b.write(len(accept_s).to_bytes(4, "big"))
-            b.write(accept_s)
+            ipc_enc._write_bytes(b, accept_s)
 
     def read(self, b: io.BytesIO) -> None:
-        job_count = int.from_bytes(b.read(4), "big")
+        job_count = ipc_enc._read_int(b)
         for _ in range(job_count):
-            job_len = int.from_bytes(b.read(4), "big")
+            job_s = ipc_enc._read_bytes(b)
             job = agent.Job()
-            job.ParseFromString(b.read(job_len))
-            accept_len = int.from_bytes(b.read(4), "big")
-            accept_data = pickle.loads(b.read(accept_len))
+            job.ParseFromString(job_s)
+            accept_s = ipc_enc._read_bytes(b)
+            accept_data = pickle.loads(accept_s)
             self.jobs.append(ActiveJob(job=job, accept_data=accept_data))
 
 
 @define(kw_only=True)
 class ReloadJobsRequest:
     MSG_ID: ClassVar[int] = 3
 
@@ -72,19 +72,18 @@
 
 @define(kw_only=True)
 class ReloadJobsResponse:
     MSG_ID: ClassVar[int] = 4
     jobs: list[ActiveJob] = Factory(list)
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.jobs).to_bytes(4, "big"))
+        ipc_enc._write_int(b, len(self.jobs))
         for aj in self.jobs:
             job_s = aj.job.SerializeToString()
-            b.write(len(job_s).to_bytes(4, "big"))
-            b.write(job_s)
+            ipc_enc._write_bytes(b, job_s)
             accept_s = pickle.dumps(aj.accept_data)
             b.write(len(accept_s).to_bytes(4, "big"))
             b.write(accept_s)
 
     def read(self, b: io.BytesIO) -> None:
         job_count = int.from_bytes(b.read(4), "big")
         for _ in range(job_count):
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/cli/watcher.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/watcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,17 +39,21 @@
 
     def run(self) -> None:
         packages = []
 
         if self._watch_plugins:
             # also watch plugins that are installed in editable mode
             # this is particulary useful when developing plugins
-            packages.append(Distribution.from_name("livekit.agents"))
-            for p in Plugin.registered_plugins:
-                packages.append(Distribution.from_name(p.package))
+            try:
+                packages.append(Distribution.from_name("livekit.agents"))
+                for p in Plugin.registered_plugins:
+                    packages.append(Distribution.from_name(p.package))
+            except Exception:
+                # TODO(theomonnom): distribution isn't found on Python 3.9
+                pass
 
         paths: list[str | pathlib.Path] = [self._main_file.absolute()]
         for p in packages:
             # https://packaging.python.org/en/latest/specifications/direct-url/
             durl = p.read_text("direct_url.json")
             if not durl:
                 continue
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/codecs/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/codecs/mp3.py` & `livekit_agents-0.7.dev0/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/http_server.py` & `livekit_agents-0.7.dev0/livekit/agents/http_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 
 from aiohttp import web
 
 
 async def health_check(_):
     return web.Response(text="OK")
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/ipc/job_main.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/job_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import contextlib
 import logging
 import traceback
 
 from livekit import rtc
 
-from .. import aio, apipe, ipc_enc
+from .. import aio, apipe, ipc_enc, utils
 from ..job_context import JobContext, _ShutdownInfo
 from ..job_request import AutoSubscribe
 from ..log import logger
 from ..utils import time_ms
 from . import protocol
 
 
@@ -42,14 +42,15 @@
         except Exception as e:
             print(f"failed to log {record.filename}:{record.lineno}, exception '{e}'")
 
 
 async def _start(
     pipe: apipe.AsyncPipe, args: protocol.JobMainArgs, room: rtc.Room
 ) -> None:
+    utils.http_context._new_session_ctx()
     close_tx, close_rx = aio.channel()  # used by the JobContext to signal shutdown
 
     auto_subscribe = args.accept_data.auto_subscribe
     opts = rtc.RoomOptions(auto_subscribe=auto_subscribe == AutoSubscribe.SUBSCRIBE_ALL)
 
     cnt = room.connect(args.url, args.token, options=opts)
     start_req: protocol.StartJobRequest | None = None
@@ -106,15 +107,16 @@
         usertask.add_done_callback(log_exception)
         await pipe.write(protocol.StartJobResponse())
 
     @room.on("disconnected")
     def on_disconnected():
         close_tx.send_nowait(_ShutdownInfo(reason="room disconnected"))
 
-    async with contextlib.aclosing(aio.select([pipe, cnt, close_rx])) as select:
+    select = aio.select([pipe, cnt, close_rx])
+    try:
         while True:
             s = await select()
             if s.selected is cnt:
                 if s.exc:
                     error = "".join(traceback.format_exception_only(type(s.exc), s.exc))
                     await pipe.write(protocol.StartJobResponse(error=error))
                     break  # failed to connect, break and exit the process
@@ -132,23 +134,27 @@
                 start_req = msg
                 await _start_if_valid()
             if isinstance(msg, protocol.Ping):
                 last_timestamp = msg.timestamp
                 await pipe.write(
                     protocol.Pong(last_timestamp=last_timestamp, timestamp=time_ms())
                 )
+    finally:
+        await select.aclose()
 
     logger.debug("disconnecting from room")
     await room.disconnect()
 
     with contextlib.suppress(Exception):
         # exceptions are already logged inside the done_callback
         if usertask is not None:
             await usertask  # type: ignore
 
+    await utils.http_context._close_http_ctx()
+
     if shutting_down:
         await pipe.write(protocol.ShutdownResponse())
 
 
 def _run_job(cch: ipc_enc.ProcessPipe, args: protocol.JobMainArgs) -> None:
     """Entry point for a job process"""
     loop = asyncio.new_event_loop()
@@ -161,15 +167,15 @@
     # current process pid
     logger.debug(
         "process started",
         extra={"url": args.url},
     )
 
     pipe = apipe.AsyncPipe(cch, loop, protocol.IPC_MESSAGES)
-    loop.slow_callback_duration = 0.02  # 20ms
+    loop.slow_callback_duration = 0.03  # 30ms
     aio.debug.hook_slow_callbacks(0.75)
     loop.set_debug(args.asyncio_debug)
 
     room = rtc.Room(loop=loop)
     main_task = loop.create_task(_start(pipe, args, room))
 
     try:
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/ipc/job_process.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/job_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 import logging
 import multiprocessing as mp
 import sys
 import threading
 
@@ -44,17 +46,16 @@
         start_timeout = asyncio.sleep(consts.START_TIMEOUT)
         ping_interval = aio.interval(consts.PING_INTERVAL)
         pong_timeout = aio.sleep(consts.PING_TIMEOUT)
 
         start_res: protocol.StartJobResponse | None = None
 
         await self._pipe.write(protocol.StartJobRequest(job=self._job))
-        async with contextlib.aclosing(
-            aio.select([self._pipe, start_timeout, ping_interval, pong_timeout])
-        ) as select:
+        select = aio.select([self._pipe, start_timeout, ping_interval, pong_timeout])
+        try:
             while True:
                 s = await select()
                 if s.selected is start_timeout and start_res is None:
                     logger.error(
                         "process start timed out, killing job",
                         extra=self.logging_extra(),
                     )
@@ -104,14 +105,16 @@
                     res, protocol.ShutdownResponse
                 ):
                     logger.info(
                         "job exiting",
                         extra={"exit": res, **self.logging_extra()},
                     )
                     break
+        finally:
+            await select.aclose()
 
         await self.join()
         logger.info("job process closed", extra=self.logging_extra())
 
     async def join(self) -> None:
         def _join_process():
             try:
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/ipc/protocol.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/ipc_enc.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc_enc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import struct
 from typing import ClassVar, Protocol, Type
 
 
 class ProcessPipeReader(Protocol):
     def recv_bytes(self, maxlength: int | None = None) -> bytes: ...
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/job_context.py` & `livekit_agents-0.7.dev0/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/job_request.py` & `livekit_agents-0.7.dev0/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/llm/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/llm/function_context.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/llm/llm.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import abc
 import enum
 from typing import Callable
 
 from attrs import define
 
 from .function_context import FunctionContext
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/plugin.py` & `livekit_agents-0.7.dev0/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/stt/stream_adapter.py` & `livekit_agents-0.7.dev0/livekit/agents/stt/stream_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import logging
+from typing import Optional
 
 from livekit import rtc
 
-from ..log import logger
 from ..utils import AudioBuffer, merge_frames
-from ..vad import VADEventType, VADStream
+from ..vad import VAD, VADEventType
 from .stt import (
     STT,
     SpeechEvent,
     SpeechEventType,
     SpeechStream,
 )
 
 
 class StreamAdapter(STT):
     def __init__(
         self,
+        *,
         stt: STT,
-        vad_stream: VADStream,
+        vad: VAD,
     ) -> None:
         super().__init__(streaming_supported=True)
-        self._vad = vad_stream
+        self._vad = vad
         self._stt = stt
 
     @property
     def wrapped_stt(self) -> STT:
         return self._stt
 
     async def recognize(self, *, buffer: AudioBuffer, language: str | None = None):
@@ -48,70 +49,71 @@
             language=language,
         )
 
 
 class StreamAdapterWrapper(SpeechStream):
     def __init__(
         self,
-        vad_stream: VADStream,
+        vad: VAD,
         stt: STT,
         *args,
         **kwargs,
     ) -> None:
         super().__init__()
-        self._vad = vad_stream
+        self._vad = vad
         self._stt = stt
-        self._event_queue = asyncio.Queue[SpeechEvent | None]()
+        self._event_queue = asyncio.Queue[Optional[SpeechEvent]]()
+        self._main_task = asyncio.create_task(self._run())
+        self._vad_stream = self._vad.stream()
         self._closed = False
         self._args = args
         self._kwargs = kwargs
 
-        self._main_task = asyncio.create_task(self._run())
-
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logger.error(f"stream adapter task failed: {task.exception()}")
-
-        self._main_task.add_done_callback(log_exception)
-
+    # TODO(theomonnom): smarter adapter, create interim results using another STT?
     async def _run(self) -> None:
         try:
-            async for event in self._vad:
+            async for event in self._vad_stream:
                 if event.type == VADEventType.START_OF_SPEECH:
                     start_event = SpeechEvent(SpeechEventType.START_OF_SPEECH)
                     self._event_queue.put_nowait(start_event)
                 elif event.type == VADEventType.END_OF_SPEECH:
                     merged_frames = merge_frames(event.frames)
                     event = await self._stt.recognize(
                         buffer=merged_frames, *self._args, **self._kwargs
                     )
                     self._event_queue.put_nowait(event)
 
+                    final_event = SpeechEvent(
+                        type=SpeechEventType.FINAL_TRANSCRIPT,
+                        alternatives=[event.alternatives[0]],
+                    )
+                    self._event_queue.put_nowait(final_event)
+
                     end_event = SpeechEvent(
                         type=SpeechEventType.END_OF_SPEECH,
                         alternatives=[event.alternatives[0]],
                     )
                     self._event_queue.put_nowait(end_event)
-        except Exception as e:
-            logging.exception(f"stream adapter failed: {e}")
+        except Exception:
+            logging.exception("stt stream adapter failed")
         finally:
             self._event_queue.put_nowait(None)
 
     def push_frame(self, frame: rtc.AudioFrame) -> None:
         if self._closed:
             raise ValueError("cannot push frame to closed stream")
 
-        self._vad.push_frame(frame)
+        self._vad_stream.push_frame(frame)
 
     async def aclose(self, *, wait: bool = True) -> None:
         self._closed = True
         if not wait:
             self._main_task.cancel()
 
-        await self._vad.aclose(wait=wait)
+        await self._vad_stream.aclose(wait=wait)
         with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
 
     async def __anext__(self) -> SpeechEvent:
         evt = await self._event_queue.get()
         if evt is None:
             raise StopAsyncIteration
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/stt/stt.py` & `livekit_agents-0.7.dev0/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/tts/stream_adapter.py` & `livekit_agents-0.7.dev0/livekit/agents/tts/stream_adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,87 @@
+from __future__ import annotations
+
 import asyncio
-from typing import AsyncIterable
+import contextlib
+from typing import Optional
 
-from ..log import logger
-from ..tokenize import SentenceStream, SentenceTokenizer
+from .. import tokenize
 from .tts import (
     TTS,
+    ChunkedStream,
     SynthesisEvent,
     SynthesisEventType,
-    SynthesizedAudio,
     SynthesizeStream,
 )
 
 
+class StreamAdapter(TTS):
+    def __init__(
+        self, *, tts: TTS, sentence_tokenizer: tokenize.SentenceTokenizer
+    ) -> None:
+        super().__init__(
+            streaming_supported=True,
+            sample_rate=tts.sample_rate,
+            num_channels=tts.num_channels,
+        )
+        self._tts = tts
+        self._sentence_tokenizer = sentence_tokenizer
+
+    def synthesize(self, text: str) -> ChunkedStream:
+        return self._tts.synthesize(text=text)
+
+    def stream(self) -> SynthesizeStream:
+        return StreamAdapterWrapper(
+            tts=self._tts, sentence_tokenizer=self._sentence_tokenizer
+        )
+
+
 class StreamAdapterWrapper(SynthesizeStream):
-    def __init__(self, tts: TTS, sentence_stream: SentenceStream) -> None:
+    def __init__(
+        self, *, tts: TTS, sentence_tokenizer: tokenize.SentenceTokenizer
+    ) -> None:
         super().__init__()
         self._closed = False
         self._tts = tts
-        self._sentence_stream = sentence_stream
-        self._queue = asyncio.Queue[str]()
-        self._event_queue = asyncio.Queue[SynthesisEvent]()
-
+        self._sentence_tokenizer = sentence_tokenizer
+        self._sentence_stream = self._sentence_tokenizer.stream()
+        self._event_queue = asyncio.Queue[Optional[SynthesisEvent]]()
         self._main_task = asyncio.create_task(self._run())
 
-        def log_exception(task: asyncio.Task) -> None:
-            if not task.cancelled() and task.exception():
-                logger.error(f"speech task failed: {task.exception()}")
-
-        self._main_task.add_done_callback(log_exception)
-
     async def _run(self) -> None:
-        while True:
-            try:
-                sentence = await self._sentence_stream.__anext__()
-                audio = await self._tts.synthesize(text=sentence.text)
+        async for ev in self._sentence_stream:
+            if ev.type == tokenize.TokenEventType.STARTED:
                 self._event_queue.put_nowait(
                     SynthesisEvent(type=SynthesisEventType.STARTED)
                 )
-                self._event_queue.put_nowait(
-                    SynthesisEvent(type=SynthesisEventType.AUDIO, audio=audio)
-                )
+            elif ev.type == tokenize.TokenEventType.TOKEN:
+                async for audio in self._tts.synthesize(text=ev.token):
+                    self._event_queue.put_nowait(
+                        SynthesisEvent(type=SynthesisEventType.AUDIO, audio=audio)
+                    )
+            elif ev.type == tokenize.TokenEventType.FINISHED:
                 self._event_queue.put_nowait(
                     SynthesisEvent(type=SynthesisEventType.FINISHED)
                 )
-            except asyncio.CancelledError:
-                break
+        self._event_queue.put_nowait(None)
 
-        self._closed = True
+    def push_text(self, token: str | None) -> None:
+        if self._closed:
+            raise ValueError("cannot push frame to closed stream")
 
-    def push_text(self, token: str) -> None:
         self._sentence_stream.push_text(token)
 
-    async def flush(self) -> None:
-        await self._sentence_stream.flush()
+    async def aclose(self, *, wait: bool = True) -> None:
+        self._closed = True
+        if not wait:
+            self._main_task.cancel()
 
-    async def aclose(self) -> None:
-        self._main_task.cancel()
-        try:
+        await self._sentence_stream.aclose(wait=wait)
+        with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
-        except asyncio.CancelledError:
-            pass
-        finally:
-            self._event_queue.put_nowait(None)
 
     async def __anext__(self) -> SynthesisEvent:
-        item = await self._event_queue.get()
-        if item is None:
+        evt = await self._event_queue.get()
+        if evt is None:
             raise StopAsyncIteration
 
-        return item
-
-
-class StreamAdapter(TTS):
-    def __init__(self, tts: TTS, tokenizer: SentenceTokenizer) -> None:
-        super().__init__(streaming_supported=True)
-        self._tts = tts
-        self._tokenizer = tokenizer
-
-    def synthesize(self, *, text: str) -> AsyncIterable[SynthesizedAudio]:
-        return self._tts.synthesize(text=text)
-
-    def stream(self) -> SynthesizeStream:
-        return StreamAdapterWrapper(self._tts, self._tokenizer.stream())
+        return evt
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/tts/tts.py` & `livekit_agents-0.7.dev0/livekit/agents/tts/tts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import AsyncIterable
+from typing import AsyncIterator
 
 from livekit import rtc
 
+from ..utils import misc
+
 
 @dataclass
 class SynthesizedAudio:
     text: str
     data: rtc.AudioFrame
 
 
@@ -27,14 +29,41 @@
 
 @dataclass
 class SynthesisEvent:
     type: SynthesisEventType
     audio: SynthesizedAudio | None = None
 
 
+class ChunkedStream(ABC):
+    """
+    Used by the non-streamed synthesize API, some providers support chunked http responses
+    """
+
+    async def collect(self) -> rtc.AudioFrame:
+        """
+        Utility method to collect every frame in a single call
+        """
+        frames = []
+        async for ev in self:
+            frames.append(ev.data)
+
+        return misc.merge_frames(frames)
+
+    @abstractmethod
+    async def __anext__(self) -> SynthesizedAudio: ...
+
+    @abstractmethod
+    async def aclose(self) -> None:
+        """close is automatically called if the stream is completely collected"""
+        ...
+
+    def __aiter__(self) -> AsyncIterator[SynthesizedAudio]:
+        return self
+
+
 class SynthesizeStream(ABC):
     @abstractmethod
     def push_text(self, token: str | None) -> None:
         """
         Push some text to be synthesized. If token is None,
         it will be used to identify the end of this particular segment.
         (required by some TTS engines)
@@ -77,16 +106,15 @@
         return self._sample_rate
 
     @property
     def num_channels(self) -> int:
         return self._num_channels
 
     @abstractmethod
-    def synthesize(self, text: str) -> AsyncIterable[SynthesizedAudio]:
-        raise NotImplementedError("synthesize is not implemented")
+    def synthesize(self, text: str) -> ChunkedStream: ...
 
     def stream(self) -> SynthesizeStream:
         raise NotImplementedError(
             "streaming is not supported by this TTS, please use a different TTS or use a StreamAdapter"
         )
 
     @property
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/utils/event_emitter.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/event_emitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 class EventEmitter(Generic[T]):
     def __init__(self) -> None:
         self._events: Dict[T, Set[Callable]] = dict()
 
     def emit(self, event: T, *args, **kwargs) -> None:
         if event in self._events:
-            for callback in self._events[event]:
+            callables = self._events[event].copy()
+            for callback in callables:
                 callback(*args, **kwargs)
 
     def once(self, event: T, callback: Optional[Callable] = None) -> Callable:
         if callback is not None:
 
             def once_callback(*args, **kwargs):
                 self.off(event, once_callback)
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/utils/exp_filter.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/exp_filter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/utils/misc.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/misc.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/utils/moving_average.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/moving_average.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/vad.py` & `livekit_agents-0.7.dev0/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/version.py` & `livekit_agents-0.7.dev0/livekit/agents/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.dev1"
+__version__ = "0.7.dev0"
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/voice_assistant/assistant.py` & `livekit_agents-0.7.dev0/livekit/agents/voice_assistant/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import asyncio
 import contextlib
 import contextvars
 import time
 from typing import Any, AsyncIterable, Callable, Literal
 
 from attrs import define
 from livekit import rtc
 
-from .. import aio, utils
+from .. import aio, tokenize, transcription, utils
 from .. import llm as allm
 from .. import stt as astt
 from .. import tts as atts
 from .. import vad as avad
 from ..log import logger
 from . import plotter
 
@@ -40,14 +42,19 @@
 class _AssistantOptions:
     plotting: bool
     debug: bool
     allow_interruptions: bool
     int_speech_duration: float
     int_min_words: int
     base_volume: float
+    transcription: bool
+    word_tokenizer: tokenize.WordTokenizer
+    sentence_tokenizer: tokenize.SentenceTokenizer
+    hyphenate_word: Callable[[str], list[str]]
+    transcription_speed: float
 
 
 @define(kw_only=True, frozen=True)
 class _StartArgs:
     room: rtc.Room
     participant: rtc.RemoteParticipant | str | None
 
@@ -110,24 +117,34 @@
         interrupt_volume: float = 0.05,
         interrupt_speech_duration: float = 0.7,
         interrupt_min_words: int = 3,
         base_volume: float = 1.0,
         debug: bool = False,
         plotting: bool = False,
         loop: asyncio.AbstractEventLoop | None = None,
+        transcription: bool = True,
+        sentence_tokenizer: tokenize.SentenceTokenizer = tokenize.basic.SentenceTokenizer(),
+        word_tokenizer: tokenize.WordTokenizer = tokenize.basic.WordTokenizer(),
+        hyphenate_word: Callable[[str], list[str]] = tokenize.basic.hyphenate_word,
+        transcription_speed: float = 4,
     ) -> None:
         super().__init__()
         self._loop = loop or asyncio.get_event_loop()
         self._opts = _AssistantOptions(
             plotting=plotting,
             debug=debug,
             allow_interruptions=allow_interruptions,
             int_speech_duration=interrupt_speech_duration,
             int_min_words=interrupt_min_words,
             base_volume=base_volume,
+            transcription=transcription,
+            sentence_tokenizer=sentence_tokenizer,
+            word_tokenizer=word_tokenizer,
+            hyphenate_word=hyphenate_word,
+            transcription_speed=transcription_speed,
         )
         self._vad, self._tts, self._llm, self._stt = vad, tts, llm, stt
         self._fnc_ctx = fnc_ctx
         self._chat_ctx = chat_ctx or allm.ChatContext()
         self._speaking, self._user_speaking = False, False
         self._plotter = plotter.AssistantPlotter(self._loop)
 
@@ -171,16 +188,16 @@
                 - user_started_speaking: the user started speaking
                 - user_stopped_speaking: the user stopped speaking
                 - agent_started_speaking: the agent started speaking
                 - agent_stopped_speaking: the agent stopped speaking
                 - user_speech_committed: the user speech was committed to the chat context
                 - agent_speech_committed: the agent speech was committed to the chat context
                 - agent_speech_interrupted: the agent speech was interrupted
-                - function_calls_completed: all function calls have been completed
-                - will_synthesize_llm: the assistant will synthesize the LLM output
+                - function_calls_collected: received the complete set of functions to be executed
+                - function_calls_finished: all function calls have been completed
             callback: the callback to call when the event is emitted
         """
         return super().on(event, callback)
 
     @property
     def chat_context(self) -> allm.ChatContext:
         return self._chat_ctx
@@ -190,22 +207,22 @@
         return self._started
 
     async def say(
         self,
         source: str | allm.LLMStream | AsyncIterable[str],
         allow_interruptions: bool = True,
         add_to_ctx: bool = True,
-        stream: bool = True,
+        force_stream: bool = False,  # force the usage of TTS stream
         enqueue: bool = True,
     ) -> None:
         with contextlib.suppress(asyncio.CancelledError):
             if not self._started:
                 await self._start_future
 
-        if isinstance(source, str) and stream:
+        if isinstance(source, str) and force_stream:
             text = source
 
             async def _gen():
                 yield text
 
             source = _gen()
 
@@ -241,39 +258,14 @@
         room.on("track_published", self._on_track_published)
         room.on("track_subscribed", self._on_track_subscribed)
         room.on("track_unsubscribed", self._on_track_unsubscribed)
         room.on("participant_connected", self._on_participant_connected)
 
         self._launch_task = asyncio.create_task(self._launch())
 
-    def _mark_dirty(self):
-        """Called when the AudioStream isn't valid anymore (microphone unsubscribed or participant
-        disconnected)"""
-        if not self._ready:
-            logger.warning("assistant already marked as dirty")
-            return
-
-        self._log_debug("marking assistant as dirty")
-        self._ready = False
-
-        if self._recognize_task is not None:
-            self._recognize_task.cancel()
-
-    def _mark_ready(self, audio_stream: rtc.AudioStream):
-        """We have everything we need to start the voice assistant (audio sources & audio
-        streams)"""
-        if self._ready:
-            logger.warning("assistant already marked as ready")
-            return
-
-        self._log_debug("marking assistant as ready")
-        self._audio_stream = audio_stream
-        self._ready = True
-        self._recognize_task = asyncio.create_task(self._recognize_loop())
-
     async def aclose(self, wait: bool = True) -> None:
         if not self.started:
             return
 
         self._closed = True
         self._start_future.cancel()
 
@@ -371,50 +363,52 @@
         pub: rtc.RemoteTrackPublication,
         participant: rtc.RemoteParticipant,
     ):
         if participant.identity != self._linked_participant:
             return
 
         if pub.source == rtc.TrackSource.SOURCE_MICROPHONE:
-            audio_stream = rtc.AudioStream(track)
-            self._stream_ready(audio_stream)
+            self._user_track_ready(track)  # type: ignore
 
     def _on_track_unsubscribed(
         self,
         track: rtc.RemoteTrack,
         pub: rtc.RemoteTrackPublication,
         participant: rtc.RemoteParticipant,
     ):
         if participant.identity != self._linked_participant:
             return
 
         if pub.source == rtc.TrackSource.SOURCE_MICROPHONE:
-            self._stream_dirty()
+            self._user_track_dirty()
 
-    def _stream_dirty(self):
+    def _user_track_dirty(self):
         """Called when the AudioStream isn't valid anymore (microphone unsubscribed or participant
         disconnected)"""
         if not self._ready:
             logger.warning("assistant already marked as dirty")
             return
 
         self._log_debug("marking assistant as dirty")
         self._ready = False
 
         if self._recognize_task is not None:
             self._recognize_task.cancel()
 
-    def _stream_ready(self, audio_stream: rtc.AudioStream):
+    def _user_track_ready(self, user_track: rtc.AudioTrack):
         """We have everything we need to start the voice assistant (audio sources & audio
         streams)"""
         if self._ready:
             logger.warning("assistant already marked as ready")
             return
 
+        audio_stream = rtc.AudioStream(user_track)
+
         self._log_debug("marking assistant as ready")
+        self._user_track = user_track
         self._audio_stream = audio_stream
         self._ready = True
         self._recognize_task = asyncio.create_task(self._recognize_loop())
 
     def _recv_final_transcript(self, ev: astt.SpeechEvent):
         self._log_debug(f"assistant - received transcript {ev.alternatives[0].text}")
         self._transcripted_text += ev.alternatives[0].text
@@ -466,14 +460,22 @@
     async def _recognize_loop(self):
         """Recognize speech from the audio stream and do voice activity detection"""
         assert self._audio_stream is not None
 
         vad_stream = self._vad.stream()
         stt_stream = self._stt.stream()
 
+        stt_forwarder = utils._noop.Nop()
+        if self._opts.transcription:
+            stt_forwarder = transcription.STTSegmentsForwarder(
+                room=self._start_args.room,
+                participant=self._linked_participant,
+                track=self._user_track,
+            )
+
         select = aio.select([self._audio_stream, vad_stream, stt_stream])
         try:
             while True:
                 s = await select()
                 if s.selected is self._audio_stream:
                     audio_event: rtc.AudioFrameEvent = s.result()
                     stt_stream.push_frame(audio_event.frame)
@@ -486,23 +488,25 @@
                     elif vad_event.type == avad.VADEventType.INFERENCE_DONE:
                         self._did_vad_inference(vad_event)
                     elif vad_event.type == avad.VADEventType.END_OF_SPEECH:
                         self._user_stopped_speaking(vad_event.duration)
 
                 if s.selected is stt_stream:
                     stt_event = s.result()
+                    stt_forwarder.update(stt_event)
                     if stt_event.type == astt.SpeechEventType.FINAL_TRANSCRIPT:
                         self._recv_final_transcript(stt_event)
                     elif stt_event.type == astt.SpeechEventType.INTERIM_TRANSCRIPT:
                         self._recv_interim_transcript(stt_event)
                     elif stt_event.type == astt.SpeechEventType.END_OF_SPEECH:
                         self._transcript_finished(stt_event)
         except Exception:
             logger.exception("error in recognize loop")
         finally:
+            await stt_forwarder.aclose(wait=False)
             await stt_stream.aclose(wait=False)
             await vad_stream.aclose(wait=False)
             await select.aclose()
 
     async def _update_loop(self):
         """Update the volume every 10ms based on the speech probability"""
         speech_prob_avg = utils.MovingAverage(100)  # avg over 1s
@@ -639,21 +643,35 @@
 
         self._play_task = asyncio.create_task(self._play_speech_if_validated(data))
 
     async def _play_speech_if_validated(self, data: _SpeechData) -> None:
         """
         Start synthesis and playout the speech only if validated
         """
-        self._log_debug(f"assistant - maybe_play_speech {data}")
+        self._log_debug(f"assistant - play_speech_if_validated {data}")
         assert data.source is not None
 
         # reset volume before starting a new speech
         self._vol_filter.reset()
         po_tx, po_rx = aio.channel()  # playout channel
-        tts_co = self._synthesize_task(data, po_tx)
+
+        tts_forwarder = utils._noop.Nop()
+        if self._opts.transcription:
+            tts_forwarder = transcription.TTSSegmentsForwarder(
+                room=self._start_args.room,
+                participant=self._start_args.room.local_participant,
+                track=self._pub.sid,
+                auto_playout=False,
+                sentence_tokenizer=self._opts.sentence_tokenizer,
+                word_tokenizer=self._opts.word_tokenizer,
+                hyphenate_word=self._opts.hyphenate_word,
+                speed=self._opts.transcription_speed,
+            )
+
+        tts_co = self._synthesize_task(data, po_tx, tts_forwarder)
         _synthesize_task = asyncio.create_task(tts_co)
 
         try:
             with contextlib.suppress(aio.ChanClosed):
                 await data.val_ch.recv()  # wait for speech validation before playout
 
             # validated!
@@ -664,15 +682,15 @@
             if data.answering_user_speech is not None:
                 msg = allm.ChatMessage(
                     text=data.answering_user_speech, role=allm.ChatRole.USER
                 )
                 self._chat_ctx.messages.append(msg)
                 self.emit("user_speech_committed", self._chat_ctx, msg)
 
-            await self._playout_task(po_rx)
+            await self._playout_task(po_rx, tts_forwarder)
 
             msg = allm.ChatMessage(
                 text=data.collected_text,
                 role=allm.ChatRole.ASSISTANT,
             )
 
             if data.add_to_ctx:
@@ -681,48 +699,55 @@
                     self.emit("agent_speech_interrupted", self._chat_ctx, msg)
                 else:
                     self.emit("agent_speech_committed", self._chat_ctx, msg)
 
             self._log_debug(
                 "assistant - playout finished", extra={"interrupted": data.interrupted}
             )
+
         except Exception:
             logger.exception("error while playing speech")
         finally:
             self._playing_speech = None
             with contextlib.suppress(asyncio.CancelledError):
                 _synthesize_task.cancel()
                 await _synthesize_task
 
-            self._log_debug("assistant - maybe_play_speech finished")
+            await tts_forwarder.aclose()
+            self._log_debug("assistant - play_speech_if_validated finished")
 
     async def _synthesize_task(
         self,
         data: _SpeechData,
         po_tx: aio.ChanSender[rtc.AudioFrame],
+        tts_forwarder: transcription.TTSSegmentsForwarder | utils._noop.Nop,
     ) -> None:
         """Synthesize speech from the source"""
         assert data.source is not None
         self._log_debug("tts inference started")
 
         if isinstance(data.source, str):
             # No streaming is needed, use the TTS directly
             # This should be faster when the whole text is known in advance
             # (no buffering on the provider side)
             data.collected_text = data.source
+            tts_forwarder.push_text(data.source)
+            tts_forwarder.mark_text_segment_end()
             _start_time = time.time()
             _first_frame = True
             async for audio in self._tts.synthesize(data.source):
                 if _first_frame:
                     dt = time.time() - _start_time
                     _first_frame = False
                     self._log_debug(f"assistant - tts first frame in {dt:.2f}s")
 
+                tts_forwarder.push_audio(audio.data)
                 po_tx.send_nowait(audio.data)
 
+            tts_forwarder.mark_audio_segment_end()
             po_tx.close()
             self._log_debug("tts inference finished")
             return
 
         # otherwise, stream the text to the TTS..
         tts_stream = self._tts.stream()
 
@@ -739,45 +764,53 @@
                         dt = time.time() - _start_time
                         _first_frame = False
                         self._log_debug(
                             f"assistant - tts first frame in {dt:.2f}s (streamed)"
                         )
 
                     assert event.audio is not None
+                    tts_forwarder.push_audio(event.audio.data)
                     po_tx.send_nowait(event.audio.data)
 
+            tts_forwarder.mark_audio_segment_end()
+
         _forward_task = asyncio.create_task(_forward_stream())
         try:
             if isinstance(data.source, allm.LLMStream):
                 # stream the LLM output to the TTS
                 assistant_ctx = AssistantContext(self, data.source)
                 token = _ContextVar.set(assistant_ctx)
                 async for chunk in data.source:
                     alt = chunk.choices[0].delta.content
                     if not alt:
                         continue
                     data.collected_text += alt
+                    tts_forwarder.push_text(alt)
                     tts_stream.push_text(alt)
 
+                tts_forwarder.mark_text_segment_end()
                 tts_stream.mark_segment_end()
+
                 if len(data.source.called_functions) > 0:
                     self.emit("function_calls_collected", assistant_ctx)
 
                 await data.source.aclose()
 
                 if len(data.source.called_functions) > 0:
                     self.emit("function_calls_finished", assistant_ctx)
 
                 _ContextVar.reset(token)
             else:
                 # user defined source, stream the text to the TTS
                 async for seg in data.source:
                     data.collected_text += seg
+                    tts_forwarder.push_text(seg)
                     tts_stream.push_text(seg)
 
+                tts_forwarder.mark_text_segment_end()
                 tts_stream.mark_segment_end()
 
             await tts_stream.aclose()
         except Exception:
             logger.exception("error while streaming text to TTS")
         finally:
             po_tx.close()
@@ -786,14 +819,15 @@
                 await _forward_task
 
             self._log_debug("tts inference finished")
 
     async def _playout_task(
         self,
         po_rx: aio.ChanReceiver[rtc.AudioFrame],
+        tts_forwarder: transcription.TTSSegmentsForwarder | utils._noop.Nop,
     ) -> None:
         """Playout the synthesized speech with volume control"""
         assert self._audio_source is not None
 
         sample_idx = 0
         first_frame = True
 
@@ -801,16 +835,17 @@
             eps = 1e-6
             assert self._playing_speech is not None
             return (
                 self._playing_speech.interrupted and self._vol_filter.filtered() <= eps
             )
 
         async for buf in po_rx:
-            if first_frame and self._opts.debug:
+            if first_frame:
                 self._agent_started_speaking()
+                tts_forwarder.segment_playout_started()  # we have only one segment
                 first_frame = False
 
             if _should_break():
                 break
 
             i = 0
             while i < len(buf.data):
@@ -825,20 +860,21 @@
                 dt = 1 / len(data)
                 for si in range(0, len(data)):
                     vol = self._vol_filter.apply(dt, self._target_volume)
                     j = data[si] / 32768
                     data[si] = int(j * vol * 32768)
                     sample_idx += 1
 
-                frame = rtc.AudioFrame(
-                    data=data.tobytes(),
-                    sample_rate=buf.sample_rate,
-                    num_channels=buf.num_channels,
-                    samples_per_channel=rem,
+                await self._audio_source.capture_frame(
+                    rtc.AudioFrame(
+                        data=data.tobytes(),
+                        sample_rate=buf.sample_rate,
+                        num_channels=buf.num_channels,
+                        samples_per_channel=rem,
+                    )
                 )
-                await self._audio_source.capture_frame(frame)
 
         self._agent_stopped_speaking()
 
     def _log_debug(self, msg: str, **kwargs) -> None:
         if self._opts.debug:
             logger.debug(msg, **kwargs)
```

### Comparing `livekit_agents-0.6.dev1/livekit/agents/voice_assistant/plotter.py` & `livekit_agents-0.7.dev0/livekit/agents/voice_assistant/plotter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.6.dev1/livekit/agents/worker.py` & `livekit_agents-0.7.dev0/livekit/agents/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
 import asyncio
 import contextlib
 import os
 from typing import (
     Callable,
     Coroutine,
+    Literal,
 )
 from urllib.parse import urlparse
 
 import aiohttp
 import psutil
 from attr import define
 from livekit import api
 from livekit.protocol import agent, models
 
-from . import aio, consts, http_server, ipc
+from . import aio, consts, http_server, ipc, utils
 from .job_request import AcceptData, AvailRes, JobRequest
 from .log import logger
 from .version import __version__
 
 JobRequestFnc = Callable[[JobRequest], Coroutine]
 LoadFnc = Callable[[], float]
 
@@ -44,14 +45,15 @@
 
 @define(kw_only=True)
 class WorkerPermissions:
     can_publish: bool = True
     can_subscribe: bool = True
     can_publish_data: bool = True
     can_update_metadata: bool = True
+    can_publish_sources: list[models.TrackSource] = []
     hidden: bool = False
 
 
 # NOTE: this object must be pickle-able
 @define
 class WorkerOptions:
     request_fnc: JobRequestFnc
@@ -70,234 +72,314 @@
 
 @define(kw_only=True)
 class ActiveJob:
     job: agent.Job
     accept_data: AcceptData
 
 
-class Worker:
+EventTypes = Literal["worker_registered"]
+
+
+class Worker(utils.EventEmitter[EventTypes]):
     def __init__(
         self,
         opts: WorkerOptions,
         *,
         loop: asyncio.AbstractEventLoop | None = None,
     ) -> None:
+        super().__init__()
         opts.ws_url = opts.ws_url or opts.ws_url or os.environ.get("LIVEKIT_URL") or ""
         opts.api_key = opts.api_key or os.environ.get("LIVEKIT_API_KEY") or ""
         opts.api_secret = opts.api_secret or os.environ.get("LIVEKIT_API_SECRET") or ""
 
+        if not opts.ws_url:
+            raise ValueError(
+                "ws_url is required, or add LIVEKIT_URL in your environment"
+            )
+
+        if not opts.api_key:
+            raise ValueError(
+                "api_key is required, or add LIVEKIT_API_KEY in your environment"
+            )
+
+        if not opts.api_secret:
+            raise ValueError(
+                "api_secret is required, or add LIVEKIT_API_SECRET in your environment"
+            )
+
         self._opts = opts
         self._loop = loop or asyncio.get_event_loop()
+
         self._id = "unregistered"
-        self._session = None
-        self._closed = False
+        self._closed, self._draining, self._connecting = True, False, False
         self._tasks = set()
-        self._draining = False
         self._pending_assignments: dict[str, asyncio.Future[agent.JobAssignment]] = {}
         self._processes = dict[str, tuple[ipc.JobProcess, ActiveJob]]()
-        self._close_future = asyncio.Future(loop=self._loop)
+        self._close_future: asyncio.Future | None = None
 
-        self._chan = aio.Chan[agent.WorkerMessage](32, loop=self._loop)
-        # We use the same event loop as the worker (so the health checks are more accurate)
+        self._msg_chan = aio.Chan[agent.WorkerMessage](128, loop=self._loop)
+
+        # use the same event loop as the main worker task
+        #  -> more accurate health checks
         self._http_server = http_server.HttpServer(
             opts.host, opts.port, loop=self._loop
         )
+        self._session: aiohttp.ClientSession | None = None
+        self._api: api.LiveKitAPI | None = None
 
     async def run(self):
-        logger.info("starting worker", extra={"version": __version__})
+        if not self._closed:
+            raise Exception("worker is already running")
 
-        if not self._opts.ws_url:
-            raise ValueError("ws_url is required, or set LIVEKIT_URL env var")
-
-        if not self._opts.api_key:
-            raise ValueError("api_key is required, or set LIVEKIT_API_KEY env var")
-
-        if not self._opts.api_secret:
-            raise ValueError(
-                "api_secret is required, or set LIVEKIT_API_SECRET env var"
-            )
+        logger.info("starting worker", extra={"version": __version__})
 
+        # this LiveKit API object is only really useful in standard workers
+        self._api = api.LiveKitAPI(
+            self._opts.ws_url, self._opts.api_key, self._opts.api_secret
+        )
         self._session = aiohttp.ClientSession()
+        self._closed = False
+        self._close_future = asyncio.Future(loop=self._loop)
 
-        async def _worker_ws():
-            assert self._session is not None
-
-            retry_count = 0
-            while not self._closed:
-                try:
-                    join_jwt = (
-                        api.AccessToken(self._opts.api_key, self._opts.api_secret)
-                        .with_grants(api.VideoGrants(agent=True))
-                        .to_jwt()
-                    )
-
-                    headers = {"Authorization": f"Bearer {join_jwt}"}
-
-                    parse = urlparse(self._opts.ws_url)
-                    scheme = parse.scheme
-                    if scheme.startswith("http"):
-                        scheme = scheme.replace("http", "ws")
-                    agent_url = (
-                        f"{scheme}://{parse.netloc}/{parse.path.rstrip('/')}/agent"
-                    )
-
-                    ws = await self._session.ws_connect(agent_url, headers=headers)
-                    retry_count = 0
-
-                    await self._run_ws(ws)
-                except Exception as e:
-                    if self._closed:
-                        break
-
-                    if retry_count >= self._opts.max_retry:
-                        raise Exception(
-                            f"failed to connect to livekit-server after {retry_count} attempts: {e}"
-                        )
-
-                    retry_delay = min(retry_count * 2, 10)
-                    retry_count += 1
-
-                    logger.warning(
-                        f"failed to connect to livekit-server, retrying in {retry_delay}s: {e}",
-                    )
-                    await asyncio.sleep(retry_delay)
-
-        async def _http_server():
-            await self._http_server.run()
-
-        await asyncio.gather(_worker_ws(), _http_server())
-        self._close_future.set_result(None)
+        try:
+            await asyncio.gather(self._worker_task(), self._http_server.run())
+        finally:
+            self._close_future.set_result(None)
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def active_jobs(self) -> list[ActiveJob]:
         return [active_job for (_, active_job) in self._processes.values()]
 
     async def drain(self, timeout: int | None = None) -> None:
+        """
+        When timeout isn't None, it will raise asyncio.TimeoutError if the processes didn't finish
+        in time.
+        """
         if self._draining:
             return
 
         logger.info("draining worker", extra={"id": self.id, "timeout": timeout})
         self._draining = True
 
         # exit the queue
-        update = agent.UpdateWorkerStatus(
-            status=(agent.WorkerStatus.WS_FULL),
+        update_worker = agent.WorkerMessage(
+            update_worker=agent.UpdateWorkerStatus(
+                status=(agent.WorkerStatus.WS_FULL),
+            )
         )
-        msg = agent.WorkerMessage(update_worker=update)
-        try:
-            self._chan.send_nowait(msg)
-        except aio.ChanClosed:
-            return
+        await self._queue_msg(update_worker)
 
-        # wait for all jobs to finish with a final timeout
+        # wait for all jobs to finish
         async def _join_jobs():
             for proc, _ in self._processes.values():
                 await proc.join()
 
         if timeout:
-            with contextlib.suppress(asyncio.TimeoutError):
-                await asyncio.wait_for(_join_jobs(), timeout)
+            # this could raise asyncio.TimeoutError
+            await asyncio.wait_for(_join_jobs(), timeout)
         else:
             await _join_jobs()
 
+    async def simulate_job(
+        self, room: str, participant_identity: str | None = None
+    ) -> None:
+        assert self._api is not None
+
+        room_obj = await self._api.room.create_room(api.CreateRoomRequest(name=room))
+        participant = None
+        if participant_identity:
+            participant = await self._api.room.get_participant(
+                api.RoomParticipantIdentity(room=room, identity=participant_identity)
+            )
+
+        msg = agent.WorkerMessage()
+        msg.simulate_job.room.CopyFrom(room_obj)
+        if participant:
+            msg.simulate_job.participant.CopyFrom(participant)
+
+        await self._queue_msg(msg)
+
     async def aclose(self) -> None:
         if self._closed:
+            if self._close_future is not None:
+                await self._close_future
             return
 
         logger.info("shutting down worker", extra={"id": self.id})
 
+        assert self._close_future is not None
+        assert self._session is not None
+        assert self._api is not None
+
+        self._closed = True
+
         # shutdown processes before closing the connection to the lkserver
         close_co = []
         for proc, _ in self._processes.values():
             close_co.append(proc.aclose())
 
         await asyncio.gather(*close_co, return_exceptions=True)
 
-        await self._http_server.aclose()
-        assert self._session is not None
         await self._session.close()
+        await self._http_server.aclose()
+        await self._api.aclose()
+        await asyncio.sleep(0.25)  # see https://github.com/aio-libs/aiohttp/issues/1925
+
+        self._msg_chan.close()
 
-        self._closed = True
-        self._chan.close()
         await self._close_future
 
+    async def _queue_msg(self, msg: agent.WorkerMessage) -> None:
+        """_queue_msg raises aio.ChanClosed when the worker is closing/closed"""
+        if self._connecting:
+            which = msg.WhichOneof("message")
+            if which == "update_worker" and not msg.update_worker.metadata:
+                return
+            elif which == "ping":
+                return
+
+        await self._msg_chan.send(msg)
+
+    async def _worker_task(self) -> None:
+        assert self._session is not None
+
+        retry_count = 0
+        while not self._closed:
+            try:
+                self._connecting = True
+                join_jwt = (
+                    api.AccessToken(self._opts.api_key, self._opts.api_secret)
+                    .with_grants(api.VideoGrants(agent=True))
+                    .to_jwt()
+                )
+
+                headers = {"Authorization": f"Bearer {join_jwt}"}
+
+                parse = urlparse(self._opts.ws_url)
+                scheme = parse.scheme
+                if scheme.startswith("http"):
+                    scheme = scheme.replace("http", "ws")
+
+                agent_url = f"{scheme}://{parse.netloc}/{parse.path.rstrip('/')}/agent"
+
+                ws = await self._session.ws_connect(
+                    agent_url, headers=headers, autoping=True
+                )
+
+                retry_count = 0
+
+                # do worker registration
+                req = agent.WorkerMessage()
+                req.register.type = self._opts.worker_type
+                req.register.allowed_permissions.CopyFrom(
+                    models.ParticipantPermission(
+                        can_publish=self._opts.permissions.can_publish,
+                        can_subscribe=self._opts.permissions.can_subscribe,
+                        can_publish_data=self._opts.permissions.can_publish_data,
+                        can_update_metadata=self._opts.permissions.can_update_metadata,
+                        can_publish_sources=self._opts.permissions.can_publish_sources,
+                        hidden=self._opts.permissions.hidden,
+                        agent=True,
+                    )
+                )
+                req.register.namespace = self._opts.namespace
+                req.register.version = __version__
+                await ws.send_bytes(req.SerializeToString())
+
+                # wait for the register response before running this connection
+                first_msg_b = await ws.receive_bytes()
+                msg = agent.ServerMessage()
+                msg.ParseFromString(first_msg_b)
+
+                if not msg.HasField("register"):
+                    raise Exception("expected register response as first message")
+
+                self._handle_register(msg.register)
+                self._connecting = False
+
+                await self._run_ws(ws)
+            except Exception as e:
+                if self._closed:
+                    break
+
+                if retry_count >= self._opts.max_retry:
+                    raise Exception(
+                        f"failed to connect to livekit after {retry_count} attempts: {e}"
+                    )
+
+                retry_delay = min(retry_count * 2, 10)
+                retry_count += 1
+
+                logger.warning(
+                    f"failed to connect to livekit, retrying in {retry_delay}s: {e}",
+                )
+                await asyncio.sleep(retry_delay)
+
     async def _run_ws(self, ws: aiohttp.ClientWebSocketResponse):
         closing_ws = False
 
-        # register the worker
-        req = agent.WorkerMessage()
-        req.register.type = self._opts.worker_type
-        req.register.allowed_permissions.CopyFrom(
-            models.ParticipantPermission(
-                can_publish=self._opts.permissions.can_publish,
-                can_subscribe=self._opts.permissions.can_subscribe,
-                can_publish_data=self._opts.permissions.can_publish_data,
-                can_update_metadata=self._opts.permissions.can_update_metadata,
-                hidden=self._opts.permissions.hidden,
-                agent=True,
-            )
-        )
-        req.register.namespace = self._opts.namespace
-        req.register.version = __version__
-        await self._chan.send(req)
-
-        async def load_monitor_task():
+        async def _load_task():
+            """periodically check load and update worker status"""
             interval = aio.interval(consts.LOAD_INTERVAL)
-            registered = True
+            current_status = agent.WorkerStatus.WS_AVAILABLE
             while True:
                 await interval.tick()
-                load = self._opts.load_fnc()
-                is_full = load >= self._opts.load_threshold
-                should_register = not is_full and not self._draining
 
-                update = agent.UpdateWorkerStatus(
-                    load=load,
-                    status=(
-                        agent.WorkerStatus.WS_FULL
-                        if is_full
-                        else agent.WorkerStatus.WS_AVAILABLE
-                    ),
+                old_status = current_status
+                current_load = self._opts.load_fnc()
+                is_full = current_load >= self._opts.load_threshold
+                currently_available = not is_full and not self._draining
+
+                current_status = (
+                    agent.WorkerStatus.WS_AVAILABLE
+                    if currently_available
+                    else agent.WorkerStatus.WS_FULL
                 )
 
-                if should_register != registered:
-                    registered = should_register
+                update = agent.UpdateWorkerStatus(
+                    load=current_load,
+                    status=current_status,
+                )
 
-                    extra = {"load": load, "threshold": self._opts.load_threshold}
+                # only log if status has changed
+                if old_status != current_status and not self._draining:
+                    extra = {
+                        "load": current_load,
+                        "threshold": self._opts.load_threshold,
+                    }
                     if is_full:
                         logger.info(
                             "worker is at full capacity, marking as unavailable",
                             extra=extra,
                         )
                     else:
                         logger.info(
                             "worker is below capacity, marking as available",
                             extra=extra,
                         )
 
                 msg = agent.WorkerMessage(update_worker=update)
-                try:
-                    self._chan.send_nowait(msg)
-                except aio.ChanClosed:
-                    return
+                with contextlib.suppress(aio.ChanClosed):
+                    await self._queue_msg(msg)
 
-        async def send_task():
+        async def _send_task():
             nonlocal closing_ws
             while True:
                 try:
-                    msg = await self._chan.recv()
+                    msg = await self._msg_chan.recv()
                     await ws.send_bytes(msg.SerializeToString())
                 except aio.ChanClosed:
                     closing_ws = True
                     return
 
-        async def recv_task():
+        async def _recv_task():
             nonlocal closing_ws
             while True:
                 msg = await ws.receive()
                 if msg.type in (
                     aiohttp.WSMsgType.CLOSE,
                     aiohttp.WSMsgType.CLOSED,
                     aiohttp.WSMsgType.CLOSING,
@@ -311,38 +393,33 @@
                     logger.warning("unexpected message type: %s", msg.type)
                     continue
 
                 data = msg.data
                 msg = agent.ServerMessage()
                 msg.ParseFromString(data)
                 which = msg.WhichOneof("message")
-                if which == "register":
-                    self._handle_register(
-                        msg.register
-                    )  # we assume this is the first message we receive
-                elif which == "availability":
+                if which == "availability":
                     self._handle_availability(msg.availability)
                 elif which == "assignment":
                     self._handle_assignment(msg.assignment)
 
-        await asyncio.gather(send_task(), recv_task(), load_monitor_task())
+        await asyncio.gather(_send_task(), _recv_task(), _load_task())
 
-    def _reload_jobs(self, jobs: list[ActiveJob]):
+    def _reload_jobs(self, jobs: list[ActiveJob]) -> None:
         for aj in jobs:
             logger.info("reloading job", extra={"job": aj.job})
 
-            # reloading jobs doesn't work on third-party workers
-            # so it is ok to use the ws_url from the local worker
-            # (also create a token with the worker api key)
+            # reloading jobs isn't supported on third-party workers, using ws_url of the local worker
+            # is OK
             url = self._opts.ws_url
 
             jwt = (
                 api.AccessToken(self._opts.api_key, self._opts.api_secret)
                 .with_grants(
-                    api.VideoGrants(agent=True, room=aj.job.room.name, room_join=True)
+                    api.VideoGrants(agent=True, room_join=True, room=aj.job.room.name)
                 )
                 .with_name(aj.accept_data.name)
                 .with_metadata(aj.accept_data.metadata)
                 .with_identity(aj.accept_data.identity)
                 .to_jwt()
             )
 
@@ -371,101 +448,98 @@
 
     def _handle_register(self, reg: agent.RegisterWorkerResponse):
         self._id = reg.worker_id
         logger.info(
             "registered worker",
             extra={"id": reg.worker_id, "server_info": reg.server_info},
         )
+        self.emit("worker_registered", reg.worker_id, reg.server_info)
 
     def _handle_availability(self, msg: agent.AvailabilityRequest):
+        task = self._loop.create_task(self._answer_availability(msg))
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.discard)
+
+    async def _answer_availability(self, msg: agent.AvailabilityRequest):
+        """Ask the user if they want to accept this job and forward the answer to the server.
+        If we get the job assigned, we start a new process."""
+
         answer_tx, answer_rx = aio.channel(1)  # wait for the user res
         req = JobRequest(msg.job, answer_tx)
 
-        async def _wait_response():
-            async def _user_cb():
-                try:
-                    await self._opts.request_fnc(req)
-                except Exception:
-                    logger.exception(
-                        f"user request handler for job {req.id} failed",
-                        extra={"req": req},
-                    )
+        async def _user_cb():
+            try:
+                await self._opts.request_fnc(req)
+            except Exception:
+                logger.exception(
+                    f"user request handler for job {req.id} failed",
+                    extra={"req": req},
+                )
 
-                if not req.answered:
-                    logger.warning(
-                        f"no answer for job {req.id}, automatically rejecting the job",
-                        extra={"req": req},
-                    )
-                    await _send_ignore_err(
-                        self._chan,
-                        agent.WorkerMessage(
-                            availability=agent.AvailabilityResponse(available=False)
-                        ),
+            if not req.answered:
+                logger.warning(
+                    f"no answer for job {req.id}, automatically rejecting the job",
+                    extra={"req": req},
+                )
+
+                await self._queue_msg(
+                    agent.WorkerMessage(
+                        availability=agent.AvailabilityResponse(available=False)
                     )
+                )
 
-            user_task = self._loop.create_task(_user_cb())
+        # ask the user if they want to accept the job
+        user_task = self._loop.create_task(_user_cb())
 
-            av: AvailRes = await answer_rx.recv()  # wait for user answer
-            msg = agent.WorkerMessage()
-            msg.availability.job_id = req.id
-            msg.availability.available = av.avail
+        av: AvailRes = await answer_rx.recv()
+        resp = agent.WorkerMessage()
+        resp.availability.job_id = req.id
+        resp.availability.available = av.avail
 
-            if not av.avail:
-                await _send_ignore_err(self._chan, msg)
-                return
+        if not av.avail:
+            await self._queue_msg(resp)  # job rejected, early return
+            return
 
-            assert av.data is not None
-            assert av.assignment_tx is not None
-            msg.availability.participant_identity = av.data.identity
-            msg.availability.participant_name = av.data.name
-            msg.availability.participant_metadata = av.data.metadata
+        assert av.data is not None
+        assert av.assignment_tx is not None
 
-            wait_assignment = asyncio.Future[agent.JobAssignment]()
-            self._pending_assignments[req.id] = wait_assignment
+        resp.availability.participant_identity = av.data.identity
+        resp.availability.participant_name = av.data.name
+        resp.availability.participant_metadata = av.data.metadata
 
-            await _send_ignore_err(self._chan, msg)
+        wait_assignment = asyncio.Future[agent.JobAssignment]()
+        self._pending_assignments[req.id] = wait_assignment
 
-            # wait for server assignment
-            try:
-                await asyncio.wait_for(wait_assignment, consts.ASSIGNMENT_TIMEOUT)
-                await av.assignment_tx.send(None)
-            except asyncio.TimeoutError as e:
-                logger.warning(
-                    f"assignment for job {req.id} timed out",
-                    extra={"req": req},
-                )
-                await av.assignment_tx.send(e)
-                return
-            finally:
-                await user_task
+        await self._queue_msg(resp)
 
-            asgn = wait_assignment.result()
-            url = asgn.url
+        # the job was accepted by the user, wait for the server assignment
+        try:
+            await asyncio.wait_for(wait_assignment, consts.ASSIGNMENT_TIMEOUT)
+            await av.assignment_tx.send(None)
+        except asyncio.TimeoutError as e:
+            logger.warning(
+                f"assignment for job {req.id} timed out",
+                extra={"req": req},
+            )
+            await av.assignment_tx.send(e)
+            return
+        finally:
+            await user_task  # make sure the user task is done
 
-            if not url:
-                url = self._opts.ws_url
+        asgn = wait_assignment.result()
+        url = asgn.url
 
-            self._start_process(asgn.job, url, asgn.token, av.data)
+        if not url:
+            url = self._opts.ws_url
 
-        task = self._loop.create_task(_wait_response())
-        self._tasks.add(task)
-        task.add_done_callback(self._tasks.discard)
+        self._start_process(asgn.job, url, asgn.token, av.data)
 
     def _handle_assignment(self, assignment: agent.JobAssignment):
         job = assignment.job
         if job.id in self._pending_assignments:
             fut = self._pending_assignments.pop(job.id)
             fut.set_result(assignment)
         else:
             logger.warning(
                 f"received assignment for unknown job {job.id}",
                 extra={"job": job},
             )
-
-
-async def _send_ignore_err(
-    ch: aio.ChanSender[agent.WorkerMessage], msg: agent.WorkerMessage
-):
-    # Used when we don't care about the result of sending
-    # e.g. when closing the worker, we close the channel.
-    with contextlib.suppress(aio.ChanClosed):
-        await ch.send(msg)
```

### Comparing `livekit_agents-0.6.dev1/livekit_agents.egg-info/PKG-INFO` & `livekit_agents-0.7.dev0/livekit_agents.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.6.dev1
+Version: 0.7.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.6.dev1/livekit_agents.egg-info/SOURCES.txt` & `livekit_agents-0.7.dev0/livekit_agents.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,32 @@
 livekit/agents/llm/__init__.py
 livekit/agents/llm/function_context.py
 livekit/agents/llm/llm.py
 livekit/agents/stt/__init__.py
 livekit/agents/stt/stream_adapter.py
 livekit/agents/stt/stt.py
 livekit/agents/tokenize/__init__.py
-livekit/agents/tokenize/sentence_tokenizer.py
+livekit/agents/tokenize/_basic_hyphenator.py
+livekit/agents/tokenize/_basic_sent.py
+livekit/agents/tokenize/_basic_word.py
+livekit/agents/tokenize/basic.py
+livekit/agents/tokenize/token_stream.py
+livekit/agents/tokenize/tokenizer.py
+livekit/agents/transcription/__init__.py
+livekit/agents/transcription/_utils.py
+livekit/agents/transcription/stt_forwarder.py
+livekit/agents/transcription/tts_forwarder.py
 livekit/agents/tts/__init__.py
 livekit/agents/tts/stream_adapter.py
 livekit/agents/tts/tts.py
 livekit/agents/utils/__init__.py
+livekit/agents/utils/_noop.py
 livekit/agents/utils/event_emitter.py
 livekit/agents/utils/exp_filter.py
+livekit/agents/utils/http_context.py
 livekit/agents/utils/misc.py
 livekit/agents/utils/moving_average.py
 livekit/agents/voice_assistant/__init__.py
 livekit/agents/voice_assistant/assistant.py
 livekit/agents/voice_assistant/plotter.py
 livekit_agents.egg-info/PKG-INFO
 livekit_agents.egg-info/SOURCES.txt
```

### Comparing `livekit_agents-0.6.dev1/setup.py` & `livekit_agents-0.7.dev0/setup.py`

 * *Files identical despite different names*

