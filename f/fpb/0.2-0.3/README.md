# Comparing `tmp/fpb-0.2.tar.gz` & `tmp/fpb-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpb-0.2.tar", last modified: Thu May 23 03:53:41 2024, max compression
+gzip compressed data, was "fpb-0.3.tar", last modified: Thu May 23 04:03:23 2024, max compression
```

## Comparing `fpb-0.2.tar` & `fpb-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.596844 fpb-0.2/
--rw-rw-rw-   0        0        0      169 2024-05-23 03:53:41.595845 fpb-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.583849 fpb-0.2/fingerprint_browser/
--rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.2/fingerprint_browser/__init__.py
--rw-rw-rw-   0        0        0    17547 2024-05-23 03:47:41.000000 fpb-0.2/fingerprint_browser/hubstudio.py
--rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.2/fingerprint_browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:53:41.595845 fpb-0.2/fpb.egg-info/
--rw-rw-rw-   0        0        0      169 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 03:53:41.000000 fpb-0.2/fpb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 03:53:41.596844 fpb-0.2/setup.cfg
--rw-rw-rw-   0        0        0      278 2024-05-23 03:47:58.000000 fpb-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.751048 fpb-0.3/
+-rw-rw-rw-   0        0        0      169 2024-05-23 04:03:23.751048 fpb-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.747048 fpb-0.3/fingerprint_browser/
+-rw-rw-rw-   0        0        0       41 2024-05-04 22:20:38.000000 fpb-0.3/fingerprint_browser/__init__.py
+-rw-rw-rw-   0        0        0    17618 2024-05-23 03:58:14.000000 fpb-0.3/fingerprint_browser/hubstudio.py
+-rw-rw-rw-   0        0        0      299 2024-05-23 03:47:41.000000 fpb-0.3/fingerprint_browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 04:03:23.750048 fpb-0.3/fpb.egg-info/
+-rw-rw-rw-   0        0        0      169 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 04:03:23.000000 fpb-0.3/fpb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 04:03:23.751048 fpb-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      278 2024-05-23 03:57:26.000000 fpb-0.3/setup.py
```

### Comparing `fpb-0.2/fingerprint_browser/hubstudio.py` & `fpb-0.3/fingerprint_browser/hubstudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,25 @@
             f"--timeout={timeout}",
             f"--threads={threads}",
         ]
         if remote_debugging:
             cmds.append("--remote_debugging")
         if line_setting:
             cmds.append(f"--line_setting={line_setting}")
-
+        utils.terminate_process_by_name("hubstudio_connector.exe")
         p = await asyncio.create_subprocess_exec(
             os.path.join(client_path, "hubstudio_connector.exe"),
             *cmds,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             creationflags=subprocess.CREATE_NO_WINDOW,
         )
 
         def on_exit():
-            p.kill()
+            p.terminate()
             utils.terminate_process_by_name("hubstudio_connector.exe")
 
         atexit.register(on_exit)
 
         while True:
             output_line = await p.stdout.readline()
             output_line = output_line.decode().strip()
```

