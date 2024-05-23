# Comparing `tmp/comai-0.1.0.tar.gz` & `tmp/comai-0.2.0rc0.tar.gz`

## Comparing `comai-0.1.0.tar` & `comai-0.2.0rc0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0  4135795 2020-02-02 00:00:00.000000 comai-0.1.0/demo.gif
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 comai-0.1.0/logo.svg
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 comai-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 comai-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/__main__.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/animations.py
--rwxr-xr-x   0        0        0     2073 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/cli.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/config.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/context.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/history.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/menu.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 comai-0.1.0/src/comai/translation.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 comai-0.1.0/tests/test_comai.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 comai-0.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.1.0/LICENSE
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 comai-0.1.0/README.md
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 comai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    46765 2020-02-02 00:00:00.000000 comai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0   409001 2020-02-02 00:00:00.000000 comai-0.2.0rc0/demo.gif
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 comai-0.2.0rc0/logo.svg
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 comai-0.2.0rc0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 comai-0.2.0rc0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/__main__.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/animations.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/chain.py
+-rwxr-xr-x   0        0        0     5158 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/cli.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/context.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/history.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/ollama.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/openai.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/prompt.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 comai-0.2.0rc0/src/comai/settings.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 comai-0.2.0rc0/tests/test_comai.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 comai-0.2.0rc0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 comai-0.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 comai-0.2.0rc0/README.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 comai-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    46042 2020-02-02 00:00:00.000000 comai-0.2.0rc0/PKG-INFO
```

### Comparing `comai-0.1.0/logo.svg` & `comai-0.2.0rc0/logo.svg`

 * *Files identical despite different names*

### Comparing `comai-0.1.0/.github/workflows/release.yml` & `comai-0.2.0rc0/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 name: Release new version
 
-on: 
+on:
   workflow_dispatch:
     inputs:
       type:
-        description: 'Release type'
+        description: "Release type"
         required: true
-        default: 'preview'
+        default: "preview"
         type: choice
         options:
-        - major
-        - minor
-        - fix
-        - preview
-        - release
+          - fix
+          - minor
+          - minor,preview
+          - major,preview
+          - release
 
 jobs:
   test:
     uses: ./.github/workflows/tests.yml
-    secrets:
-      OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
   release:
     needs: test
     runs-on: ubuntu-latest
     steps:
       - name: Checkout Repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: setup git
         run: |
           git config user.name "$GITHUB_ACTOR"
           git config user.email "${GITHUB_ACTOR_ID}+${GITHUB_ACTOR}@users.noreply.github.com"
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - name: Install hatch
         run: pip install hatch
       - name: Bump Version
         run: |
           hatch version $TYPE
```

### Comparing `comai-0.1.0/src/comai/context.py` & `comai-0.2.0rc0/src/comai/context.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import os
 import sys
 from dataclasses import dataclass
 
+session_id = os.getenv("TERM_SESSION_ID")
+
 shell = os.getenv("SHELL")
 if not shell:
     shell = "bash"
 
 system = None
 if sys.platform == "linux":
     system = "linux"
@@ -13,22 +15,23 @@
     system = "mac"
 
 
 @dataclass
 class Context:
     system: str
     shell: str
+    session_id: str | None
 
 
 def get_context() -> Context:
     system = None
     if sys.platform == "linux":
         system = "linux"
     elif sys.platform == "darwin":
         system = "macOS"
 
     shell = os.getenv("SHELL")
     if not shell:
         shell = "bash"
     shell = shell.split("/")[-1]
 
-    return Context(system, shell)
+    return Context(system, shell, session_id)
```

### Comparing `comai-0.1.0/LICENSE` & `comai-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `comai-0.1.0/README.md` & `comai-0.2.0rc0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,107 @@
 <div align="center">
-  <img src="https://raw.githubusercontent.com/ricopinazo/comai/main/logo.svg" alt="demo" width="200"/>
-  
-  **The AI powered terminal assistant**
-  
-  [![Tests](https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg)](https://github.com/ricopinazo/comai/actions/workflows/tests.yml)
-  [![Latest release](https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases)](https://github.com/ricopinazo/comai/releases)
-  [![PyPI](https://img.shields.io/pypi/v/comai)](https://pypi.org/project/comai/)
-  [![Issues](https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen)](https://github.com/ricopinazo/comai/issues)
-  [![License GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-  [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+  <img src="https://raw.githubusercontent.com/ricopinazo/comai/main/logo.svg" alt="comai" width="200"/>
+
+**The AI powered terminal assistant**
+
+[![Tests](https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg)](https://github.com/ricopinazo/comai/actions/workflows/tests.yml)
+[![Latest release](https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases)](https://github.com/ricopinazo/comai/releases)
+[![PyPI](https://img.shields.io/pypi/v/comai)](https://pypi.org/project/comai/)
+[![Issues](https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen)](https://github.com/ricopinazo/comai/issues)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/comai)](https://pypi.org/project/comai/)
+[![License GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+
 </div>
 
 ## What is comai? 🎯
 
-`comai` is an open source terminal assistant powered by OpenAI API that enables you to interact with your command line interface using natural language instructions. It simplifies your workflow by converting natural language queries into executable commands. No more memorizing complex syntax. Just chat with `comai` using plain English!
+`comai` is an open source CLI utility that translates natural language instructions into executable commands.
 
 <div align="left">
-<img src="https://raw.githubusercontent.com/ricopinazo/comai/main/demo.gif" alt="demo" width="350"/>
+<img src="https://github.com/ricopinazo/comai/blob/956aa235f3950fe5b057d2e6d50032702a579b0c/demo.gif" alt="demo" width="350"/>
 </div>
 
 ## Installation 🚀
 
-Getting `comai` up and running is a breeze. You can simply use [`pip`](https://pip.pypa.io/en/stable/) to install the latest version:
+`comai` is available as a python package. We recommend using [`pipx`](https://pypa.github.io/pipx/) to install it:
 
 ```shell
-pip install comai
+pipx install comai
 ```
 
-However, if you usually work with python environments, it is recommended to use [`pipx`](https://pypa.github.io/pipx/) instead:
+By default, `comai` is setup to use [ollama](https://ollama.com) under the hood, which allows you to host any popular open source LLM locally. If you are happy with this, make sure to install and have ollama running. You can find the install instructions [here](https://ollama.com/download).
+
+Once installed, make sure to download the `llama3` model, since comai has been optimised for it
 
 ```shell
-pipx install comai
+ollama pull llama3
 ```
 
-The first time you run it, it'll ask you for an OpenAI API key. You can create a developer account [here](https://platform.openai.com/overview). Once in your account, go to `API Keys` section and `Create new secret key`. We recommend setting a usage limit under `Billing`/`Usage limits`.
+Otherwise, you can set up any other model available in the ollama service via:
+
+```shell
+comai --config
+```
 
 > **_NOTE:_** `comai` uses the environment variable `TERM_SESSION_ID` to maintain context between calls so you don't need to repeat yourself giving instructions to it. You can check if it is available in your default terminal checking the output of `echo $TERM_SESSION_ID`, which should return some type of UUID. If the output is empty, you can simply add the following to your `.zshrc`/`.bashrc` file:
+>
 > ```shell
 > export TERM_SESSION_ID=$(uuidgen)
 > ```
 
-## Usage Examples 🎉
+## Usage examples 🎉
 
 Using `comai` is straightforward. Simply invoke the `comai` command followed by your natural language instruction. `comai` will provide you with the corresponding executable command, which you can execute by pressing Enter or ignore by pressing any other key.
 
 Let's dive into some exciting examples of how you can harness the power of `comai`:
 
-1. Manage your system like a pro:
-```shell
-$ comai print my private ip address
-❯ ifconfig | grep "inet " | grep -v 127.0.0.1 | awk '{print $2}'
-192.168.0.2
+1. Access network details:
 
-$ comai and my public one
-❯ curl ifconfig.me
+```
+$ comai print my public ip address
+❯ curl -s4 ifconfig.co
 92.234.58.146
 ```
 
-2. Master the intricacies of `git`:
+2. Manage `git` like a pro:
+
 ```shell
-$ comai squash the last 3 commits into a single commit
-❯ git rebase -i HEAD~3
+$ comai rename the current branch to awesome-branch
+❯ git branch -m $(git rev-parse --abbrev-ref HEAD) awesome-branch
 
 $ comai show me all the branches having commit c4c0d2d in common
-❯ git branch --contains c4c0d2d
-  chat-api
-  configparser
-* main
+❯ git branch -a --contains c4c0d2d
+  main
+  fix/terrible-bug
+* awesome-branch
 ```
 
-3. Check the weather forecast for your location:
-```shell
-$ comai show me the weather forecast
-❯ curl wttr.in
-```
+3. Find the annoying process using the port 8080:
 
-4. Find the annoying process using the port 8080:
 ```shell
 $ comai show me the process using the port 8080
 ❯ lsof -i :8080
 COMMAND   PID      USER   FD   TYPE            DEVICE SIZE/OFF NODE NAME
 node    36350 pedrorico   18u  IPv4 0xe0d28ea918e376b      0t0  TCP *:http-alt (LISTEN)
-
-$ comai show me only the PID
-❯ lsof -t -i :8080
-36350
-
-$ comai kill it
-❯ kill $(lsof -t -i :8080)
 ```
 
-5. Swiftly get rid of all your docker containers:
+4. Get rid of all your docker containers:
+
 ```shell
 $ comai stop and remove all running docker containers
 ❯ docker stop $(docker ps -aq) && docker rm $(docker ps -aq)
 ```
 
-These are just a few examples of how `comai` can help you harness the power of the command line and provide you with useful and entertaining commands. Feel free to explore and experiment with the commands generated by `comai` to discover more exciting possibilities!
-
 ## Contributions welcome! 🤝
 
 If you're interested in joining the development of new features for `comai`, here's all you need to get started:
 
 1. Clone the [repository](https://github.com/ricopinazo/comai) and navigate to the root folder.
 2. Install the package in editable mode by running `pip install -e .`.
-3. Run the tests using `pytest`. Make sure you have the `OPENAI_API_KEY` environment variable set up with your OpenAI API key. Alternatively, you can create a file named `.env` and define the variable there.
-
-
-This project utilizes black for code formatting. To ensure your changes adhere to this format, simply follow these steps:
-
-```shell
-pip install black
-black .
-```
-
-For users of VS Code, you can configure the following options after installing `black`:
-
-```json
-"editor.formatOnSave": true,
-"python.formatting.provider": "black"
-```
+3. Run the tests using `pytest`.
+4. Format your code using [black](https://github.com/psf/black) before submitting any change.
 
 ## License 📜
 
 Comai is licensed under the GPLv3. You can find the full text of the license in the [LICENSE](./LICENSE) file.
```

### Comparing `comai-0.1.0/pyproject.toml` & `comai-0.2.0rc0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "comai"
 dynamic = ["version"]
-authors = [
-  { name="Pedro Rico", email="ricopinazo@gmail.com" },
-]
+authors = [{ name = "Pedro Rico", email = "ricopinazo@gmail.com" }]
 description = "AI powered console assistant"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Operating System :: MacOS",
     "Operating System :: Unix",
 ]
 dependencies = [
-  "typer==0.9.0",
-  "openai==0.27.5",
-  "cryptography==40.0.2",
-  "termcolor==2.3.0",
+    "typer-slim==0.12.3",
+    "rich==13.7.1",
+    "prompt-toolkit==3.0.43",
+    "simple-term-menu==1.6.4",
+    "langchain==0.1.17",
+    "langchain-openai==0.1.6",
+    "ollama==0.1.9",
 ]
 
 [project.urls]
 homepage = "https://github.com/ricopinazo/comai"
 repository = "https://github.com/ricopinazo/comai"
 issues = "https://github.com/ricopinazo/comai/issues"
 
 [project.scripts]
 comai = "comai.cli:app"
 
 [project.optional-dependencies]
-test = [
+dev = [
     "pytest",
     "hatchling",
-    "python-dotenv"
+    "types-requests==2.31.0.20240406",
+    "mypy==1.9.0",
+    "black==24.4.0",
 ]
 
 [tool.hatch.version]
 path = "src/comai/__init__.py"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `comai-0.1.0/PKG-INFO` & `comai-0.2.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: comai
-Version: 0.1.0
+Version: 0.2.0rc0
 Summary: AI powered console assistant
 Project-URL: homepage, https://github.com/ricopinazo/comai
 Project-URL: repository, https://github.com/ricopinazo/comai
 Project-URL: issues, https://github.com/ricopinazo/comai/issues
 Author-email: Pedro Rico <ricopinazo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -683,143 +683,129 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: cryptography==40.0.2
-Requires-Dist: openai==0.27.5
-Requires-Dist: termcolor==2.3.0
-Requires-Dist: typer==0.9.0
-Provides-Extra: test
-Requires-Dist: hatchling; extra == 'test'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: python-dotenv; extra == 'test'
+Requires-Dist: langchain-openai==0.1.6
+Requires-Dist: langchain==0.1.17
+Requires-Dist: ollama==0.1.9
+Requires-Dist: prompt-toolkit==3.0.43
+Requires-Dist: rich==13.7.1
+Requires-Dist: simple-term-menu==1.6.4
+Requires-Dist: typer-slim==0.12.3
+Provides-Extra: dev
+Requires-Dist: black==24.4.0; extra == 'dev'
+Requires-Dist: hatchling; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: types-requests==2.31.0.20240406; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/ricopinazo/comai/main/logo.svg" alt="demo" width="200"/>
-  
-  **The AI powered terminal assistant**
-  
-  [![Tests](https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg)](https://github.com/ricopinazo/comai/actions/workflows/tests.yml)
-  [![Latest release](https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases)](https://github.com/ricopinazo/comai/releases)
-  [![PyPI](https://img.shields.io/pypi/v/comai)](https://pypi.org/project/comai/)
-  [![Issues](https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen)](https://github.com/ricopinazo/comai/issues)
-  [![License GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
-  [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+  <img src="https://raw.githubusercontent.com/ricopinazo/comai/main/logo.svg" alt="comai" width="200"/>
+
+**The AI powered terminal assistant**
+
+[![Tests](https://github.com/ricopinazo/comai/actions/workflows/tests.yml/badge.svg)](https://github.com/ricopinazo/comai/actions/workflows/tests.yml)
+[![Latest release](https://img.shields.io/github/v/release/ricopinazo/comai?color=brightgreen&include_prereleases)](https://github.com/ricopinazo/comai/releases)
+[![PyPI](https://img.shields.io/pypi/v/comai)](https://pypi.org/project/comai/)
+[![Issues](https://img.shields.io/github/issues/ricopinazo/comai?color=brightgreen)](https://github.com/ricopinazo/comai/issues)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/comai)](https://pypi.org/project/comai/)
+[![License GPLv3](https://img.shields.io/badge/license-GPLv3-blue.svg)](./LICENSE)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+
 </div>
 
 ## What is comai? 🎯
 
-`comai` is an open source terminal assistant powered by OpenAI API that enables you to interact with your command line interface using natural language instructions. It simplifies your workflow by converting natural language queries into executable commands. No more memorizing complex syntax. Just chat with `comai` using plain English!
+`comai` is an open source CLI utility that translates natural language instructions into executable commands.
 
 <div align="left">
-<img src="https://raw.githubusercontent.com/ricopinazo/comai/main/demo.gif" alt="demo" width="350"/>
+<img src="https://github.com/ricopinazo/comai/blob/956aa235f3950fe5b057d2e6d50032702a579b0c/demo.gif" alt="demo" width="350"/>
 </div>
 
 ## Installation 🚀
 
-Getting `comai` up and running is a breeze. You can simply use [`pip`](https://pip.pypa.io/en/stable/) to install the latest version:
+`comai` is available as a python package. We recommend using [`pipx`](https://pypa.github.io/pipx/) to install it:
 
 ```shell
-pip install comai
+pipx install comai
 ```
 
-However, if you usually work with python environments, it is recommended to use [`pipx`](https://pypa.github.io/pipx/) instead:
+By default, `comai` is setup to use [ollama](https://ollama.com) under the hood, which allows you to host any popular open source LLM locally. If you are happy with this, make sure to install and have ollama running. You can find the install instructions [here](https://ollama.com/download).
+
+Once installed, make sure to download the `llama3` model, since comai has been optimised for it
 
 ```shell
-pipx install comai
+ollama pull llama3
 ```
 
-The first time you run it, it'll ask you for an OpenAI API key. You can create a developer account [here](https://platform.openai.com/overview). Once in your account, go to `API Keys` section and `Create new secret key`. We recommend setting a usage limit under `Billing`/`Usage limits`.
+Otherwise, you can set up any other model available in the ollama service via:
+
+```shell
+comai --config
+```
 
 > **_NOTE:_** `comai` uses the environment variable `TERM_SESSION_ID` to maintain context between calls so you don't need to repeat yourself giving instructions to it. You can check if it is available in your default terminal checking the output of `echo $TERM_SESSION_ID`, which should return some type of UUID. If the output is empty, you can simply add the following to your `.zshrc`/`.bashrc` file:
+>
 > ```shell
 > export TERM_SESSION_ID=$(uuidgen)
 > ```
 
-## Usage Examples 🎉
+## Usage examples 🎉
 
 Using `comai` is straightforward. Simply invoke the `comai` command followed by your natural language instruction. `comai` will provide you with the corresponding executable command, which you can execute by pressing Enter or ignore by pressing any other key.
 
 Let's dive into some exciting examples of how you can harness the power of `comai`:
 
-1. Manage your system like a pro:
-```shell
-$ comai print my private ip address
-❯ ifconfig | grep "inet " | grep -v 127.0.0.1 | awk '{print $2}'
-192.168.0.2
+1. Access network details:
 
-$ comai and my public one
-❯ curl ifconfig.me
+```
+$ comai print my public ip address
+❯ curl -s4 ifconfig.co
 92.234.58.146
 ```
 
-2. Master the intricacies of `git`:
+2. Manage `git` like a pro:
+
 ```shell
-$ comai squash the last 3 commits into a single commit
-❯ git rebase -i HEAD~3
+$ comai rename the current branch to awesome-branch
+❯ git branch -m $(git rev-parse --abbrev-ref HEAD) awesome-branch
 
 $ comai show me all the branches having commit c4c0d2d in common
-❯ git branch --contains c4c0d2d
-  chat-api
-  configparser
-* main
+❯ git branch -a --contains c4c0d2d
+  main
+  fix/terrible-bug
+* awesome-branch
 ```
 
-3. Check the weather forecast for your location:
-```shell
-$ comai show me the weather forecast
-❯ curl wttr.in
-```
+3. Find the annoying process using the port 8080:
 
-4. Find the annoying process using the port 8080:
 ```shell
 $ comai show me the process using the port 8080
 ❯ lsof -i :8080
 COMMAND   PID      USER   FD   TYPE            DEVICE SIZE/OFF NODE NAME
 node    36350 pedrorico   18u  IPv4 0xe0d28ea918e376b      0t0  TCP *:http-alt (LISTEN)
-
-$ comai show me only the PID
-❯ lsof -t -i :8080
-36350
-
-$ comai kill it
-❯ kill $(lsof -t -i :8080)
 ```
 
-5. Swiftly get rid of all your docker containers:
+4. Get rid of all your docker containers:
+
 ```shell
 $ comai stop and remove all running docker containers
 ❯ docker stop $(docker ps -aq) && docker rm $(docker ps -aq)
 ```
 
-These are just a few examples of how `comai` can help you harness the power of the command line and provide you with useful and entertaining commands. Feel free to explore and experiment with the commands generated by `comai` to discover more exciting possibilities!
-
 ## Contributions welcome! 🤝
 
 If you're interested in joining the development of new features for `comai`, here's all you need to get started:
 
 1. Clone the [repository](https://github.com/ricopinazo/comai) and navigate to the root folder.
 2. Install the package in editable mode by running `pip install -e .`.
-3. Run the tests using `pytest`. Make sure you have the `OPENAI_API_KEY` environment variable set up with your OpenAI API key. Alternatively, you can create a file named `.env` and define the variable there.
-
-
-This project utilizes black for code formatting. To ensure your changes adhere to this format, simply follow these steps:
-
-```shell
-pip install black
-black .
-```
-
-For users of VS Code, you can configure the following options after installing `black`:
-
-```json
-"editor.formatOnSave": true,
-"python.formatting.provider": "black"
-```
+3. Run the tests using `pytest`.
+4. Format your code using [black](https://github.com/psf/black) before submitting any change.
 
 ## License 📜
 
 Comai is licensed under the GPLv3. You can find the full text of the license in the [LICENSE](./LICENSE) file.
```

