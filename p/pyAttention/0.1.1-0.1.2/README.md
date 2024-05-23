# Comparing `tmp/pyAttention-0.1.1.tar.gz` & `tmp/pyattention-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAttention-0.1.1.tar", last modified: Tue Jun 22 13:58:06 2021, max compression
+gzip compressed data, was "pyattention-0.1.2.tar", max compression
```

## Comparing `pyAttention-0.1.1.tar` & `pyattention-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     2609 2021-06-22 12:17:09.589774 pyAttention-0.1.1/README.md
--rw-r--r--   0        0        0       22 2021-06-21 18:49:09.284692 pyAttention-0.1.1/pyattention/__init__.py
--rw-r--r--   0        0        0     1530 2021-06-12 17:11:55.138359 pyAttention-0.1.1/pyattention/collection.py
--rw-r--r--   0        0        0      361 2021-06-12 17:06:02.672810 pyAttention-0.1.1/pyattention/exception.py
--rw-r--r--   0        0        0     9325 2021-06-12 17:11:55.128167 pyAttention-0.1.1/pyattention/media.py
--rw-r--r--   0        0        0     1442 2021-06-12 17:08:28.106813 pyAttention-0.1.1/pyattention/parser.py
--rw-r--r--   0        0        0    23605 2021-06-12 17:26:46.450836 pyAttention-0.1.1/pyattention/source.py
--rw-r--r--   0        0        0     1394 2021-06-12 17:08:28.162292 pyAttention-0.1.1/pyattention/util.py
--rw-r--r--   0        0        0     1921 2021-06-21 18:51:01.445029 pyAttention-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3264 2021-06-22 13:58:06.955057 pyAttention-0.1.1/setup.py
--rw-r--r--   0        0        0     3551 2021-06-22 13:58:06.955407 pyAttention-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2609 2024-05-21 12:46:19.406605 pyattention-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-21 12:46:19.406893 pyattention-0.1.2/pyAttention/__init__.py
+-rw-r--r--   0        0        0     1530 2024-05-21 12:46:19.406990 pyattention-0.1.2/pyAttention/collection.py
+-rw-r--r--   0        0        0      361 2024-05-21 12:46:19.407090 pyattention-0.1.2/pyAttention/exception.py
+-rw-r--r--   0        0        0     9349 2024-05-21 12:46:19.407259 pyattention-0.1.2/pyAttention/media.py
+-rw-r--r--   0        0        0     1442 2024-05-21 12:46:19.407361 pyattention-0.1.2/pyAttention/parser.py
+-rw-r--r--   0        0        0    23605 2024-05-21 12:46:19.407518 pyattention-0.1.2/pyAttention/source.py
+-rw-r--r--   0        0        0     1394 2024-05-21 12:46:19.407675 pyattention-0.1.2/pyAttention/util.py
+-rw-r--r--   0        0        0     2333 2024-05-23 21:13:16.815537 pyattention-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 pyattention-0.1.2/PKG-INFO
```

### Comparing `pyAttention-0.1.1/README.md` & `pyattention-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyAttention-0.1.1/pyattention/collection.py` & `pyattention-0.1.2/pyAttention/collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from pyattention.source import source
+from pyAttention.source import source
 
 
 class collection(source):
     def __init__(self, loop=None):
         self._srcTaskList = {}
         self._last = {}
```

### Comparing `pyAttention-0.1.1/pyattention/media.py` & `pyattention-0.1.2/pyAttention/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
-from pyattention import parser
-from pyattention.exception import MessageException, MessageTimeout
-from pyattention.source import socketIO, tcp
-from pyattention.util import message, status
+from pyAttention import parser
+from pyAttention.exception import MessageException, MessageTimeout
+from pyAttention.source import socketIO, tcp
+from pyAttention.util import message, status
 
 
 class mpd(tcp):
     def __init__(
         self,
         host="127.0.0.1",
         port=6600,
@@ -52,15 +52,15 @@
 
     def stop(self):
         self._command("stop\n")
 
     def volume(self, val=None):
         if val is None:
             return
-        if type(val) != int:
+        if type(val) is not int:
             raise TypeError("Volume value must be an integer")
 
         self._command(f"volume {val}\n")
 
     async def _mpdMessage(self, wait=0.25):
         """
         Read an MPD message until receiving either an OK or and ACK
@@ -114,19 +114,19 @@
                 msg.status = status.TIMEOUT
                 raise MessageTimeout("No response from source", msg)
 
             msgSize += len(line)
             msg.status = (
                 status.SUCCESS
                 if line[0 : len(good)] == good
-                else status.FAILED
-                if line[0 : len(bad)] == bad
-                else status.OVERFLOW
-                if msgSize > message.MAXSIZE
-                else None
+                else (
+                    status.FAILED
+                    if line[0 : len(bad)] == bad
+                    else status.OVERFLOW if msgSize > message.MAXSIZE else None
+                )
             )
 
             if msg.status is not None:
                 if msg.status in [status.SUCCESS, status.FAILED]:
                     msg.footer = line
                 else:
                     lines.append(line)
@@ -271,11 +271,11 @@
 
     def stop(self):
         self.emit("stop")
 
     def volume(self, val=None):
         if val is None:
             return
-        if type(val) != int:
+        if type(val) is not int:
             raise TypeError("Volume value must be an integer")
 
         self.emit("volume", data=val)
```

### Comparing `pyAttention-0.1.1/pyattention/parser.py` & `pyattention-0.1.2/pyAttention/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # parser.py
-from pyattention.exception import ParserException
+from pyAttention.exception import ParserException
 
 """
 parser module
 
 parsers are functions that accept a message and some optional arguments and return
 a scalar, list, or dictionary that represents the data contained within the message.
```

### Comparing `pyAttention-0.1.1/pyattention/source.py` & `pyattention-0.1.2/pyAttention/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import asyncio
 import concurrent.futures
 import logging
 import time
 import traceback
 
-from pyattention.exception import ConnectionException
-from pyattention.util import status, threadloop
+from pyAttention.exception import ConnectionException
+from pyAttention.util import status, threadloop
 
 DEFAULT_FREQUENCY = (
     60  # If not specified all source polling will occur once per minute
 )
 
 
 class source:
```

### Comparing `pyAttention-0.1.1/pyattention/util.py` & `pyattention-0.1.2/pyAttention/util.py`

 * *Files identical despite different names*

### Comparing `pyAttention-0.1.1/pyproject.toml` & `pyattention-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.coverage.run]
 branch = true
-source = ['pyattention']
-omit = ['setup.py', 'docs/*', '.tox/*', 'pyattention/media.py']
+source = ['pyAttention']
+omit = ['setup.py', 'docs/*', '.tox/*', 'pyAttention/media.py']
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -17,15 +17,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "pyAttention"
-version = "0.1.1"
+version = "0.1.2"
 description = "A library to monitor information sources"
 authors = ["dhrone <dhrone@dhrone.xyz>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dhrone/pyAttention"
 repository = "https://github.com/dhrone/pyAttention"
 keywords = ["pyAttention", "data", "database", "rss", "sql", "socketio", "websocket", "volumio", "mpd", "light", "weight", "message", "broker"]
@@ -33,48 +33,73 @@
   "Environment :: Console",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",    
 ]
+packages = [{include = "pyAttention"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.9,<4.0"
+greenlet = "^3.0.3"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^3.9.0"
-coverage = "^5.5"
-pytest-cov = "^2.11.1"
-isort = "^5.8.0"
-darglint = "^1.7.0"
-rstcheck = "^3.3.1"
-ipython = "^7.24.1"
-codecov = "^2.1.11"
-black = "^21.6b0"
-python-socketio = {version = "^4.6.1", extras = ["client"]}
-psutil = "^5.8.0"
+[tool.poetry.group.test.dependencies]
+pytest = "^8.2.1"
+pytest-cov = "^5.0.0"
+codecov = "^2.1.13"
+coverage = "^7.5.1"
+flake8 = "^7.0.0"
+black = "^24.4.2"
+isort = "^5.13.2"
+
+
+[tool.poetry.group.doc.dependencies]
+darglint = "^1.8.1"
+rstcheck = "^6.2.1"
+
+
+[tool.poetry.group.rss.dependencies]
+beautifulsoup4 = "^4.12.3"
+httpx = "^0.27.0"
+lxml = "^5.2.2"
+
+
+[tool.poetry.group.sqlite.dependencies]
+sqlalchemy = "^2.0.30"
+aiosqlite = "^0.20.0"
+
+
+[tool.poetry.group.postgresql.dependencies]
+sqlalchemy = "^2.0.30"
+asyncpg = "^0.29.0"
+
+
+[tool.poetry.group.mysql.dependencies]
+sqlalchemy = "^2.0.30"
+aiomysql = "^0.2.0"
+
+
+[tool.poetry.group.socketio.dependencies]
+aiohttp = "^3.9.5"
+python-socketio = "^5.11.2"
+
+
+[tool.poetry.group.system.dependencies]
 netifaces = "^0.11.0"
-httpx = "^0.18.1"
-lxml = "^4.6.3"
-beautifulsoup4 = "^4.9.3"
-SQLAlchemy = "^1.4.18"
-aiosqlite = "^0.17.0"
-asyncpg = "^0.23.0"
-aiomysql = "^0.0.21"
-aiohttp = "^3.7.4"
+psutil = "^5.9.8"
 
 [tool.pytest.ini_options]
 minversion = 6.0
 addopts = "-ra -v --cov=pyAttention --cov-report term --cov-report html"
 testpaths = [
   "tests"
 ]
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.8"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pyAttention-0.1.1/PKG-INFO` & `pyattention-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
-Name: pyattention
-Version: 0.1.1
+Name: pyAttention
+Version: 0.1.2
 Summary: A library to monitor information sources
 Home-page: https://github.com/dhrone/pyAttention
 License: MIT
 Keywords: pyAttention,data,database,rss,sql,socketio,websocket,volumio,mpd,light,weight,message,broker
 Author: dhrone
 Author-email: dhrone@dhrone.xyz
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Project-URL: Repository, https://github.com/dhrone/pyAttention
 Description-Content-Type: text/markdown
 
 # pyAttention
 A library to monitor information sources
 
 ![build](https://github.com/dhrone/pyattention/actions/workflows/test.yml/badge.svg) [![codecov](https://codecov.io/gh/dhrone/pyAttention/branch/master/graph/badge.svg?token=ZCAT8XRG4W)](https://codecov.io/gh/dhrone/pyAttention)
```

