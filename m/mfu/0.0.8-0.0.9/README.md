# Comparing `tmp/mfu-0.0.8.tar.gz` & `tmp/mfu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfu-0.0.8.tar", last modified: Fri May 17 08:53:45 2024, max compression
+gzip compressed data, was "mfu-0.0.9.tar", last modified: Fri May 17 09:06:04 2024, max compression
```

## Comparing `mfu-0.0.8.tar` & `mfu-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/
--rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 08:53:45.038613 mfu-0.0.8/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      508 2024-05-17 08:53:33.000000 mfu-0.0.8/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.034613 mfu-0.0.8/mfu/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.8/mfu/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.8/mfu/__main__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.8/mfu/main.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu/scripts/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.8/mfu/scripts/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.8/mfu/scripts/cluster.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.8/mfu/scripts/config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.8/mfu/scripts/doctor.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3709 2024-05-17 08:49:07.000000 mfu-0.0.8/mfu/scripts/sync.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu/utils/
--rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.8/mfu/utils/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.8/mfu/utils/forcelink.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.8/mfu/utils/general.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:53:45.038613 mfu-0.0.8/mfu.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/PKG-INFO
--rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/SOURCES.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/dependency_links.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/entry_points.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      104 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/requires.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:53:45.000000 mfu-0.0.8/mfu.egg-info/top_level.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      516 2024-05-17 08:53:42.000000 mfu-0.0.8/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:53:45.038613 mfu-0.0.8/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.8/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 09:06:04.282274 mfu-0.0.9/
+-rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 09:06:04.282274 mfu-0.0.9/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      508 2024-05-17 08:53:33.000000 mfu-0.0.9/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 09:06:04.282274 mfu-0.0.9/mfu/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.9/mfu/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.9/mfu/__main__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.9/mfu/main.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 09:06:04.282274 mfu-0.0.9/mfu/scripts/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.9/mfu/scripts/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.9/mfu/scripts/cluster.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.9/mfu/scripts/config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.9/mfu/scripts/doctor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3706 2024-05-17 09:05:42.000000 mfu-0.0.9/mfu/scripts/sync.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 09:06:04.282274 mfu-0.0.9/mfu/utils/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.9/mfu/utils/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.9/mfu/utils/forcelink.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.9/mfu/utils/general.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 09:06:04.282274 mfu-0.0.9/mfu.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)      895 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/PKG-INFO
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/entry_points.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      104 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/requires.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 09:06:04.000000 mfu-0.0.9/mfu.egg-info/top_level.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      516 2024-05-17 09:06:00.000000 mfu-0.0.9/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 09:06:04.282274 mfu-0.0.9/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.9/setup.py
```

### Comparing `mfu-0.0.8/PKG-INFO` & `mfu-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
```

### Comparing `mfu-0.0.8/mfu/scripts/cluster.py` & `mfu-0.0.9/mfu/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.8/mfu/scripts/config.py` & `mfu-0.0.9/mfu/scripts/config.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.8/mfu/scripts/doctor.py` & `mfu-0.0.9/mfu/scripts/doctor.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.8/mfu/scripts/sync.py` & `mfu-0.0.9/mfu/scripts/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     command_list = command.split(" ")
                     if run_command(command_list) == 0:
                         click.echo(
                             f"Synced: {event.src_path} to {pod_name}:{podroot}{event.src_path.replace(f'{self.project_path}/WebContent', '')}")
                 else:
                     click.echo(click.style('No pods were found', fg='red'))
                     click.echo(click.style(f'Search Details:', fg='red'))
-                    click.echo(click.style(f'- Namespace: forcelink-{branch_name}', fg='red'))
+                    click.echo(click.style(f'- Namespace: acumen-{branch_name}', fg='red'))
                     click.echo(click.style(f'- Pod Label: {podlabel}', fg='red'))
 
     click.echo(f'Starting to listen on: {path}')
     repo = Repo(path)
     branch_name = f"{repo.active_branch}"
     event_handler = Handler(path, branch_name)
     observer = Observer()
```

### Comparing `mfu-0.0.8/mfu/utils/forcelink.py` & `mfu-0.0.9/mfu/utils/forcelink.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.8/mfu/utils/general.py` & `mfu-0.0.9/mfu/utils/general.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.8/mfu.egg-info/PKG-INFO` & `mfu-0.0.9/mfu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.8
+Version: 0.0.9
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
```

### Comparing `mfu-0.0.8/pyproject.toml` & `mfu-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mfu"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Michael Botha", email="michael@408.co.za" },
 ]
 description = "Michael's fun utilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

