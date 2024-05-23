# Comparing `tmp/imas_tools-0.4.3.tar.gz` & `tmp/imas_tools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imas_tools-0.4.3.tar", max compression
+gzip compressed data, was "imas_tools-0.4.5.tar", max compression
```

## Comparing `imas_tools-0.4.3.tar` & `imas_tools-0.4.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.3/imas_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.3/imas_tools/portal/__init__.py
--rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.3/imas_tools/portal/article.py
--rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.3/imas_tools/portal/interfaces.py
--rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.3/imas_tools/recochoku.py
--rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.3/imas_tools/story/__init__.py
--rw-r--r--   0        0        0      594 2024-05-20 17:11:36.122440 imas_tools-0.4.3/imas_tools/story/adapter.py
--rw-r--r--   0        0        0     3265 2024-05-20 17:20:46.453495 imas_tools-0.4.3/imas_tools/story/gakuen_parser.py
--rw-r--r--   0        0        0      465 2024-05-20 17:23:29.540311 imas_tools-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.3/README.md
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.035606 imas_tools-0.4.5/imas_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:34.820658 imas_tools-0.4.5/imas_tools/portal/__init__.py
+-rw-r--r--   0        0        0     4772 2024-04-19 15:23:32.617350 imas_tools-0.4.5/imas_tools/portal/article.py
+-rw-r--r--   0        0        0     2363 2024-04-18 15:56:10.247192 imas_tools-0.4.5/imas_tools/portal/interfaces.py
+-rw-r--r--   0        0        0     4126 2024-04-13 12:27:59.670781 imas_tools-0.4.5/imas_tools/recochoku.py
+-rw-r--r--   0        0        0        0 2024-05-20 16:09:08.603881 imas_tools-0.4.5/imas_tools/story/__init__.py
+-rw-r--r--   0        0        0     2889 2024-05-23 14:43:59.886176 imas_tools-0.4.5/imas_tools/story/adapter.py
+-rw-r--r--   0        0        0     2673 2024-05-23 14:04:07.150308 imas_tools-0.4.5/imas_tools/story/gakuen_parser.py
+-rw-r--r--   0        0        0     1842 2024-05-23 14:32:30.221320 imas_tools-0.4.5/imas_tools/story/story_csv.py
+-rw-r--r--   0        0        0      517 2024-05-23 15:15:28.635463 imas_tools-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 09:02:36.044152 imas_tools-0.4.5/README.md
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 imas_tools-0.4.5/PKG-INFO
```

### Comparing `imas_tools-0.4.3/imas_tools/portal/article.py` & `imas_tools-0.4.5/imas_tools/portal/article.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.3/imas_tools/portal/interfaces.py` & `imas_tools-0.4.5/imas_tools/portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.3/imas_tools/recochoku.py` & `imas_tools-0.4.5/imas_tools/recochoku.py`

 * *Files identical despite different names*

### Comparing `imas_tools-0.4.3/imas_tools/story/gakuen_parser.py` & `imas_tools-0.4.5/imas_tools/story/gakuen_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,36 @@
-import json
-
+from typing import Any
 
 def parse_identifier(message, i):
     j = i
     while message[i].isalnum() or message[i] == "_":
         i = i + 1
     return i, message[j:i]
 
 
 def parse_string(message, i):
     j = i
-    while message[i] != "=" and message[i] != "]":
+    n = 0
+    while n != 0 or (message[i] != "=" and message[i] != "]"):
+        if message[i] == "\\":
+            i = i + 1
+            if message[i] == "{":
+                n = n + 1
+            elif message[i] == "}":
+                n = n - 1
+                if n < 0:
+                    raise ValueError()
         i = i + 1
     if message[i] == "=":
         i = i - 1
         while message[i] != " ":
             i = i - 1
     return i, message[j:i]
 
 
-def parse_json(message, i):
-    j = i
-    if message[i : i + 2] != r"\{":
-        raise ValueError()
-    n = 1
-    i = i + 2
-    while n > 0:
-        if i + 2 <= len(message):
-            if message[i : i + 2] == r"\{":
-                n = n + 1
-                i = i + 2
-                continue
-            elif message[i : i + 2] == r"\}":
-                n = n - 1
-                i = i + 2
-                continue
-        i = i + 1
-    obj = json.loads(message[j:i].replace(r"\{", "{").replace(r"\}", "}"))
-    if "__tag__" in obj:
-        raise ValueError()
-    return i, obj
-
-
 def parse_object(message, i):
     if message[i] != "[":
         raise ValueError()
     i = i + 1
     i, tag = parse_identifier(message, i)
     obj = {"__tag__": tag}
     while message[i] != "]":
@@ -54,17 +39,15 @@
         i = i + 1
         i, key = parse_identifier(message, i)
         if key == "__tag__":
             raise ValueError()
         if message[i] != "=":
             raise ValueError()
         i = i + 1
-        if i + 2 <= len(message) and message[i : i + 2] == r"\{":
-            i, value = parse_json(message, i)
-        elif message[i] == "[":
+        if message[i] == "[":
             i, value = parse_object(message, i)
         else:
             i, value = parse_string(message, i)
         if key not in obj:
             obj[key] = value
         elif type(obj[key]) is list:
             obj[key].append(value)
@@ -72,57 +55,49 @@
             obj[key] = [obj[key], value]
     if message[i] != "]":
         raise ValueError()
     i = i + 1
     return i, obj
 
 
-def parse_message(message: str):
+def parse_message(message):
     i, o = parse_object(message, 0)
     if i != len(message):
         raise ValueError()
     return o
 
 
-def parse_messages(messages: str) -> list:
+def parse_messages(messages: str) -> list[dict[str, Any]]:
     return [
         parse_message(message) for message in messages.split("\n") if message.strip()
     ]
 
 
-def encode_json(obj):
-    return (
-        json.dumps(obj, ensure_ascii=False, separators=(",", ":"))
-        .replace("{", r"\{")
-        .replace("}", r"\}")
-    )
-
-
 def encode_message_kv(k, v):
     if k == "__tag__":
         if type(v) is not str:
             raise ValueError()
         return v
     if type(v) is list:
-        return " ".join([encode_message_kv(k, w) for w in v])
+        return " ".join([encode_message_kv(k, w) for w in v]) # type: ignore
     if type(v) is str:
         return f"{k}={v}"
     if type(v) is not dict:
-        raise ValueError
-    if "__tag__" in v:
-        return f"{k}={encode_message(v)}"
-    return f"{k}={encode_json(v)}"
+        return ValueError()
+    if "__tag__" not in v:
+        raise ValueError()
+    return f"{k}={encode_message(v)}"
 
 
 def encode_message(obj):
     return (
         "["
         + " ".join(
             [obj["__tag__"]]
             + [encode_message_kv(k, v) for k, v in obj.items() if k != "__tag__"]
         )
         + "]"
     )
 
 
-def encode_messages(objs):
+def encode_messages(objs) -> str:
     return "\n".join(encode_message(obj) for obj in objs)
```

### Comparing `imas_tools-0.4.3/PKG-INFO` & `imas_tools-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imas-tools
-Version: 0.4.3
+Version: 0.4.5
 Summary: 
 Author: darwintree
 Author-email: 17946284+darwintree@users.noreply.github.com
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

