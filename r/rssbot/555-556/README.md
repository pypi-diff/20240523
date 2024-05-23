# Comparing `tmp/rssbot-555.tar.gz` & `tmp/rssbot-556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-555.tar", last modified: Mon Apr 29 11:14:20 2024, max compression
+gzip compressed data, was "rssbot-556.tar", last modified: Thu May 23 18:37:34 2024, max compression
```

## Comparing `rssbot-555.tar` & `rssbot-556.tar`

### file list

```diff
@@ -1,40 +1,34 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/
--rw-r--r--   0 bart      (1000) bart      (1001)     2322 2024-04-29 11:14:20.312440 rssbot-555/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1785 2024-04-28 14:36:32.000000 rssbot-555/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.308441 rssbot-555/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1111 2024-04-29 10:43:37.000000 rssbot-555/bin/rssbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2069 2024-04-29 10:39:51.000000 rssbot-555/bin/rssbotd
--rw-r--r--   0 bart      (1000) bart      (1001)      861 2024-04-28 14:45:08.000000 rssbot-555/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1001)       53 2024-04-28 14:24:03.000000 rssbot-555/rssbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-04-28 14:24:03.000000 rssbot-555/rssbot/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4002 2024-04-28 14:24:03.000000 rssbot-555/rssbot/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)      581 2024-04-28 14:24:03.000000 rssbot-555/rssbot/command.py
--rw-r--r--   0 bart      (1000) bart      (1001)      285 2024-04-28 14:24:03.000000 rssbot-555/rssbot/default.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1397 2024-04-28 14:24:03.000000 rssbot-555/rssbot/errors.py
--rw-r--r--   0 bart      (1000) bart      (1001)      813 2024-04-28 14:24:03.000000 rssbot-555/rssbot/event.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2008 2024-04-28 14:24:03.000000 rssbot-555/rssbot/find.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1405 2024-04-28 14:24:03.000000 rssbot-555/rssbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      238 2024-04-29 10:45:21.000000 rssbot-555/rssbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      216 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      344 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      372 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18838 2024-04-28 14:32:53.000000 rssbot-555/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      183 2024-04-29 10:45:08.000000 rssbot-555/rssbot/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10834 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      988 2024-04-28 14:24:09.000000 rssbot-555/rssbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6085 2024-04-28 14:24:03.000000 rssbot-555/rssbot/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)      278 2024-04-28 14:24:03.000000 rssbot-555/rssbot/repeater.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1260 2024-04-29 10:42:53.000000 rssbot-555/rssbot/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1956 2024-04-28 14:24:03.000000 rssbot-555/rssbot/thread.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1085 2024-04-28 14:24:03.000000 rssbot-555/rssbot/timer.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1120 2024-04-28 14:24:03.000000 rssbot-555/rssbot/whitelist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1266 2024-04-28 14:24:03.000000 rssbot-555/rssbot/workdir.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-04-29 11:14:20.312440 rssbot-555/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     2322 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      638 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-04-29 11:14:20.000000 rssbot-555/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-04-29 11:14:20.312440 rssbot-555/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      185 2024-04-28 14:22:49.000000 rssbot-555/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.073503 rssbot-556/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2378 2024-05-23 18:37:34.073503 rssbot-556/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1841 2024-05-23 18:37:14.000000 rssbot-556/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     2537 2024-05-22 15:24:52.000000 rssbot-556/bin/rssbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1921 2024-05-22 15:24:52.000000 rssbot-556/bin/rssbotd
+-rw-r--r--   0 bart      (1000) bart      (1001)      861 2024-05-22 15:24:52.000000 rssbot-556/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)       72 2024-05-22 15:24:52.000000 rssbot-556/rssbot/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-22 15:24:52.000000 rssbot-556/rssbot/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-22 15:24:52.000000 rssbot-556/rssbot/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-22 15:24:52.000000 rssbot-556/rssbot/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2002 2024-05-23 01:28:27.000000 rssbot-556/rssbot/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-22 15:24:52.000000 rssbot-556/rssbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-22 15:24:52.000000 rssbot-556/rssbot/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.073503 rssbot-556/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      294 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18778 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3112 2024-05-23 13:09:07.000000 rssbot-556/rssbot/modules/opm.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     8892 2024-05-23 13:13:33.000000 rssbot-556/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-22 15:24:52.000000 rssbot-556/rssbot/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-23 01:33:08.000000 rssbot-556/rssbot/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-22 15:24:52.000000 rssbot-556/rssbot/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-22 15:24:52.000000 rssbot-556/rssbot/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-23 18:37:34.069503 rssbot-556/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2378 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      521 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-23 18:37:34.000000 rssbot-556/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-23 18:37:34.073503 rssbot-556/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      185 2024-05-22 15:24:52.000000 rssbot-556/setup.py
```

### Comparing `rssbot-555/PKG-INFO` & `rssbot-556/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 555
+Version: 556
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
@@ -87,14 +87,21 @@
 ::
 
     $ rssbot rss <url>
     $ rssbot dpl <url> <item1,item2>
     $ rssbot rem <url>
     $ rssbot nme <url> <name>
 
+opml
+
+::
+
+    $ rssbot exp
+    $ rssbot imp <filename>
+
 
 SYSTEMD
 
 save the following it in /etc/systemd/system/rssbot.service and
 replace "<user>" with the user running pipx
 
 ::
```

### Comparing `rssbot-555/README.rst` & `rssbot-556/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,21 @@
 ::
 
     $ rssbot rss <url>
     $ rssbot dpl <url> <item1,item2>
     $ rssbot rem <url>
     $ rssbot nme <url> <name>
 
+opml
+
+::
+
+    $ rssbot exp
+    $ rssbot imp <filename>
+
 
 SYSTEMD
 
 save the following it in /etc/systemd/system/rssbot.service and
 replace "<user>" with the user running pipx
 
 ::
```

### Comparing `rssbot-555/pyproject.toml` & `rssbot-556/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rssbot"
 description = "24/7 feed fetcher"
-version = "555"
+version = "556"
 authors = [
     {name = "Bart Thate",email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
```

### Comparing `rssbot-555/rssbot/broker.py` & `rssbot-556/rssbot/broker.py`

 * *Files identical despite different names*

### Comparing `rssbot-555/rssbot/client.py` & `rssbot-556/rssbot/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This file is placed in the Public Domain.
 
 
 "client"
 
 
-from .command import Command
-from .default import Default
-from .errors  import later
-from .event   import Event
-from .handler import Handler
+import inspect
+
+
+from .handler import Event, Handler
+from .object  import Default, Object
+from .thread  import later
 
 
 class Client(Handler):
 
     "Client"
 
     def __init__(self):
@@ -32,39 +33,51 @@
 
     def show(self, evt):
         "show results into a channel."
         for txt in evt.result:
             self.say(evt.channel, txt)
 
 
-def cmnd(txt, out):
-    "do a command using the provided output function."
-    clt = Client()
-    clt.raw = out
-    evn = Event()
-    evn.orig = object.__repr__(clt)
-    evn.txt = txt
-    command(clt, evn)
-    evn.wait()
-    return evn
+class Command(Object): # pylint: disable=R0903
+
+    "Command"
+
+    cmds = Object()
+
+
+def add(func):
+    "add command."
+    setattr(Command.cmds, func.__name__, func)
 
 
 def command(bot, evt):
     "check for and run a command."
-    parse_cmd(evt)
+    parse(evt)
     func = getattr(Command.cmds, evt.cmd, None)
     if func:
         try:
             func(evt)
         except Exception as exc: # pylint: disable=W0718
             later(exc)
     bot.show(evt)
     evt.ready()
 
 
+def cmnd(txt, outer):
+    "do a command using the provided output function."
+    clt = Client()
+    clt.raw = outer
+    evn = Event()
+    evn.orig = object.__repr__(clt)
+    evn.txt = txt
+    command(clt, evn)
+    evn.wait()
+    return evn
+
+
 def laps(seconds, short=True):
     "show elapsed time."
     txt = ""
     nsec = float(seconds)
     if nsec < 1:
         return f"{nsec:.2f}s"
     yea = 365*24*60*60
@@ -97,15 +110,15 @@
         txt += f"{minutes}m"
     if sec:
         txt += f"{sec}s"
     txt = txt.strip()
     return txt
 
 
-def parse_cmd(obj, txt=None):
+def parse(obj, txt=None):
     "parse a string for a command."
     args = []
     obj.args    = obj.args or []
     obj.cmd     = obj.cmd or ""
     obj.gets    = obj.gets or Default()
     obj.hasmods = obj.hasmod or False
     obj.index   = None
@@ -151,25 +164,26 @@
         obj.txt  = obj.cmd or ""
         obj.rest = " ".join(obj.args)
         obj.txt  = obj.cmd + " " + obj.rest
     else:
         obj.txt = obj.cmd or ""
 
 
-def spl(txt):
-    "split comma separated string into a list."
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
+def scancmd(mod) -> None:
+    "scan module for commands."
+    for key, cmd in inspect.getmembers(mod, inspect.isfunction):
+        if key.startswith("cb"):
+            continue
+        if 'event' in cmd.__code__.co_varnames:
+            add(cmd)
 
 
 def __dir__():
     return (
         'Client',
-        'cmnd',
+        'Commands',
+        'add',
         'command',
-        'lapse',
-        'parse_cmd',
-        'spl'
+        'laps',
+        'parse',
+        'scancmd'
     )
```

### Comparing `rssbot-555/rssbot/find.py` & `rssbot-556/rssbot/find.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # This file is placed in the Public Domain.
 
 
-"locate"
+"find"
 
 
 import os
 import time
 
 
-from .default   import Default
-from .object    import fqn, search, update
-from .whitelist import long
-from .workdir   import fetch, store, strip
+from .disk import fetch, long, store, strip
+from .object import Default, fqn, search, update
 
 
 def fns(mtc=""):
     "show list of files."
     dname = ''
     pth = store(mtc)
     for rootdir, dirs, _files in os.walk(pth, topdown=False):
@@ -42,25 +40,27 @@
     return timed
 
 
 def find(mtc, selector=None, index=None, deleted=False):
     "find object matching the selector dict."
     clz = long(mtc)
     nrs = -1
+    result = []
     for fnm in sorted(fns(clz), key=fntime):
         obj = Default()
         fetch(obj, fnm)
-        if not deleted and '__deleted__' in obj:
+        if not deleted and '__deleted__' in dir(obj):
             continue
         if selector and not search(obj, selector):
             continue
         nrs += 1
         if index is not None and nrs != int(index):
             continue
-        yield (fnm, obj)
+        result.append((fnm, obj))
+    return result
 
 
 def last(obj, selector=None):
     "return last object saved."
     if selector is None:
         selector = {}
     result = sorted(
```

### Comparing `rssbot-555/rssbot/handler.py` & `rssbot-556/rssbot/handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 
 
 import queue
 import threading
 import _thread
 
 
-from .object import Object
+from .object import Default, Object
 from .thread import launch
 
 
+rpr = object.__repr__
+
+
 class Handler:
 
     "Handler"
 
     def __init__(self):
         self.cbs      = Object()
         self.queue    = queue.Queue()
@@ -57,11 +60,42 @@
         launch(self.loop)
 
     def stop(self):
         "stop the event loop."
         self.stopped.set()
 
 
+class Event(Default): # pylint: disable=R0902
+
+    "Event"
+
+    def __init__(self):
+        Default.__init__(self)
+        self._thr    = None
+        self._ready  = threading.Event()
+        self.done    = False
+        self.orig    = None
+        self.result  = []
+        self.txt     = ""
+        self.type    = "event"
+
+    def ready(self):
+        "event is ready."
+        self._ready.set()
+
+    def reply(self, txt):
+        "add text to the result"
+        self.result.append(txt)
+
+    def wait(self):
+        "wait for event to be ready."
+        if self._thr:
+            self._thr.join()
+        self._ready.wait()
+        return self.result
+
+
 def __dir__():
     return (
-        'Handler',
+        'Event',
+        'Handler'
     )
```

### Comparing `rssbot-555/rssbot/modules/irc.py` & `rssbot-556/rssbot/modules/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,29 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..client    import Client, command
-from ..default   import Default
-from ..event     import Event
-from ..errors    import Errors, debug, later
-from ..find      import last
-from ..object    import Object, edit, fmt, keys, values
-from ..runtime   import broker
-from ..thread    import launch
-from ..whitelist import whitelist
-from ..workdir   import sync
+from ..client  import Client, command
+from ..disk    import sync, whitelist
+from ..find    import last
+from ..handler import Event
+from ..log     import Logging, debug
+from ..object  import Default, Object, edit, fmt, keys, values
+from ..run     import broker
+from ..thread  import later, launch
 
 
 NAME    = __file__.split(os.sep)[-3]
 saylock = _thread.allocate_lock()
 
 
-Errors.filter = ["PING", "PONG", "PRIVMSG"]
+Logging.filter = ["PING", "PONG", "PRIVMSG"]
 
 
 def init():
     "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
```

### Comparing `rssbot-555/rssbot/modules/rss.py` & `rssbot-556/rssbot/modules/rss.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # This file is placed in the Public Domain.
 
 
 "rich site syndicate"
 
 
+import html
 import html.parser
 import re
 import time
 import urllib
 import urllib.request
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..client     import laps, spl
-from ..default    import Default
-from ..find       import find, fntime, last
-from ..object     import Object, fmt, update, values
-from ..repeater   import Repeater
-from ..runtime    import broker
-from ..thread     import launch
-from ..workdir    import sync
+from ..client import laps
+from ..disk   import sync
+from ..find   import find, fntime, last
+from ..object import Default, Object, fmt, update, values
+from ..run    import broker, spl
+from ..thread import Repeater, launch
 
 
 def init():
     "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
@@ -35,22 +34,14 @@
 
 DEBUG = False
 
 
 fetchlock = _thread.allocate_lock()
 
 
-TEMPLATE = """<opml version="1.0">
-    <head>
-        <title>rssbot opml</title>
-    </head>
-    <body>
-        <outline title="rssbot opml" text="24/7 feed fetcher">"""
-
-
 class Feed(Default): # pylint: disable=R0903
 
     "Feed"
 
 
 class Rss(Default): # pylint: disable=R0903
 
@@ -152,63 +143,26 @@
 
 
 class Parser:
 
     "Parser"
 
     @staticmethod
-    def getvalue(line, attr):
-        "retrieve attribute value."
-        lne = ''
-        index1 = line.find(f'{attr}="')
-        if index1 == -1:
-            return lne
-        index1 += len(attr) + 2
-        index2 = line.find('"', index1)
-        if index2 == -1:
-            index2 = line.find('"/>', index1)
-        if index2 == -1:
-            return lne
-        lne = line[index1:index2]
-        if 'CDATA' in lne:
-            lne = lne.replace('![CDATA[', '')
-            lne = lne.replace(']]', '')
-            #lne = lne[1:-1]
-        return lne
-
-    @staticmethod
-    def getattrs(line, token):
-        "split for attributes."
-        result = ""
-        index1 = line.find(f'<{token} ')
-        if index1 == -1:
-            return result
-        index1 += len(token) + 2
-        index2 = line.find('/>', index1)
-        if index2 == -1:
-            return result
-        result = line[index1:index2]
-        return result.strip()
-
-    @staticmethod
     def getitem(line, item):
         "match items."
         lne = ''
         index1 = line.find(f'<{item}>')
         if index1 == -1:
             return lne
         index1 += len(item) + 2
         index2 = line.find(f'</{item}>', index1)
         if index2 == -1:
             return lne
         lne = line[index1:index2]
-        if 'CDATA' in lne:
-            lne = lne.replace('![CDATA[', '')
-            lne = lne.replace(']]', '')
-            lne = lne[1:-1]
+        lne = cdata(lne)
         return lne.strip()
 
     @staticmethod
     def getitems(text, token):
         "loop for items."
         index = 0
         result = []
@@ -236,26 +190,14 @@
             for itm in spl(items):
                 val = Parser.getitem(line, itm)
                 if val:
                     val = unescape(val.strip())
                     val = val.replace("\n", "")
                     val = striphtml(val)
                     setattr(obj, itm, val)
-                else:
-                    att = Parser.getattrs(line, toke)
-                    if not att:
-                        continue
-                    if itm == "link":
-                        itm = "href"
-                    val = Parser.getvalue(att, itm)
-                    if not val:
-                        continue
-                    if itm == "href":
-                        itm = "link"
-                    setattr(obj, itm, val.strip())
             result.append(obj)
         return result
 
 
 def getfeed(url, items):
     "fetch a feed."
     result = [Object(), Object()]
@@ -268,14 +210,15 @@
     if rest:
         if url.endswith('atom'):
             result = Parser.parse(str(rest.data, 'utf-8'), 'entry', items) or []
         else:
             result = Parser.parse(str(rest.data, 'utf-8'), 'item', items) or []
     return result
 
+
 def gettinyurl(url):
     "fetch a tinyurl."
     postarray = [
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
@@ -287,14 +230,24 @@
             line = txt.decode('UTF-8').strip()
             i = re.search('data-clipboard-text="(.*?)"', line, re.M)
             if i:
                 return i.groups()
     return []
 
 
+def cdata(line):
+    "retrieve text from CDATA."
+    if 'CDATA' in line:
+        lne = line.replace('![CDATA[', '')
+        lne = lne.replace(']]', '')
+        lne = lne[1:-1]
+        return lne
+    return line
+
+
 def geturl(url):
     "fetch a url."
     if not url.startswith("http://") and not url.startswith("https://"):
         return ""
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
     req.add_header('User-agent', useragent("rss fetcher"))
@@ -329,28 +282,14 @@
     for _fn, feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             sync(feed)
     event.reply('ok')
 
 
-def exp(event):
-    "export to opml."
-    event.reply(TEMPLATE)
-    nrs = 0
-    for _fn, obj in find("rss"):
-        nrs += 1
-        name = obj.name or f"url{nrs}"
-        txt = f'<outline name={name} display_list={obj.display_list} xmlUrl="{obj.rss}"/>'
-        event.reply(" "*12 + txt)
-    event.reply(" "*8 + "</outline>")
-    event.reply("    <body>")
-    event.reply("</opml>")
-
-
 def nme(event):
     "set name of feed."
     if len(event.args) != 2:
         event.reply('nme <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
     for _fn, feed in find('rss', selector):
```

### Comparing `rssbot-555/rssbot/modules/thr.py` & `rssbot-556/rssbot/modules/thr.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client import laps
+from ..client    import laps
 from ..object import Object, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
```

### Comparing `rssbot-555/rssbot/object.py` & `rssbot-556/rssbot/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # This file is placed in the Public Domain.
 
 
 "clean namespace"
 
 
 import json
-import os
 import pathlib
 import _thread
 
 
 lock = _thread.allocate_lock()
 
 
-class Object:
+class Object: # pylint: disable=R0902
 
     "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
@@ -26,14 +25,22 @@
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
+class Default(Object): # pylint: disable=R0902,R0903
+
+    "Default"
+
+    def __getattr__(self, key):
+        return self.__dict__.get(key, "")
+
+
 def construct(obj, *args, **kwargs):
     "construct an object from provided arguments."
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
@@ -147,15 +154,16 @@
     "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
     "write an object to disk."
     with lock:
-        cdir(os.path.dirname(pth))
+        path = pathlib.Path(pth)
+        path.parent.mkdir(parents=True, exist_ok=True)
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
     "ObjectDecoder"
@@ -238,25 +246,18 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
 def __dir__():
     return (
         'Object',
+        'Default',
         'construct',
         'dump',
         'dumps',
         'edit',
         'fmt',
         'fqn',
         'hook',
```

### Comparing `rssbot-555/rssbot/runtime.py` & `rssbot-556/rssbot/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # This file is placed in the Public Domain.
 
 
 "runtime"
 
 
-
-from .broker    import Broker
-from .client    import spl
-from .errors    import later
-from .command   import scan as scancmd
-from .whitelist import scan as scancls
+from .broker  import Broker
+from .client  import scancmd
+from .disk    import scancls
+from .thread  import later
 
 
 broker = Broker()
 
 
 def init(pkg, modstr, disable=""):
     "start modules"
     mds = []
     for modname in spl(modstr):
-        if doskip(modname, disable):
+        if skip(modname, disable):
             continue
         mod = getattr(pkg, modname, None)
         if not mod:
             continue
         if "init" in dir(mod):
             try:
                 mod.init()
@@ -33,32 +31,42 @@
     return mds
 
 
 def scan(pkg, modstr, disable=""):
     "scan modules for commands and classes"
     mds = []
     for modname in spl(modstr):
-        if doskip(modname, disable):
+        if skip(modname, disable):
             continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         scancmd(module)
         scancls(module)
     return mds
 
 
-def doskip(name, skipp):
+def skip(name, skipp):
     "check for skipping"
     for skp in spl(skipp):
         if skp in name:
             return True
     return False
 
 
+def spl(txt):
+    "split comma separated string into a list."
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
+
 
 def __dir__():
     return (
         'broker',
         'init',
-        'scan'
+        'scan',
+        'skip',
+        'spl'
     )
```

### Comparing `rssbot-555/rssbot.egg-info/PKG-INFO` & `rssbot-556/rssbot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 555
+Version: 556
 Summary: 24/7 feed fetcher
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/rssbot
 Project-URL: bugs, https://github.com/xobjectz/rssbot/issues
 Project-URL: source, https://github.com/xobjectz/rssbot
 Classifier: Development Status :: 3 - Alpha
@@ -87,14 +87,21 @@
 ::
 
     $ rssbot rss <url>
     $ rssbot dpl <url> <item1,item2>
     $ rssbot rem <url>
     $ rssbot nme <url> <name>
 
+opml
+
+::
+
+    $ rssbot exp
+    $ rssbot imp <filename>
+
 
 SYSTEMD
 
 save the following it in /etc/systemd/system/rssbot.service and
 replace "<user>" with the user running pipx
 
 ::
```

### Comparing `rssbot-555/rssbot.egg-info/SOURCES.txt` & `rssbot-556/rssbot.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,26 @@
 pyproject.toml
 setup.py
 bin/rssbot
 bin/rssbotd
 rssbot/__init__.py
 rssbot/broker.py
 rssbot/client.py
-rssbot/command.py
-rssbot/default.py
-rssbot/errors.py
-rssbot/event.py
+rssbot/disk.py
 rssbot/find.py
 rssbot/handler.py
+rssbot/log.py
 rssbot/object.py
-rssbot/repeater.py
-rssbot/runtime.py
+rssbot/run.py
 rssbot/thread.py
-rssbot/timer.py
-rssbot/whitelist.py
-rssbot/workdir.py
 rssbot.egg-info/PKG-INFO
 rssbot.egg-info/SOURCES.txt
 rssbot.egg-info/dependency_links.txt
 rssbot.egg-info/top_level.txt
 rssbot/modules/__init__.py
 rssbot/modules/cmd.py
 rssbot/modules/err.py
-rssbot/modules/flt.py
 rssbot/modules/irc.py
 rssbot/modules/mod.py
+rssbot/modules/opm.py
 rssbot/modules/rss.py
 rssbot/modules/thr.py
```

