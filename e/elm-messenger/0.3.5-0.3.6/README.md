# Comparing `tmp/elm_messenger-0.3.5.tar.gz` & `tmp/elm_messenger-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_messenger-0.3.5.tar", last modified: Thu May 16 16:19:24 2024, max compression
+gzip compressed data, was "elm_messenger-0.3.6.tar", last modified: Thu May 23 02:26:18 2024, max compression
```

## Comparing `elm_messenger-0.3.5.tar` & `elm_messenger-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-16 16:19:24.900945 elm_messenger-0.3.5/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.5/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-16 16:19:24.900945 elm_messenger-0.3.5/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      888 2024-05-15 03:21:04.000000 elm_messenger-0.3.5/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-16 16:19:24.900945 elm_messenger-0.3.5/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-16 16:19:24.000000 elm_messenger-0.3.5/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-16 16:19:24.900945 elm_messenger-0.3.5/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.5/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.5/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16638 2024-05-16 16:16:18.000000 elm_messenger-0.3.5/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1090 2024-05-15 18:35:42.000000 elm_messenger-0.3.5/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2024-05-16 16:19:24.900945 elm_messenger-0.3.5/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.5/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      888 2024-05-15 03:21:04.000000 elm_messenger-0.3.6/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16639 2024-05-23 02:21:06.000000 elm_messenger-0.3.6/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1090 2024-05-15 18:35:42.000000 elm_messenger-0.3.6/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2024-05-23 02:26:18.950249 elm_messenger-0.3.6/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/setup.py
```

### Comparing `elm_messenger-0.3.5/PKG-INFO` & `elm_messenger-0.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.5
+Version: 0.3.6
 Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm_messenger-0.3.5/Readme.md` & `elm_messenger-0.3.6/Readme.md`

 * *Files identical despite different names*

### Comparing `elm_messenger-0.3.5/elm_messenger.egg-info/PKG-INFO` & `elm_messenger-0.3.6/elm_messenger.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.5
+Version: 0.3.6
 Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `elm_messenger-0.3.5/messengercli/messenger.py` & `elm_messenger-0.3.6/messengercli/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
 def component(
     scene: str,
     name: str,
     compdir: str = typer.Option(
         "Components", "--cdir", "-cd", help="Directory to store components"
     ),
     is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create layer in sceneproto"
+        False, "--proto", "-p", help="Create a component in sceneproto"
     ),
     init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
 ):
     name = check_name(name)
     scene = check_name(scene)
     compdir = check_name(compdir)
     msg = Messenger()
@@ -412,15 +412,15 @@
 
 
 @app.command()
 def scene(
     name: str,
     raw: bool = typer.Option(False, "--raw", help="Use raw scene without layers"),
     is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create layer in sceneproto"
+        False, "--proto", "-p", help="Create a sceneproto"
     ),
     init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
 ):
     name = check_name(name)
     msg = Messenger()
     input(
         f"You are going to create a {'raw ' if raw else ''}{'sceneproto' if is_proto else 'scene'} named {name}, continue?"
@@ -452,15 +452,15 @@
     has_component: bool = typer.Option(
         False, "--with-component", "-c", help="Use components in this layer"
     ),
     compdir: str = typer.Option(
         "Components", "--cdir", "-cd", help="Directory of components in the scene"
     ),
     is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create layer in sceneproto"
+        False, "--proto", "-p", help="Create a layer in sceneproto"
     ),
     init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
 ):
     scene = check_name(scene)
     layer = check_name(layer)
     msg = Messenger()
     input(
```

### Comparing `elm_messenger-0.3.5/messengercli/updater.py` & `elm_messenger-0.3.6/messengercli/updater.py`

 * *Files identical despite different names*

