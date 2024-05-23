# Comparing `tmp/watch_run-0.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/watch_run-0.0.5-cp39-cp39-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 423880 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  1041408 b- defN 24-May-23 09:08 watch_run.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1222 b- defN 24-May-23 09:08 watch_run-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-23 09:08 watch_run-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       46 b- defN 24-May-23 09:08 watch_run-0.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 24-May-23 09:08 watch_run-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      492 b- defN 24-May-23 09:08 watch_run-0.0.3.dist-info/RECORD
-6 files, 1043278 bytes uncompressed, 422990 bytes compressed:  59.5%
+Zip file size: 2085004 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx  2948568 b- defN 24-May-23 06:29 run_py.cpython-39-darwin.so
+-rwxr-xr-x  2.0 unx  2949979 b- defN 24-May-23 11:17 watch_run.cpython-39-darwin.so
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-23 11:23 watch_run-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-May-23 11:23 watch_run-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-May-23 11:23 watch_run-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-23 11:23 watch_run-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      581 b- defN 24-May-23 11:23 watch_run-0.0.5.dist-info/RECORD
+7 files, 5900474 bytes uncompressed, 2083980 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: watch_run.cp39-win_amd64.pyd
+Filename: run_py.cpython-39-darwin.so
 Comment: 
 
-Filename: watch_run-0.0.3.dist-info/METADATA
+Filename: watch_run.cpython-39-darwin.so
 Comment: 
 
-Filename: watch_run-0.0.3.dist-info/WHEEL
+Filename: watch_run-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: watch_run-0.0.3.dist-info/entry_points.txt
+Filename: watch_run-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: watch_run-0.0.3.dist-info/top_level.txt
+Filename: watch_run-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: watch_run-0.0.3.dist-info/RECORD
+Filename: watch_run-0.0.5.dist-info/top_level.txt
+Comment: 
+
+Filename: watch_run-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `watch_run-0.0.3.dist-info/METADATA` & `watch_run-0.0.5.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: watch-run
-Version: 0.0.3
-Summary: watch_run project
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
-# My watch_run Project
-
-This is a plugin only for Python that enables easy monitoring of parameter changes without needing to modify the source code.
-
-What is particularly noteworthy is that it allows for monitoring of parameter changes through class objects in a production environment without affecting the runtime speed(just like print). 
-
-It is especially useful for streamlining the execution process and monitoring for bugs in a production environment.
-
-Run 'watch_run main.py' in the same place where you previously run 'python3 main.py'. This is the only command.
-
-## Installation
-
-```sh
-pip install watch_run
-```
-
-## Usage
-
-```sh
-watch_run main.py
-```
-
-## Features
-
-Monitor Ordinary Variables: Free of charge. Provides monitoring at 10-15 times the normal runtime speed.
-
-Monitor through Class Objects: Paid feature. Enables monitoring in a production environment without impacting performance.
-You can purchase this feature through the application interface.
-
-It prints the call stack.
-
-
-
-
-
-
+Metadata-Version: 2.1
+Name: watch-run
+Version: 0.0.5
+Summary: watch_run project
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+# My watch_run Project
+
+This is a plugin only for Python that enables easy monitoring of parameter changes without needing to modify the source code.
+
+What is particularly noteworthy is that it allows for monitoring of parameter changes through class objects in a production environment without affecting the runtime speed(just like print). 
+
+It is especially useful for streamlining the execution process and monitoring for bugs in a production environment.
+
+Run 'watch_run main.py' in the same place where you previously run 'python3 main.py'. This is the only command.
+
+## Installation
+
+```sh
+pip install watch_run
+```
+
+## Usage
+
+```sh
+watch_run main.py
+```
+
+## Features
+
+Monitor Ordinary Variables: Free of charge. Provides monitoring at 10-15 times the normal runtime speed.
+
+Monitor through Class Objects: Paid feature. Enables monitoring in a production environment without impacting performance.
+You can purchase this feature through the application interface.
+
+It prints the call stack.
+
+
+
+
+
+
```

