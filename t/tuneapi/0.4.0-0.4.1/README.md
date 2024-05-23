# Comparing `tmp/tuneapi-0.4.0.tar.gz` & `tmp/tuneapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.4.0.tar", max compression
+gzip compressed data, was "tuneapi-0.4.1.tar", max compression
```

## Comparing `tuneapi-0.4.0.tar` & `tuneapi-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.0/LICENSE
--rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.0/README.md
--rw-r--r--   0        0        0      769 2024-05-13 05:24:53.684666 tuneapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-13 05:24:58.687284 tuneapi-0.4.0/tuneapi/__init__.py
--rw-r--r--   0        0        0      351 2024-05-12 11:13:29.482846 tuneapi-0.4.0/tuneapi/__main__.py
--rw-r--r--   0        0        0     6012 2024-05-13 05:29:39.964606 tuneapi-0.4.0/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6965 2024-05-10 05:19:42.218444 tuneapi-0.4.0/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     5009 2024-05-12 10:18:59.196318 tuneapi-0.4.0/tuneapi/apis/model_gemini.py
--rw-r--r--   0        0        0     3159 2024-05-12 10:20:04.649037 tuneapi-0.4.0/tuneapi/apis/model_groq.py
--rw-r--r--   0        0        0     3177 2024-04-18 21:08:27.197387 tuneapi-0.4.0/tuneapi/apis/model_mistral.py
--rw-r--r--   0        0        0     6328 2024-04-26 00:29:23.039606 tuneapi-0.4.0/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5822 2024-04-22 20:41:11.558482 tuneapi-0.4.0/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0     3714 2024-04-23 01:23:26.207221 tuneapi-0.4.0/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-04-25 04:12:26.606262 tuneapi-0.4.0/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    15414 2024-04-24 21:00:11.105695 tuneapi-0.4.0/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1153 2024-05-13 05:29:07.982518 tuneapi-0.4.0/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.0/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.0/tuneapi/utils/fs.py
--rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.0/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.0/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.0/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.0/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.0/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.0/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.0/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.0/tuneapi/utils/subway.py
--rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.0/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tuneapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 08:29:50.671125 tuneapi-0.4.1/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-13 05:27:01.434096 tuneapi-0.4.1/README.md
+-rw-r--r--   0        0        0      769 2024-05-23 17:10:07.027196 tuneapi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-23 17:10:01.975687 tuneapi-0.4.1/tuneapi/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-21 04:32:29.030680 tuneapi-0.4.1/tuneapi/__main__.py
+-rw-r--r--   0        0        0     6012 2024-05-21 06:57:23.060317 tuneapi-0.4.1/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     8597 2024-05-23 09:49:53.188434 tuneapi-0.4.1/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8131 2024-05-23 12:07:04.181995 tuneapi-0.4.1/tuneapi/apis/model_gemini.py
+-rw-r--r--   0        0        0     5897 2024-05-23 09:48:23.978502 tuneapi-0.4.1/tuneapi/apis/model_groq.py
+-rw-r--r--   0        0        0     6065 2024-05-23 09:48:52.204641 tuneapi-0.4.1/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     7729 2024-05-23 09:49:19.313038 tuneapi-0.4.1/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     6278 2024-05-23 09:49:47.799288 tuneapi-0.4.1/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0     3714 2024-05-21 06:57:20.143110 tuneapi-0.4.1/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      220 2024-05-23 09:12:22.307150 tuneapi-0.4.1/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    17546 2024-05-23 12:37:01.286725 tuneapi-0.4.1/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1247 2024-05-21 04:49:29.146672 tuneapi-0.4.1/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0     9846 2024-05-21 05:00:43.950665 tuneapi-0.4.1/tuneapi/utils/code.py
+-rw-r--r--   0        0        0      345 2024-05-12 08:34:03.731467 tuneapi-0.4.1/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2987 2024-05-12 08:34:17.889266 tuneapi-0.4.1/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0     1024 2024-05-13 05:28:35.812363 tuneapi-0.4.1/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33527 2024-05-12 08:34:20.152416 tuneapi-0.4.1/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3778 2024-05-12 08:34:28.068601 tuneapi-0.4.1/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2131 2024-05-12 08:34:30.772098 tuneapi-0.4.1/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4883 2024-05-12 08:34:35.753162 tuneapi-0.4.1/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0     1220 2024-05-12 08:34:38.734730 tuneapi-0.4.1/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2496 2024-05-12 08:34:41.922150 tuneapi-0.4.1/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5838 2024-05-12 08:34:44.657582 tuneapi-0.4.1/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0     1430 2024-05-13 05:28:59.510065 tuneapi-0.4.1/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 tuneapi-0.4.1/PKG-INFO
```

### Comparing `tuneapi-0.4.0/LICENSE` & `tuneapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/pyproject.toml` & `tuneapi-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.4.0"
+version = "0.4.1"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.4.0/tuneapi/apis/__init__.py` & `tuneapi-0.4.1/tuneapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/apis/model_anthropic.py` & `tuneapi-0.4.1/tuneapi/apis/model_gemini.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,215 +1,249 @@
 # Copyright © 2024- Frello Technology Private Limited
+# https://ai.google.dev/gemini-api/docs/function-calling
 
 import json
 import requests
-from typing import Optional, Dict, Any, Tuple, List
+from typing import Optional, Any
 
-from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
-from tuneapi.types import Thread, human, Message
+import tuneapi.utils as tu
+import tuneapi.types as tt
 
 
-class Anthropic:
+class Gemini:
     def __init__(
         self,
-        model: Optional[str] = "claude-3-haiku-20240307",
-        base_url: str = "https://api.anthropic.com/v1/messages",
+        id: Optional[str] = "gemini-1.5-pro-latest",
+        base_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{id}:{rpc}",
     ):
-        self.anthropic_model = model
+        self._gemeni_model_id = id
         self.base_url = base_url
-        self.anthropic_api_token = ENV.ANTHROPIC_TOKEN("")
+        self.gemini_token = tu.ENV.GEMINI_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
-        self.anthropic_api_token = token
+        self.gemini_token = token
 
-    def tool_to_claude_xml(self, tool):
-        tool_signature = ""
-        if len(tool["parameters"]) > 0:
-            for name, p in tool["parameters"]["properties"].items():
-                param = f"""<parameter>
-                <name> {name} </name>
-                <type> {p['type']} </type>
-                <description> {p['description']} </description>
-                """
-                if name in tool["parameters"]["required"]:
-                    param += "<required> true </required>\n"
-                param += "</parameter>"
-                tool_signature += param + "\n"
-        tool_signature = tool_signature.strip()
-
-        constructed_prompt = (
-            "<tool_description>\n"
-            f"<tool_name> {tool['name']} </tool_name>\n"
-            "<description>\n"
-            f"{tool['description']}\n"
-            "</description>\n"
-            "<parameters>\n"
-            f"{tool_signature}\n"
-            "</parameters>\n"
-            "</tool_description>"
-        )
-        return constructed_prompt
-
-    def _process_input(
-        self, chats, tools: Optional[List] = None, token: Optional[str] = None
-    ):
-        if not token and not self.anthropic_api_token:  # type: ignore
+    def _process_input(self, chats, token: Optional[str] = None):
+        if not token and not self.gemini_token:  # type: ignore
             raise Exception(
-                "Please set ANTHROPIC_TOKEN environment variable or pass through function"
+                "Gemini API key not found. Please set GEMINI_TOKEN environment variable or pass through function"
             )
-        token = token or self.anthropic_api_token
-        if isinstance(chats, Thread):
-            messages = chats.to_dict()["chats"]
+        if isinstance(chats, tt.Thread):
+            thread = chats
         elif isinstance(chats, str):
-            messages = Thread(human(chats)).to_dict()["chats"]
+            thread = tt.Thread(tt.human(chats))
         else:
-            messages = chats
+            raise Exception("Invalid input")
 
-        # create the anthropic style data
         system = ""
-        claude_messages = []
-        if messages[0]["role"] == Message.SYSTEM:
-            system_message = messages.pop(0)
-            system = system_message["content"]
-        for m in messages:
-            # correct the role
-            role = m["role"]
-            if m["role"] == Message.HUMAN:
-                role = "user"
-            elif m["role"] == Message.GPT:
-                role = "assistant"
-
-            # correct content
-            content = m["content"]
-            if type(content) == str:
-                content = [{"type": "text", "text": content.strip()}]
-            claude_messages.append(
-                {
-                    "role": role,
-                    "content": content,
-                }
-            )
+        if thread.chats[0].role == tt.Message.SYSTEM:
+            system = thread.chats[0].value
 
-        if tools:
-            tool_use_system_prompt = (
-                "In this environment you have access to a set of tools you can use to answer the user's question.\n"
-                "\n"
-                "You may call them like this:\n"
-                "<function_calls>\n"
-                "<invoke>\n"
-                "<tool_name>$TOOL_NAME</tool_name>\n"
-                "<parameters>\n"
-                "<$PARAMETER_NAME>$PARAMETER_VALUE</$PARAMETER_NAME>\n"
-                "...\n"
-                "</parameters>\n"
-                "</invoke>\n"
-                "</function_calls>\n"
-                "\n"
-                "Here are the tools available:\n"
-                "<tools>\n"
-                + "\n".join([self.tool_to_claude_xml(tool) for tool in tools])
-                + "\n</tools>"
-            )
-            system += "\n\n" + tool_use_system_prompt
-        system = system.strip()
+        messages = []
+        prev_fn_name = ""
+        for m in thread.chats[int(system != "") :]:
+            if m.role == tt.Message.HUMAN:
+                messages.append(
+                    {
+                        "role": "user",
+                        "parts": [{"text": m.value}],
+                    }
+                )
+            elif m.role == tt.Message.GPT:
+                messages.append(
+                    {
+                        "role": "model",
+                        "parts": [{"text": m.value}],
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_CALL:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                prev_fn_name = _m["name"]
+                messages.append(
+                    {
+                        "role": "model",
+                        "parts": [
+                            {
+                                "functionCall": {
+                                    "name": _m["name"],
+                                    "args": _m["arguments"],
+                                }
+                            }
+                        ],
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_RESP:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                messages.append(
+                    {
+                        "role": "function",
+                        "parts": [
+                            {
+                                "functionResponse": {
+                                    "name": prev_fn_name,
+                                    "response": {
+                                        "name": prev_fn_name,
+                                        "content": _m,
+                                    },
+                                }
+                            }
+                        ],
+                    }
+                )
+            else:
+                raise Exception(f"Unknown role: {m.role}")
+
+        # create headers
+        headers = self._process_header()
+        params = {"key": self.gemini_token}
+        return headers, system.strip(), messages, params
 
-        headers = {
-            "x-api-key": token,
+    def _process_header(self):
+        return {
             "Content-Type": "application/json",
-            "anthropic-version": "2023-06-01",
         }
-        return headers, system, claude_messages
 
     def chat(
         self,
-        chats: Thread | str,
-        tools: Optional[List] = None,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
+        timeout=None,
+        raw: bool = False,
         **kwargs,
-    ):
+    ) -> Any:
         output = ""
-        for i in self.stream_chat(
+        for x in self.stream_chat(
             chats=chats,
-            tools=tools,
             model=model,
             max_tokens=max_tokens,
             temperature=temperature,
             token=token,
+            timeout=timeout,
+            raw=raw,
             **kwargs,
         ):
-            output += i
+            if isinstance(x, dict):
+                output = x
+            else:
+                output += x
         return output
 
     def stream_chat(
         self,
-        chats: Thread | str,
-        tools: Optional[List] = None,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
-        timeout=(5, 30),
+        timeout=(5, 60),
         raw: bool = False,
+        debug: bool = False,
         **kwargs,
-    ) -> Any:
-        headers, system, claude_messages = self._process_input(
-            chats=chats,
-            tools=tools,
-            token=token,
-        )
+    ):
+        tools = []
+        if isinstance(chats, tt.Thread):
+            tools = [x.to_dict() for x in chats.tools]
+        headers, system, messages, params = self._process_input(chats, token)
         data = {
-            "model": model or self.anthropic_model,
-            "max_tokens": max_tokens,
-            "messages": claude_messages,
-            "temperature": temperature,
-            "system": system,
-            "stream": True,
-            **kwargs,
+            "systemInstruction": {
+                "parts": [{"text": system}],
+            },
+            "contents": messages,
+            "generationConfig": {
+                "temperature": temperature,
+                "topK": 0,
+                "topP": 0.95,
+                "maxOutputTokens": max_tokens,
+                "stopSequences": [],
+            },
+            "safetySettings": [
+                {
+                    "category": "HARM_CATEGORY_HARASSMENT",
+                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
+                },
+                {
+                    "category": "HARM_CATEGORY_HATE_SPEECH",
+                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
+                },
+                {
+                    "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT",
+                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
+                },
+                {
+                    "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
+                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
+                },
+            ],
         }
-        r = requests.post(
-            self.base_url,
+        if tools:
+            data["tool_config"] = {
+                "function_calling_config": {
+                    "mode": "ANY",
+                }
+            }
+            data["tools"] = [{"function_declarations": tools}]
+        data.update(kwargs)
+
+        if debug:
+            fp = "sample_gemini.json"
+            print("Saving at path " + fp)
+            tu.to_json(data, fp=fp)
+
+        response = requests.post(
+            self.base_url.format(
+                id=model or self._gemeni_model_id,
+                rpc="streamGenerateContent",
+            ),
             headers=headers,
+            params=params,
             json=data,
+            stream=True,
             timeout=timeout,
         )
         try:
-            r.raise_for_status()
+            response.raise_for_status()
         except Exception as e:
-            print(r.text)
+            print(response.text)
             raise e
 
-        for line in r.iter_lines():
-            line = line.decode().strip()
-            if not "data:" in line or not line:
-                continue
-
-            # create openai style raw response
-            if raw:
-                try:
-                    resp = json.loads(line.replace("data:", "").strip())
-                    if "delta" in resp:
-                        yield (
-                            "data: "
-                            + to_json(
-                                {
-                                    "choices": [
-                                        {"delta": {"content": resp["delta"]["text"]}}
-                                    ]
-                                },
-                                tight=True,
-                            )
-                        ).encode() + b"\r\n"
-                except:
-                    yield line.encode() + b"\r\n"
+        block_lines = ""
+        done = False
+        for lno, line in enumerate(response.iter_lines()):
+            line = line.decode("utf-8")
+            # print(f"[{lno:03d}] {line}")
+
+            # get the clean line for block
+            if line == ("[{"):  # first line
+                line = line[1:]
+            elif line == "," or line == "]":  # intermediate or last line
                 continue
+            block_lines += line
 
-            # return token
-            try:
-                resp = json.loads(line.replace("data:", "").strip())
-                if "delta" in resp:
-                    yield resp["delta"]["text"]
-            except:
-                break
-        return
+            # is the block done?
+            if line == "{":
+                done = False
+            elif line == "}":
+                done = True
+
+            if done:
+                part_data = json.loads(block_lines)["candidates"][0]["content"][
+                    "parts"
+                ][0]
+                if "text" in part_data:
+                    if raw:
+                        yield tu.to_json(
+                            {
+                                "object": "gemini_text",
+                                "choices": [{"delta": {"content": part_data["text"]}}],
+                            },
+                            tight=True,
+                        ).encode()
+                    else:
+                        yield part_data["text"]
+                elif "functionCall" in part_data:
+                    fn_call = part_data["functionCall"]
+                    fn_call["arguments"] = fn_call.pop("args")
+                    yield fn_call
+                block_lines = ""
```

### Comparing `tuneapi-0.4.0/tuneapi/apis/model_gemini.py` & `tuneapi-0.4.1/tuneapi/apis/model_groq.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,177 @@
 # Copyright © 2024- Frello Technology Private Limited
 
 import json
 import requests
 from typing import Optional, Dict, Any, Tuple, List
 
-from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
-from tuneapi.types import Thread, human, Message
+import tuneapi.utils as tu
+import tuneapi.types as tt
 
 
-class Gemini:
+class Groq:
     def __init__(
         self,
-        id: Optional[str] = "gemini-1.5-pro-latest",
-        base_url: str = "https://generativelanguage.googleapis.com/v1beta/models/{id}:{rpc}",
+        id: Optional[str] = "llama3-70b-8192",
+        base_url: str = "https://api.groq.com/openai/v1/chat/completions",
     ):
-        self._gemeni_model_id = id
+        self.groq_model_id = id
         self.base_url = base_url
-        self.gemini_token = ENV.GEMINI_TOKEN("")
+        self.groq_api_token = tu.ENV.GROQ_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
-        self.gemini_token = token
+        self.groq_api_token = token
 
     def _process_input(self, chats, token: Optional[str] = None):
-        if not token and not self.gemini_token:  # type: ignore
+        if not token and not self.groq_api_token:  # type: ignore
             raise Exception(
-                "Gemini API key not found. Please set GEMINI_TOKEN environment variable or pass through function"
+                "Please set GROQ_TOKEN environment variable or pass through function"
             )
-        if isinstance(chats, Thread):
-            messages_tt = chats.to_dict()["chats"]
+        token = token or self.groq_api_token
+        if isinstance(chats, tt.Thread):
+            thread = chats
         elif isinstance(chats, str):
-            messages_tt = Thread(human(chats)).to_dict()["chats"]
+            thread = tt.Thread(tt.human(chats))
         else:
-            messages_tt = chats
+            raise Exception("Invalid input")
 
-        # create body
-        # - multiple assistants works
-        messages = []
-        for m in messages_tt:
-            messages.append(
-                {
-                    "role": m["role"],
-                    "parts": [{"text": m["content"]}],
-                }
-            )
-
-        # create headers
-        headers = self._process_header()
-        params = {"key": self.gemini_token}
-        return headers, messages, params
+        prev_tool_id = tu.get_random_string(5)
+        final_messages = []
+        for i, m in enumerate(thread.chats):
+            if m.role == tt.Message.SYSTEM:
+                final_messages.append({"role": "system", "content": m.value})
+            elif m.role == tt.Message.HUMAN:
+                final_messages.append({"role": "user", "content": m.value})
+            elif m.role == tt.Message.GPT:
+                final_messages.append(
+                    {
+                        "role": "assistant",
+                        "content": m.value.strip(),
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_CALL:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                final_messages.append(
+                    {
+                        "role": "assistant",
+                        "tool_calls": [
+                            {
+                                "type": "function",
+                                "id": prev_tool_id,
+                                "function": {
+                                    "name": _m["name"],
+                                    "arguments": tu.to_json(_m["arguments"]),
+                                },
+                            }
+                        ],
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_RESP:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                final_messages.append(
+                    {
+                        "role": "tool",
+                        "tool_call_id": prev_tool_id,
+                        "content": tu.to_json(_m, tight=True),
+                    }
+                )
+                prev_tool_id = tu.get_random_string(5)  # reset tool id
+            else:
+                raise Exception(f"Invalid message type: {m.role}")
 
-    def _process_header(self):
-        return {
+        headers = {
+            "Authorization": "Bearer " + token,
             "Content-Type": "application/json",
         }
+        return headers, final_messages
 
     def chat(
         self,
-        chats: Thread | str,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
-        timeout=None,
-        raw: bool = False,
+        timeout=(5, 30),
         **kwargs,
-    ) -> Any:
+    ) -> str | Dict[str, Any]:
         output = ""
-        for i in self.stream_chat(
+        for x in self.stream_chat(
             chats=chats,
             model=model,
             max_tokens=max_tokens,
             temperature=temperature,
             token=token,
             timeout=timeout,
-            raw=raw,
             **kwargs,
         ):
-            output += i
+            if isinstance(x, dict):
+                output = x
+            else:
+                output += x
         return output
 
     def stream_chat(
         self,
-        chats: Thread | str,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
         timeout=(5, 60),
+        debug: bool = False,
         raw: bool = False,
-        **kwargs,
     ):
-        headers, messages, params = self._process_input(chats, token)
+        tools = []
+        if isinstance(chats, tt.Thread):
+            tools = [{"type": "function", "function": x.to_dict()} for x in chats.tools]
+        headers, messages = self._process_input(chats, token)
         data = {
-            "contents": messages,
-            "generationConfig": {
-                "temperature": temperature,
-                "topK": 0,
-                "topP": 0.95,
-                "maxOutputTokens": max_tokens,
-                "stopSequences": [],
-            },
-            "safetySettings": [
-                {
-                    "category": "HARM_CATEGORY_HARASSMENT",
-                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
-                },
-                {
-                    "category": "HARM_CATEGORY_HATE_SPEECH",
-                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
-                },
-                {
-                    "category": "HARM_CATEGORY_SEXUALLY_EXPLICIT",
-                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
-                },
-                {
-                    "category": "HARM_CATEGORY_DANGEROUS_CONTENT",
-                    "threshold": "BLOCK_MEDIUM_AND_ABOVE",
-                },
-            ],
+            "temperature": temperature,
+            "messages": messages,
+            "model": model or self.groq_model_id,
+            "stream": True,
+            "max_tokens": max_tokens,
+            "tools": tools,
         }
-        data.update(kwargs)
+        if debug:
+            fp = "sample_groq.json"
+            print("Saving at path " + fp)
+            tu.to_json(data, fp=fp)
 
         response = requests.post(
-            self.base_url.format(
-                id=model or self._gemeni_model_id,
-                rpc="streamGenerateContent",
-            ),
+            self.base_url,
             headers=headers,
-            params=params,
             json=data,
             stream=True,
             timeout=timeout,
         )
         try:
             response.raise_for_status()
         except Exception as e:
             print(response.text)
             raise e
 
-        block_lines = ""
-        done = False
-        for lno, line in enumerate(response.iter_lines()):
-            line = line.decode("utf-8")
-            # print(f"[{lno:03d}] {line}")
+        fn_call = None
+        for line in response.iter_lines():
             if raw:
                 yield line
                 continue
 
-            # get the clean line for block
-            if line == ("[{"):  # first line
-                line = line[1:]
-            elif line == "," or line == "]":  # intermediate or last line
-                continue
-            block_lines += line
-
-            # is the block done?
-            if line == "{":
-                done = False
-            elif line == "}":
-                done = True
-
-            if done:
-                yield json.loads(block_lines)["candidates"][0]["content"]["parts"][0][
-                    "text"
-                ]
-                block_lines = ""
+            line = line.decode().strip()
+            if line:
+                try:
+                    x = json.loads(line.replace("data: ", ""))["choices"][0]["delta"]
+                    if "tool_calls" not in x:
+                        yield x["content"]
+                    else:
+                        y = x["tool_calls"][0]["function"]
+                        if fn_call is None:
+                            fn_call = {"name": y["name"], "arguments": y["arguments"]}
+                        else:
+                            fn_call["arguments"] += y["arguments"]
+                except:
+                    break
+        if fn_call:
+            fn_call["arguments"] = tu.from_json(fn_call["arguments"])
+            yield fn_call
+        return
```

### Comparing `tuneapi-0.4.0/tuneapi/apis/model_openai.py` & `tuneapi-0.4.1/tuneapi/apis/model_tune.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,209 +1,187 @@
 # Copyright © 2024- Frello Technology Private Limited
 
 import json
 import requests
-from typing import Optional, Dict, Any, Tuple, List
+from typing import Optional, Dict, Any
 
-from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
-from tuneapi.types import Thread, human, Message
+import tuneapi.utils as tu
+import tuneapi.types as tt
 
 
-class Openai:
+class TuneModel:
+    """Defines the model used in tune.app. See [Tune Studio](https://studio.tune.app/) for more information."""
+
     def __init__(
         self,
-        id: Optional[str] = "gpt-3.5-turbo",
-        base_url: str = "https://api.openai.com/v1/chat/completions",
+        id: Optional[str] = None,
+        base_url: str = "https://proxy.tune.app/chat/completions",
+        org_id: Optional[str] = None,
     ):
-        self._openai_model_id = id
+        self.tune_model_id = id or tu.ENV.TUNEAPI_MODEL("")
         self.base_url = base_url
-        self.openai_api_token = ENV.OPENAI_TOKEN("")
+        self.tune_api_token = tu.ENV.TUNEAPI_TOKEN("")
+        self.tune_org_id = org_id or tu.ENV.TUNEORG_ID("")
 
     def set_api_token(self, token: str) -> None:
-        self.openai_api_token = token
+        self.tune_api_token = token
+
+    def set_org_id(self, org_id: str) -> None:
+        self.tune_org_id = org_id
 
     def _process_input(self, chats, token: Optional[str] = None):
-        if not token and not self.openai_api_token:  # type: ignore
+        if not token and not self.tune_api_token:  # type: ignore
             raise Exception(
-                "OpenAI API key not found. Please set OPENAI_TOKEN environment variable or pass through function"
+                "Tune API key not found. Please set TUNEAPI_TOKEN environment variable or pass through function"
             )
-        if isinstance(chats, Thread):
-            messages = chats.to_dict()["chats"]
+        token = token or self.tune_api_token
+
+        if isinstance(chats, tt.Thread):
+            thread = chats
         elif isinstance(chats, str):
-            messages = Thread(human(chats)).to_dict()["chats"]
+            thread = tt.Thread(tt.human(chats))
         else:
-            messages = chats
-        headers = self._process_header(token)
-        return headers, messages
-
-    def _process_header(self, token: Optional[str] = None):
-        return {
-            "Authorization": "Bearer " + (token or self.openai_api_token),
+            raise Exception("Invalid input")
+
+        prev_tool_id = tu.get_random_string(5)
+        final_messages = []
+        for i, m in enumerate(thread.chats):
+            if m.role == tt.Message.SYSTEM:
+                final_messages.append({"role": "system", "content": m.value})
+            elif m.role == tt.Message.HUMAN:
+                final_messages.append({"role": "user", "content": m.value})
+            elif m.role == tt.Message.GPT:
+                final_messages.append(
+                    {
+                        "role": "assistant",
+                        "content": m.value.strip(),
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_CALL:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                final_messages.append(
+                    {
+                        "role": "assistant",
+                        "tool_calls": [
+                            {
+                                "type": "function",
+                                "id": prev_tool_id,
+                                "function": {
+                                    "name": _m["name"],
+                                    "arguments": tu.to_json(_m["arguments"]),
+                                },
+                            }
+                        ],
+                    }
+                )
+            elif m.role == tt.Message.FUNCTION_RESP:
+                _m = tu.from_json(m.value) if isinstance(m.value, str) else m.value
+                final_messages.append(
+                    {
+                        "role": "tool",
+                        "tool_call_id": prev_tool_id,
+                        "content": tu.to_json(_m, tight=True),
+                    }
+                )
+                prev_tool_id = tu.get_random_string(5)  # reset tool id
+            else:
+                raise Exception(f"Invalid message type: {m.role}")
+
+        headers = {
+            "Authorization": token,
             "Content-Type": "application/json",
         }
+        if self.tune_org_id:
+            headers["X-Org-Id"] = self.tune_org_id
+        return headers, final_messages
 
     def chat(
         self,
-        chats: Thread | str,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
+        timeout=(5, 30),
         **kwargs,
-    ) -> Any:
+    ) -> str | Dict[str, Any]:
         output = ""
-        for i in self.stream_chat(
+        for x in self.stream_chat(
             chats=chats,
             model=model,
             max_tokens=max_tokens,
             temperature=temperature,
             token=token,
+            timeout=timeout,
             **kwargs,
         ):
-            output += i
+            if isinstance(x, dict):
+                output = x
+            else:
+                output += x
         return output
 
     def stream_chat(
         self,
-        chats: Thread | str,
+        chats: tt.Thread | str,
         model: Optional[str] = None,
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
         timeout=(5, 60),
         raw: bool = False,
+        debug: bool = False,
     ):
         headers, messages = self._process_input(chats, token)
         data = {
             "temperature": temperature,
             "messages": messages,
-            "model": model or self._openai_model_id,
+            "model": model or self.tune_model_id,
             "stream": True,
             "max_tokens": max_tokens,
         }
-        # for m in messages:
-        #     print(m)
+        if isinstance(chats, tt.Thread):
+            data["tools"] = [
+                {"type": "function", "function": x.to_dict()} for x in chats.tools
+            ]
+        if debug:
+            fp = "sample_tune.json"
+            print("Saving at path " + fp)
+            tu.to_json(data, fp=fp)
+
         response = requests.post(
             self.base_url,
             headers=headers,
             json=data,
             stream=True,
             timeout=timeout,
         )
         try:
             response.raise_for_status()
         except Exception as e:
             print(response.text)
             raise e
 
+        fn_call = None
         for line in response.iter_lines():
             if raw:
                 yield line
                 continue
 
             line = line.decode().strip()
             if line:
                 try:
-                    yield json.loads(line.replace("data: ", ""))["choices"][0]["delta"][
-                        "content"
-                    ]
+                    x = json.loads(line.replace("data: ", ""))["choices"][0]["delta"]
+                    if "tool_calls" not in x:
+                        yield x["content"]
+                    else:
+                        y = x["tool_calls"][0]["function"]
+                        if fn_call is None:
+                            fn_call = {"name": y["name"], "arguments": y["arguments"]}
+                        else:
+                            fn_call["arguments"] += y["arguments"]
                 except:
                     break
+        if fn_call:
+            fn_call["arguments"] = tu.from_json(fn_call["arguments"])
+            yield fn_call
         return
-
-    def function_call(
-        self,
-        chats: Thread | str,
-        tools: List,
-        model: Optional[str] = None,
-        max_tokens: int = 1024,
-        temperature: float = None,
-        token: Optional[str] = None,
-        timeout=(5, 60),
-    ):
-        headers, messages = self._process_input(chats, token)
-        data = {
-            "temperature": temperature,
-            "messages": messages,
-            "model": model or self._openai_model_id,
-            "tools": tools,
-            "stream": False,
-            "max_tokens": max_tokens,
-        }
-        # for m in messages:
-        #     print(m)
-        r = requests.post(
-            "https://api.openai.com/v1/chat/completions",
-            headers=headers,
-            json=data,
-            timeout=timeout,
-        )
-        try:
-            r.raise_for_status()
-        except Exception as e:
-            print(r.text)
-            raise e
-        x = r.json()["choices"][0]["message"]
-        if "tool_calls" not in x:
-            return x["content"]
-        else:
-            y = x["tool_calls"][0]["function"]
-            # print(x)
-            return {
-                "name": y["name"],
-                "arguments": from_json(y["arguments"]),
-            }
-
-    def embedding(
-        self,
-        chats: Thread | List[str] | str,
-        cum: bool = False,
-        model: str = "text-embedding-3-small",
-        token: Optional[str] = None,
-        timeout=(5, 60),
-    ):
-        text = []
-
-        headers = self._process_header(token)
-        if isinstance(chats, Thread):
-            headers, messages = self._process_input(chats, token)
-            for i, m in enumerate(messages):
-                x = f"<{m['role']}> : {m['content']}\n\n"
-                if not text:
-                    text.append(x)
-                    continue
-                if cum:
-                    # create a cumulative string from start till now
-                    x = ""
-                    for j in range(i + 1):
-                        x += f"<{messages[j]['role']}> : {messages[j]['content']}\n\n"
-                else:
-                    # attach to previous message
-                    text[-1] += x
-                text.append(x)
-        elif isinstance(chats, list) and len(chats) and isinstance(chats[0], str):
-            # this is an exception
-            text = chats
-        elif isinstance(chats, str):
-            text = [chats]
-        else:
-            raise ValueError(f"Invalid input type. Got {type(chats)}")
-
-        r = requests.post(
-            "https://api.openai.com/v1/embeddings",
-            json={
-                "input": text,
-                "model": model,
-                "encoding_format": "float",
-            },
-            headers=headers,
-            timeout=timeout,
-        )
-        try:
-            r.raise_for_status()
-        except Exception as e:
-            print(r.text)
-            raise e
-        emb = [
-            x["embedding"] for x in sorted(r.json()["data"], key=lambda x: x["index"])
-        ]
-        return emb
```

### Comparing `tuneapi-0.4.0/tuneapi/apis/threads.py` & `tuneapi-0.4.1/tuneapi/apis/threads.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/types/chats.py` & `tuneapi-0.4.1/tuneapi/types/chats.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,84 @@
 import os
 import json
 import random
 from functools import partial
 from collections.abc import Iterable
 from typing import Dict, List, Any, Tuple, Optional, Generator, Union
 
-from tuneapi.utils import to_json, get_random_string, logger
+from tuneapi.utils import to_json, get_random_string, logger, from_json
+
+
+class Tool:
+
+    class Prop:
+        def __init__(
+            self,
+            name: str,
+            description: str,
+            type: str,
+            required: bool = False,
+            items: Optional[Dict] = None,
+            enum: Optional[List[str]] = None,
+        ):
+            self.name = name
+            self.description = description
+            self.required = required
+            self.type = type
+            self.items = items
+            self.enum = enum
+
+    def __init__(
+        self,
+        name: str,
+        description: str,
+        parameters: List["Tool.Prop"],
+    ):
+        self.name = name
+        self.description = description
+        self.parameters = parameters
+
+    def __repr__(self) -> str:
+        return f"<Tool: {self.name}>"
+
+    def to_dict(self):
+        properties = {}
+        required = []
+        for x in self.parameters:
+            properties[x.name] = {
+                "type": x.type,
+                "description": x.description,
+            }
+            if x.items:
+                properties[x.name]["items"] = x.items
+            if x.enum:
+                properties[x.name]["enum"] = x.enum
+            if x.required:
+                required.append(x.name)
+
+        return {
+            "name": self.name,
+            "description": self.description,
+            "parameters": {
+                "type": "object",
+                "properties": properties,
+                "required": required,
+            },
+        }
+
+    @classmethod
+    def from_dict(cls, x):
+        parameters = []
+        for k, v in x["parameters"].get("properties", {}).items():
+            parameters.append(cls.Prop(name=k, **v))
+        return cls(
+            name=x["name"],
+            description=x["description"],
+            parameters=parameters,
+        )
 
 
 class Message:
     # names that are our standards roles
     SYSTEM = "system"
     HUMAN = "human"
     GPT = "gpt"
@@ -32,17 +101,14 @@
         "assistant": GPT,
         "machine": GPT,
         # functions
         "function_call": FUNCTION_CALL,
         "function-call": FUNCTION_CALL,
         "function_resp": FUNCTION_RESP,
         "function-resp": FUNCTION_RESP,
-        # tools
-        "tools": TOOLS,
-        "tool": TOOLS,
     }
 
     # start initialization here
     def __init__(self, value: str | float | List[Dict[str, Any]], role: str, **kwargs):
         if role not in self.KNOWN_ROLES:
             raise ValueError(f"Unknown role: {role}. Update dictionary `KNOWN_ROLES`")
         if value is None:
@@ -122,15 +188,16 @@
         )  # type: ignore
 
 
 ### Aliases
 human = partial(Message, role=Message.HUMAN)
 system = partial(Message, role=Message.SYSTEM)
 assistant = partial(Message, role=Message.GPT)
-tools = partial(Message, role=Message.TOOLS)
+function_call = partial(Message, role=Message.FUNCTION_CALL)
+function_resp = partial(Message, role=Message.FUNCTION_RESP)
 
 
 class Thread:
     """
     If the last Message is a "value".
 
     Args:
@@ -141,21 +208,23 @@
     def __init__(
         self,
         *chats: Union[List[Message], Message],
         jl: Optional[Dict[str, Any]] = None,
         model: Optional[str] = None,
         id: str = "",
         title: str = "",
+        tools: List[Tool] = [],
         **kwargs,
     ):
         self.chats = list(chats)
         self.jl = jl
         self.model = model
         self.id = id
         self.title = title
+        self.tools = tools
 
         #
         kwargs = {k: v for k, v in sorted(kwargs.items())}
         self.meta = kwargs
         self.keys = list(kwargs.keys())
         self.values = tuple(kwargs.values())
 
@@ -170,14 +239,16 @@
         x = "<Thread "
         if self.id:
             x += f"'{self.id}' "
         for k, v in self.meta.items():
             x += f"{k}={v} "
         for c in self.chats:
             x += f"\n  {c}"
+        if self.tools:
+            x += f"\n  <tools: {[x.name for x in self.tools]}>"
         x += "\n>"
         return x
 
     def __getattr__(self, __name: str) -> Any:
         if __name in self.meta:
             return self.meta[__name]
         raise AttributeError(f"Attribute {__name} not found")
@@ -192,30 +263,33 @@
             return {
                 "chats": [x.to_dict() for x in self.chats],
                 "jl": self.jl,
                 "model": self.model,
                 "meta": self.meta,
                 "title": self.title,
                 "id": self.id,
+                "tools": [x.to_dict() for x in self.tools],
             }
         return {
             "chats": [x.to_dict() for x in self.chats],
+            "tools": [x.to_dict() for x in self.tools],
         }
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "Thread":
         chats = data.get("chats", []) or data.get("conversations", [])
         if not chats:
             raise ValueError("No chats found")
         return cls(
             *[Message.from_dict(x) for x in chats],
             id=data.get("id", ""),
             jl=data.get("jl", ""),
             model=data.get("model", ""),
             title=data.get("title", ""),
+            tools=[Tool.from_dict(x) for x in data.get("tools", [])],
             **data.get("meta", {}),
         )
 
     def to_ft(
         self, id: Any = None, drop_last: bool = False
     ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         chats = self.chats if not drop_last else self.chats[:-1]
@@ -470,13 +544,12 @@
             raise ValueError(f"Folder '{folder}/train' does not exist")
         if not os.path.exists(f"{folder}/eval"):
             raise ValueError(f"Folder '{folder}/eval' does not exist")
         if not os.path.exists(f"{folder}/tune_config.json"):
             raise ValueError(f"File '{folder}/tune_config.json' does not exist")
 
         # not sure what to do with these
-        with open(f"{folder}/tune_config.json", "r") as f:
-            config = json.load(f)
+        config = from_json(f"{folder}/tune_config.json")
         return cls(
             train=ThreadsList.from_disk(f"{folder}/train"),
             eval=ThreadsList.from_disk(f"{folder}/eval"),
         )
```

### Comparing `tuneapi-0.4.0/tuneapi/utils/__init__.py` & `tuneapi-0.4.1/tuneapi/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,68 @@
 # Copyright © 2024- Frello Technology Private Limited
 # REMEMBER: nothing from outside tune should be imported in utils
 
 import os
 
-from tuneapi.utils.env import ENV
-from tuneapi.utils.logger import (
-    get_logger,
-    warning_with_fix,
-    logger,
-)
-from tuneapi.utils.serdeser import (
-    to_json,
-    from_json,
-    dict_to_structpb,
-    structpb_to_dict,
-    to_b64,
-    from_b64,
-)
-from tuneapi.utils.networking import (
-    UnAuthException,
-    DoNotRetryException,
-    exponential_backoff,
-)
-from tuneapi.utils.parallel import (
-    batched,
-    threaded_map,
-)
-from tuneapi.utils.randomness import (
-    get_random_string,
-    get_snowflake,
+from tuneapi.utils.code import (
+    func_to_vars,
+    Var,
 )
+from tuneapi.utils.env import ENV
 from tuneapi.utils.fs import (
     list_dir,
     get_files_in_folder,
     folder,
     joinp,
     load_module_from_path,
     fetch,
 )
-from tuneapi.utils.terminal import (
-    hr,
-    color,
+from tuneapi.utils.logger import (
+    get_logger,
+    warning_with_fix,
+    logger,
 )
 from tuneapi.utils.mime import (
     get_mime_type,
 )
 from tuneapi.utils.misc import (
     SimplerTimes,
     unsafe_exit,
     safe_exit,
     hashstr,
     encrypt,
     decrypt,
 )
+from tuneapi.utils.networking import (
+    UnAuthException,
+    DoNotRetryException,
+    exponential_backoff,
+)
+from tuneapi.utils.parallel import (
+    batched,
+    threaded_map,
+)
+from tuneapi.utils.randomness import (
+    get_random_string,
+    get_snowflake,
+)
+from tuneapi.utils.serdeser import (
+    to_json,
+    from_json,
+    dict_to_structpb,
+    structpb_to_dict,
+    to_b64,
+    from_b64,
+    to_pickle,
+    from_pickle,
+)
 from tuneapi.utils.subway import (
     SubwayClientError,
     SubwayServerError,
     Subway,
     get_session,
     get_subway,
 )
+from tuneapi.utils.terminal import (
+    hr,
+    color,
+)
```

### Comparing `tuneapi-0.4.0/tuneapi/utils/fs.py` & `tuneapi-0.4.1/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/logger.py` & `tuneapi-0.4.1/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/mime.py` & `tuneapi-0.4.1/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/misc.py` & `tuneapi-0.4.1/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/networking.py` & `tuneapi-0.4.1/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/parallel.py` & `tuneapi-0.4.1/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/randomness.py` & `tuneapi-0.4.1/tuneapi/utils/randomness.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/serdeser.py` & `tuneapi-0.4.1/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/subway.py` & `tuneapi-0.4.1/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/tuneapi/utils/terminal.py` & `tuneapi-0.4.1/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.4.0/PKG-INFO` & `tuneapi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: MIT
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

