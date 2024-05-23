# Comparing `tmp/protai-0.1.0.tar.gz` & `tmp/protai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.1.0.tar", last modified: Fri May 17 06:22:55 2024, max compression
+gzip compressed data, was "protai-0.2.0.tar", last modified: Thu May 23 14:30:47 2024, max compression
```

## Comparing `protai-0.1.0.tar` & `protai-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 06:22:55.444038 protai-0.1.0/
--rw-rw-rw-   0        0        0     2638 2024-05-17 06:22:55.443038 protai-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      828 2024-05-17 06:22:19.000000 protai-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 06:22:55.430879 protai-0.1.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-15 19:00:22.000000 protai-0.1.0/protai/VERSION
--rw-rw-rw-   0        0        0       67 2024-05-17 02:38:44.000000 protai-0.1.0/protai/__init__.py
--rw-rw-rw-   0        0        0     2467 2024-05-17 03:30:15.000000 protai-0.1.0/protai/auth.py
--rw-rw-rw-   0        0        0     2433 2024-05-17 06:06:42.000000 protai-0.1.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-17 06:22:55.442037 protai-0.1.0/protai.egg-info/
--rw-rw-rw-   0        0        0     2638 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      599 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 06:22:55.000000 protai-0.1.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 06:22:55.444038 protai-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.579933 protai-0.2.0/
+-rw-rw-rw-   0        0        0     1479 2024-05-23 14:30:47.578933 protai-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2024-05-17 06:24:20.000000 protai-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.560903 protai-0.2.0/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-23 14:30:37.000000 protai-0.2.0/protai/VERSION
+-rw-rw-rw-   0        0        0       69 2024-05-22 20:52:15.000000 protai-0.2.0/protai/__init__.py
+-rw-rw-rw-   0        0        0     4469 2024-05-23 14:23:52.000000 protai-0.2.0/protai/auth.py
+-rw-rw-rw-   0        0        0     2345 2024-05-23 14:19:00.000000 protai-0.2.0/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.577933 protai-0.2.0/protai.egg-info/
+-rw-rw-rw-   0        0        0     1479 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:30:47.579933 protai-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.2.0/setup.py
```

### Comparing `protai-0.1.0/README.md` & `protai-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `protai-0.1.0/protai/protai.py` & `protai-0.2.0/protai/protai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-#!/usr/bin/env python
-import sys
-import os
-import pathlib
-from rich import print
-from rich.markdown import Markdown
-from groq import Groq
-from auth import authGroq, changeApiKey
-
-
-# Set your GROQ API endpoint URL
-GROQ_API_URL = "https://api.groq.io/v1/query"
-# Get the absolute path of the current directory
-current_directory = os.path.abspath(os.path.dirname(__file__))
-# Construct the absolute path for the VERSION file
-version_file_path = os.path.join(current_directory, "VERSION")
-with open(version_file_path, "r") as f:
-    try:
-        TERMAI_VERSION = f.read().strip()
-        # print(TERMAI_VERSION)
-    except ValueError:
-        TERMAI_VERSION = "Invalid version number"
-
-
-def exitHandler(exit_code: int) -> None:
-    sys.exit(exit_code)
-
-
-def main():
-    if len(sys.argv) < 2:
-        print("Usage: termai <user input>")
-        exitHandler(1)
-
-    # user_input = urllib.parse.quote(sys.argv[1])  # Sanitize the user input
-    user_input = ""
-    for args in sys.argv:
-        if args == sys.argv[0]:
-            continue
-        if args == "-h" or args == "--help":
-            print("Usage: termai <user input>")
-            exitHandler(0)
-        if args == "-v" or args == "--version":
-            print(f"{TERMAI_VERSION}")
-            exitHandler(0)
-        if args == "-c" or args == "--change":
-            print("Change the API key for the GROQ API")
-            exitHandler(changeApiKey())
-        user_input += str(args) + " "
-    # print(f"[DEBUG] User input is: {user_input}")
-
-    # Set the query parameters
-    client = Groq(api_key=authGroq())
-    system_prompt = "You are an AI agent called TermAI. You will reply succinctly to any input you receive. \
-        Your replies will be in the Github Markdown format. ALWAYS start your replies with '[TermAI]: ' \
-        If providing code snippets, always ensure code highlighting for the appropriate programming language \
-        is applied."
-
-    # Send the request to the GROQ API
-    chat_completion = client.chat.completions.create(
-        messages=[
-            {"role": "system", "content": system_prompt},
-            {"role": "user", "content": user_input},
-        ],
-        model="llama3-8b-8192",
-    )
-    reply = chat_completion.choices[0].message.content
-
-    # Print the reply in Markdown using Glow
-    print(Markdown(reply))
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+import sys
+import os
+from rich import print
+from rich.markdown import Markdown
+from groq import Groq
+from auth import authGroq, changeApiKey
+
+
+# Set your GROQ API endpoint URL
+GROQ_API_URL = "https://api.groq.io/v1/query"
+# Get the absolute path of the current directory
+current_directory = os.path.abspath(os.path.dirname(__file__))
+# Construct the absolute path for the VERSION file
+version_file_path = os.path.join(current_directory, "VERSION")
+with open(version_file_path, "r") as f:
+    try:
+        ProtAI_VERSION = f.read().strip()
+        # print(ProtAI_VERSION)
+    except ValueError:
+        ProtAI_VERSION = "Invalid version number"
+
+
+def exitHandler(exit_code: int) -> None:
+    sys.exit(exit_code)
+
+
+def main():
+    if len(sys.argv) < 2:
+        print("Usage: termai <user input>")
+        exitHandler(1)
+
+    # user_input = urllib.parse.quote(sys.argv[1])  # Sanitize the user input
+    user_input = ""
+    for args in sys.argv:
+        if args == sys.argv[0]:
+            continue
+        if args == "-h" or args == "--help":
+            print("Usage: termai <user input>")
+            exitHandler(0)
+        if args == "-v" or args == "--version":
+            print(f"{ProtAI_VERSION}")
+            exitHandler(0)
+        if args == "-c" or args == "--change":
+            print("Change the API key for the GROQ API")
+            exitHandler(changeApiKey())
+        user_input += str(args) + " "
+    # print(f"[DEBUG] User input is: {user_input}")
+
+    # Set the query parameters
+    client = Groq(api_key=authGroq())
+    system_prompt = "You are an AI agent called TermAI. You will reply succinctly to any input you receive. \
+        Your replies will be in the Github Markdown format. ALWAYS start your replies with '[TermAI]: ' \
+        If providing code snippets, always ensure code highlighting for the appropriate programming language \
+        is applied."
+
+    # Send the request to the GROQ API
+    chat_completion = client.chat.completions.create(
+        messages=[
+            {"role": "system", "content": system_prompt},
+            {"role": "user", "content": user_input},
+        ],
+        model="llama3-8b-8192",
+    )
+    reply = chat_completion.choices[0].message.content
+
+    # Print the reply in Markdown using Glow
+    print(Markdown(reply))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `protai-0.1.0/setup.py` & `protai-0.2.0/setup.py`

 * *Files identical despite different names*

