# Comparing `tmp/chess_pairings-0.1.5.tar.gz` & `tmp/chess_pairings-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_pairings-0.1.5.tar", last modified: Sun May 19 09:46:31 2024, max compression
+gzip compressed data, was "chess_pairings-0.1.6.tar", last modified: Thu May 23 17:16:12 2024, max compression
```

## Comparing `chess_pairings-0.1.5.tar` & `chess_pairings-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-19 09:46:27.000000 chess_pairings-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.243346 chess_pairings-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/src/chess_pairings/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      463 2024-05-19 09:09:22.000000 chess_pairings-0.1.5/src/chess_pairings/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-05-19 09:08:59.000000 chess_pairings-0.1.5/src/chess_pairings/_classify.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/src/chess_pairings/chess_results/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/_donwload.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/errors.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-05-02 17:54:54.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4013 2024-05-11 16:42:20.000000 chess_pairings-0.1.5/src/chess_pairings/chess_results/parsing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/src/chess_pairings/types/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-19 08:19:56.000000 chess_pairings-0.1.5/src/chess_pairings/types/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-05-19 09:06:42.000000 chess_pairings-0.1.5/src/chess_pairings/types/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-05-19 09:18:03.000000 chess_pairings-0.1.5/src/chess_pairings/types/ids.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2590 2024-05-19 09:26:58.000000 chess_pairings-0.1.5/src/chess_pairings/types/mapping.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-05-11 16:42:02.000000 chess_pairings-0.1.5/src/chess_pairings/types/pairings.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-19 09:46:31.253346 chess_pairings-0.1.5/src/chess_pairings.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-19 09:46:31.000000 chess_pairings-0.1.5/src/chess_pairings.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-05-19 09:46:31.000000 chess_pairings-0.1.5/src/chess_pairings.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-19 09:46:31.000000 chess_pairings-0.1.5/src/chess_pairings.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-05-19 09:46:31.000000 chess_pairings-0.1.5/src/chess_pairings.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-19 09:46:31.000000 chess_pairings-0.1.5/src/chess_pairings.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-23 17:16:08.000000 chess_pairings-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.329748 chess_pairings-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.329748 chess_pairings-0.1.6/src/chess_pairings/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      491 2024-05-20 06:44:12.000000 chess_pairings-0.1.6/src/chess_pairings/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-05-19 09:08:59.000000 chess_pairings-0.1.6/src/chess_pairings/_classify.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings/chess_results/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      531 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2347 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/_donwload.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      357 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/errors.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      274 2024-05-02 17:54:54.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4013 2024-05-11 16:42:20.000000 chess_pairings-0.1.6/src/chess_pairings/chess_results/parsing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings/types/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-19 08:19:56.000000 chess_pairings-0.1.6/src/chess_pairings/types/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      432 2024-05-20 06:43:53.000000 chess_pairings-0.1.6/src/chess_pairings/types/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      657 2024-05-20 06:43:41.000000 chess_pairings-0.1.6/src/chess_pairings/types/ids.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2590 2024-05-19 09:26:58.000000 chess_pairings-0.1.6/src/chess_pairings/types/mapping.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      718 2024-05-11 16:42:02.000000 chess_pairings-0.1.6/src/chess_pairings/types/pairings.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-23 17:16:12.339748 chess_pairings-0.1.6/src/chess_pairings.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      535 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      773 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       49 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-05-23 17:16:12.000000 chess_pairings-0.1.6/src/chess_pairings.egg-info/top_level.txt
```

### Comparing `chess_pairings-0.1.5/PKG-INFO` & `chess_pairings-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
```

### Comparing `chess_pairings-0.1.5/pyproject.toml` & `chess_pairings-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-pairings"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Tools for storing and fetching chess tournament pairings"
 dependencies = [
   "pydantic"
 ]
```

### Comparing `chess_pairings-0.1.5/src/chess_pairings/_classify.py` & `chess_pairings-0.1.6/src/chess_pairings/_classify.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings/chess_results/__init__.pyi` & `chess_pairings-0.1.6/src/chess_pairings/chess_results/__init__.pyi`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings/chess_results/_donwload.py` & `chess_pairings-0.1.6/src/chess_pairings/chess_results/_donwload.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings/chess_results/parsing.py` & `chess_pairings-0.1.6/src/chess_pairings/chess_results/parsing.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings/types/ids.py` & `chess_pairings-0.1.6/src/chess_pairings/types/ids.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 
 class GameId(RoundId):
   board: str
 
 def gameId(tournId: str, group: str, round: str, board: str) -> GameId:
   return GameId(tournId=tournId, group=group, round=round, board=board)
 
+def stringifyId(tournId: str, group: str, round: str, board: str) -> str:
+  return f'{tournId}/{group}/{round}/{board}'
+
 def roundId(tournId: str, group: str, round: str) -> RoundId:
   return RoundId(tournId=tournId, group=group, round=round)
 
 def groupId(tournId: str, group: str) -> GroupId:
   return GroupId(tournId=tournId, group=group)
```

### Comparing `chess_pairings-0.1.5/src/chess_pairings/types/mapping.py` & `chess_pairings-0.1.6/src/chess_pairings/types/mapping.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings/types/pairings.py` & `chess_pairings-0.1.6/src/chess_pairings/types/pairings.py`

 * *Files identical despite different names*

### Comparing `chess_pairings-0.1.5/src/chess_pairings.egg-info/PKG-INFO` & `chess_pairings-0.1.6/src/chess_pairings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess-pairings
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tools for storing and fetching chess tournament pairings
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/chess.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Provides-Extra: chess-results
```

### Comparing `chess_pairings-0.1.5/src/chess_pairings.egg-info/SOURCES.txt` & `chess_pairings-0.1.6/src/chess_pairings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

