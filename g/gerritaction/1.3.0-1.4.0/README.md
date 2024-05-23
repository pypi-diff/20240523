# Comparing `tmp/gerritaction-1.3.0.tar.gz` & `tmp/gerritaction-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerritaction-1.3.0.tar", last modified: Wed Aug  2 02:16:26 2023, max compression
+gzip compressed data, was "gerritaction-1.4.0.tar", last modified: Thu May 23 10:50:59 2024, max compression
```

## Comparing `gerritaction-1.3.0.tar` & `gerritaction-1.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-08-02 02:08:33.000000 gerritaction-1.3.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       69 2023-08-02 02:08:33.000000 gerritaction-1.3.0/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-08-02 02:16:26.798526 gerritaction-1.3.0/PKG-INFO
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2666 2023-08-02 02:13:03.000000 gerritaction-1.3.0/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2023-08-02 02:13:20.000000 gerritaction-1.3.0/action.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.790526 gerritaction-1.3.0/gerritaction/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/__init__.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)      226 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/__version__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/action/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/action/__init__.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)     3121 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/action/action.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/cmd/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/__init__.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)     1276 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/argument.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/cmd/banner.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/config/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/config/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1799 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/config/config.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/gerrit/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/gerrit/__init__.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)     9545 2023-08-02 02:14:13.000000 gerritaction-1.3.0/gerritaction/gerrit/gerrit.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/logger/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/logger/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1608 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/logger/logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      877 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/main.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.794526 gerritaction-1.3.0/gerritaction/proto/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/proto/__init__.py
--rw-r--r--   0 codespace  (1000) codespace  (1000)      387 2023-08-02 02:13:20.000000 gerritaction-1.3.0/gerritaction/proto/proto.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-08-02 02:16:26.790526 gerritaction-1.3.0/gerritaction.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      777 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      107 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-08-02 02:16:26.000000 gerritaction-1.3.0/gerritaction.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-08-02 02:16:26.798526 gerritaction-1.3.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1470 2023-08-02 02:13:20.000000 gerritaction-1.3.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.238382 gerritaction-1.4.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-23 04:13:27.000000 gerritaction-1.4.0/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       69 2024-05-23 04:13:27.000000 gerritaction-1.4.0/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4064 2024-05-23 10:50:59.238382 gerritaction-1.4.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3151 2024-05-23 10:18:06.000000 gerritaction-1.4.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      223 2024-05-23 04:13:27.000000 gerritaction-1.4.0/action.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.230382 gerritaction-1.4.0/gerritaction/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      226 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/__version__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.234382 gerritaction-1.4.0/gerritaction/action/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/action/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5148 2024-05-23 10:18:13.000000 gerritaction-1.4.0/gerritaction/action/action.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.234382 gerritaction-1.4.0/gerritaction/cmd/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/cmd/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2236 2024-05-23 10:18:59.000000 gerritaction-1.4.0/gerritaction/cmd/argument.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/cmd/banner.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.234382 gerritaction-1.4.0/gerritaction/config/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/config/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3036 2024-05-23 10:19:24.000000 gerritaction-1.4.0/gerritaction/config/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.238382 gerritaction-1.4.0/gerritaction/gerrit/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/gerrit/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14278 2024-05-23 10:19:48.000000 gerritaction-1.4.0/gerritaction/gerrit/gerrit.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.238382 gerritaction-1.4.0/gerritaction/logger/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/logger/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1608 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/logger/logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1065 2024-05-23 10:20:17.000000 gerritaction-1.4.0/gerritaction/main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.238382 gerritaction-1.4.0/gerritaction/proto/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/proto/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-23 04:13:27.000000 gerritaction-1.4.0/gerritaction/proto/proto.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-23 10:50:59.238382 gerritaction-1.4.0/gerritaction.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4064 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      777 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      107 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2024-05-23 10:50:59.000000 gerritaction-1.4.0/gerritaction.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2024-05-23 10:50:59.238382 gerritaction-1.4.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1470 2024-05-23 04:13:27.000000 gerritaction-1.4.0/setup.py
```

### Comparing `gerritaction-1.3.0/LICENSE` & `gerritaction-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gerritaction-1.3.0/PKG-INFO` & `gerritaction-1.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: gerritaction
-Version: 1.3.0
-Summary: Gerrit Action
-Home-page: https://github.com/craftslab/gerritaction
-Download-URL: https://github.com/craftslab/gerritaction/archive/v1.3.0.tar.gz
-Author: Jia Jia
-Author-email: angersax@sina.com
-License: Apache-2.0
-Keywords: gerrit,action
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gerritaction
 
 [![Actions Status](https://github.com/craftslab/gerritaction/workflows/CI/badge.svg?branch=master&event=push)](https://github.com/craftslab/gerritaction/actions?query=workflow%3ACI)
 [![License](https://img.shields.io/github/license/craftslab/gerritaction.svg?color=brightgreen)](https://github.com/craftslab/gerritaction/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/gerritaction.svg?color=brightgreen)](https://pypi.org/project/gerritaction)
 [![Tag](https://img.shields.io/github/tag/craftslab/gerritaction.svg?color=brightgreen)](https://github.com/craftslab/gerritaction/tags)
 
@@ -40,46 +22,62 @@
 ## Run
 
 ```bash
 git clone https://github.com/craftslab/gerritaction.git
 
 cd gerritaction
 pip install -Ur requirements.txt
-python action.py --config-file="config.yml" --gerrit-action="delete-reviewer:account-id,..." --gerrit-query="since:2021-01-01 until:2021-01-02"
+python action.py --config-file="config.yml" --change-query="since:2024-01-01 until:2024-01-02"
 ```
 
 
 
 ## Docker
 
 ```bash
 git clone https://github.com/craftslab/gerritaction.git
 
 cd gerritaction
 docker build --no-cache -f Dockerfile -t craftslab/gerritaction:latest .
-docker run -it -v /tmp:/tmp craftslab/gerritaction:latest ./gerritaction --config-file="config.yml" --gerrit-action="delete-reviewer:account-id,..." --gerrit-query="since:2021-01-01 until:2021-01-02"
+docker run -it -v /tmp:/tmp craftslab/gerritaction:latest ./gerritaction --config-file="config.yml" --change-query="since:2024-01-01 until:2024-01-02"
 ```
 
 
 
 ## Usage
 
 ```
-usage: action.py [-h] --config-file CONFIG_FILE --gerrit-action GERRIT_ACTION --gerrit-query GERRIT_QUERY [-v]
+usage: action.py [-h] --config-file CONFIG_FILE
+                 [--account-query ACCOUNT_QUERY] [--change-query CHANGE_QUERY]
+                 [--change-action CHANGE_ACTION] [--group-query GROUP_QUERY]
+                 [--project-query PROJECT_QUERY] [--output-file OUTPUT_FILE]
+                 [-v]
 
 Gerrit Action
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --config-file CONFIG_FILE
                         config file (.yml)
-  --gerrit-action GERRIT_ACTION
-                        gerrit action (add-reviewer:account-id,... delete-reviewer:account-id,... add-attention:account-id,... remove-attention:account-id,... approve-change:Code-Review=+2,... delete-change submit-change)
-  --gerrit-query GERRIT_QUERY
-                        gerrit query (status:open since:2021-01-01 until:2021-01-02)
+  --account-query ACCOUNT_QUERY
+                        account query (name:john email:example.com)
+  --change-query CHANGE_QUERY
+                        change query (status:open since:2024-01-01
+                        until:2024-01-02)
+  --change-action CHANGE_ACTION
+                        change action (add-reviewer:account-id,... delete-
+                        reviewer:account-id,... add-attention:account-id,...
+                        remove-attention:account-id,... approve-change:Code-
+                        Review=+2,... delete-change submit-change)
+  --group-query GROUP_QUERY
+                        group query (name:admin member:john)
+  --project-query PROJECT_QUERY
+                        project query (name:test state:active)
+  --output-file OUTPUT_FILE
+                        output file (.json)
   -v, --version         show program's version number and exit
 ```
 
 
 
 ## Settings
 
@@ -94,17 +92,14 @@
   name: gerritaction
 spec:
   gerrit:
     host: http://127.0.0.1/
     port: 8080
     user: user
     pass: pass
-    query:
-      option:
-        - CURRENT_REVISION
 ```
 
 
 
 ## License
 
 Project License can be found [here](LICENSE).
```

### Comparing `gerritaction-1.3.0/gerritaction/gerrit/gerrit.py` & `gerritaction-1.4.0/gerritaction/gerrit/gerrit.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,59 +14,126 @@
         self._info = info
 
     def __str__(self):
         return self._info
 
 
 class Gerrit(object):
-    _QUERY_LIMIT = 1000
+    _ACCOUNT_LIMIT = 1000
+    _ACCOUNT_OPTION = ["DETAILS"]
+    _CHANGE_LIMIT = 1000
+    _CHANGE_OPTION = ["CURRENT_REVISION"]
+    _GROUP_LIMIT = 1000
+    _GROUP_OPTION = ["INCLUDES"]
+    _PROJECT_LIMIT = 1000
+    _PROJECT_OPTION = []
 
     def __init__(self, config):
         if config is None or config.get("gerrit", None) is None:
             raise GerritException("config invalid")
         self._config = config["gerrit"]
         self._host = str(self._config.get("host", "http://127.0.0.1"))
         self._port = str(self._config.get("port", 8080))
         self._user = str(self._config.get("user", ""))
         self._pass = str(self._config.get("pass", ""))
-        self._query = self._config.get("query", {"option": ["CURRENT_REVISION"]})
         if len(self._pass) != 0 and len(self._user) != 0:
             self._url = self._host + ":" + self._port + "/a"
         else:
             self._url = self._host + ":" + self._port
 
-    def query_changes(self, search, start):
-        def _helper(search, start):
+    def query_account(self, search, start):
+        def _accounts(_search, _start):
             payload = {
-                "o": self._query["option"],
-                "q": search,
-                "start": start,
-                "n": self._QUERY_LIMIT,
+                "o": self._ACCOUNT_OPTION,
+                "q": _search,
+                "start": _start,
+                "n": self._ACCOUNT_LIMIT,
+            }
+            if len(self._pass) != 0 and len(self._user) != 0:
+                response = requests.get(
+                    url=self._url + "/accounts/",
+                    auth=(self._user, self._pass),
+                    params=payload,
+                )
+            else:
+                response = requests.get(url=self._url + "/accounts/", params=payload)
+            if response.status_code != requests.codes.ok:
+                Logger.error("failed to query account with search %s" % _search)
+                return None
+            return json.loads(response.text.replace(")]}'", ""))
+
+        def _deduplicate(data):
+            buf = []
+            key = []
+            for item in data:
+                k = item.get("ssh_public_key", "")
+                if k not in key:
+                    key.append(k)
+            for item in data:
+                if item.get("ssh_public_key", "") in key:
+                    buf.append(item)
+            return buf
+
+        def _sshkeys(data):
+            for i in range(len(data)):
+                data[i]["sshkeys"] = _deduplicate(self.get_sshkey(data[i]))
+            return data
+
+        buf = _accounts(search, start)
+        if buf is None or len(buf) == 0:
+            return []
+        if buf[-1].get("_more_accounts", False) is False:
+            return _sshkeys(buf)
+        buf.extend(self.query_account(search, start + len(buf)))
+        return buf
+
+    def query_change(self, search, start):
+        def _helper(_search, _start):
+            payload = {
+                "o": self._CHANGE_OPTION,
+                "q": _search,
+                "start": _start,
+                "n": self._CHANGE_LIMIT,
             }
             if len(self._pass) != 0 and len(self._user) != 0:
                 response = requests.get(
                     url=self._url + "/changes/",
                     auth=(self._user, self._pass),
                     params=payload,
                 )
             else:
                 response = requests.get(url=self._url + "/changes/", params=payload)
             if response.status_code != requests.codes.ok:
-                Logger.error("failed to query change with search %s" % search)
+                Logger.error("failed to query change with search %s" % _search)
                 return None
             return json.loads(response.text.replace(")]}'", ""))
 
         buf = _helper(search, start)
         if buf is None or len(buf) == 0:
             return []
         if buf[-1].get("_more_changes", False) is False:
             return buf
-        buf.extend(self.query_changes(search, start + len(buf)))
+        buf.extend(self.query_change(search, start + len(buf)))
         return buf
 
+    def get_sshkey(self, account):
+        if len(self._pass) != 0 and len(self._user) != 0:
+            response = requests.get(
+                url=self._url + "/accounts/" + str(account["_account_id"]) + "/sshkeys",
+                auth=(self._user, self._pass),
+            )
+        else:
+            response = requests.get(
+                url=self._url + "/accounts/" + str(account["_account_id"]) + "/sshkeys"
+            )
+        if response.status_code != requests.codes.ok:
+            Logger.error("failed to get sshkey for account %s" % account["_account_id"])
+            return None
+        return json.loads(response.text.replace(")]}'", ""))
+
     def get_detail(self, change):
         if len(self._pass) != 0 and len(self._user) != 0:
             response = requests.get(
                 url=self._url + "/changes/" + str(change["_number"]) + "/detail",
                 auth=(self._user, self._pass),
             )
         else:
@@ -266,7 +333,65 @@
         if response.status_code != requests.codes.ok:
             Logger.error(
                 "failed to submit change %s by account %s"
                 % (change["_number"], self._user)
             )
             return None
         return json.loads(response.text.replace(")]}'", ""))
+
+    def query_group(self, search, start):
+        def _helper(_search, _start):
+            payload = {
+                "o": self._GROUP_OPTION,
+                "query": _search,
+                "start": _start,
+                "limit": self._GROUP_LIMIT,
+            }
+            if len(self._pass) != 0 and len(self._user) != 0:
+                response = requests.get(
+                    url=self._url + "/groups/",
+                    auth=(self._user, self._pass),
+                    params=payload,
+                )
+            else:
+                response = requests.get(url=self._url + "/groups/", params=payload)
+            if response.status_code != requests.codes.ok:
+                Logger.error("failed to query group with search %s" % _search)
+                return None
+            return json.loads(response.text.replace(")]}'", ""))
+
+        buf = _helper(search, start)
+        if buf is None or len(buf) == 0:
+            return []
+        if buf[-1].get("_more_groups", False) is False:
+            return buf
+        buf.extend(self.query_group(search, start + len(buf)))
+        return buf
+
+    def query_project(self, search, start):
+        def _helper(_search, _start):
+            payload = {
+                "o": self._PROJECT_OPTION,
+                "query": _search,
+                "start": _start,
+                "limit": self._PROJECT_LIMIT,
+            }
+            if len(self._pass) != 0 and len(self._user) != 0:
+                response = requests.get(
+                    url=self._url + "/projects/",
+                    auth=(self._user, self._pass),
+                    params=payload,
+                )
+            else:
+                response = requests.get(url=self._url + "/projects/", params=payload)
+            if response.status_code != requests.codes.ok:
+                Logger.error("failed to query project with search %s" % _search)
+                return None
+            return json.loads(response.text.replace(")]}'", ""))
+
+        buf = _helper(search, start)
+        if buf is None or len(buf) == 0:
+            return []
+        if buf[-1].get("_more_projects", False) is False:
+            return buf
+        buf.extend(self.query_project(search, start + len(buf)))
+        return buf
```

### Comparing `gerritaction-1.3.0/gerritaction/logger/logger.py` & `gerritaction-1.4.0/gerritaction/logger/logger.py`

 * *Files identical despite different names*

### Comparing `gerritaction-1.3.0/gerritaction.egg-info/SOURCES.txt` & `gerritaction-1.4.0/gerritaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gerritaction-1.3.0/setup.py` & `gerritaction-1.4.0/setup.py`

 * *Files identical despite different names*

