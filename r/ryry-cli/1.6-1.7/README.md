# Comparing `tmp/ryry_cli-1.6.tar.gz` & `tmp/ryry_cli-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-1.6.tar", last modified: Thu May 23 11:10:48 2024, max compression
+gzip compressed data, was "ryry_cli-1.7.tar", last modified: Thu May 23 11:12:07 2024, max compression
```

## Comparing `ryry_cli-1.6.tar` & `ryry_cli-1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:10:48.220596 ryry_cli-1.6/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.6/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-23 11:10:48.219091 ryry_cli-1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:10:48.210584 ryry_cli-1.6/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.6/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-23 11:10:47.000000 ryry_cli-1.6/ryry/constant.py
--rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.6/ryry/main.py
--rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.6/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.6/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8267 2024-05-23 11:10:31.000000 ryry_cli-1.6/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14641 2024-05-23 11:10:41.000000 ryry_cli-1.6/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:10:48.213584 ryry_cli-1.6/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.6/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.6/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.6/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2374 2024-05-23 10:53:41.000000 ryry_cli-1.6/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.6/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.6/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.6/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-1.6/ryry/upload.py
--rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.6/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:10:48.218095 ryry_cli-1.6/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-23 11:10:48.000000 ryry_cli-1.6/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:10:48.220596 ryry_cli-1.6/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-23 11:10:43.000000 ryry_cli-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:12:07.784284 ryry_cli-1.7/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.7/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-23 11:12:07.783286 ryry_cli-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:12:07.774207 ryry_cli-1.7/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.7/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-23 11:12:06.000000 ryry_cli-1.7/ryry/constant.py
+-rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.7/ryry/main.py
+-rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.7/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.7/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8210 2024-05-23 11:11:51.000000 ryry_cli-1.7/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    14641 2024-05-23 11:11:53.000000 ryry_cli-1.7/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:12:07.776208 ryry_cli-1.7/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.7/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.7/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.7/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2374 2024-05-23 10:53:41.000000 ryry_cli-1.7/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.7/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.7/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.7/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-1.7/ryry/upload.py
+-rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.7/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:12:07.782284 ryry_cli-1.7/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 11:12:07.000000 ryry_cli-1.7/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:12:07.784284 ryry_cli-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-23 11:11:53.000000 ryry_cli-1.7/setup.py
```

### Comparing `ryry_cli-1.6/LICENSE` & `ryry_cli-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/PKG-INFO` & `ryry_cli-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.6
+Version: 1.7
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.6/README.md` & `ryry_cli-1.7/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/main.py` & `ryry_cli-1.7/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/ryry_server_socket.py` & `ryry_cli-1.7/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/ryry_service.py` & `ryry_cli-1.7/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/ryry_webapi.py` & `ryry_cli-1.7/ryry/ryry_webapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,10 +245,8 @@
     if r1 != 0:
         return False, False, "server fail"
     if r3["status"] < 2:
         return False, False, ""
     elif r3["status"] == 2:
         return True, True, json.loads(r3["task_result"])
     elif r3["status"] == 3:
-        return True, False, r3["fail_reason"]
-    
-checkTask("4d889820-f85c-4824-885e-5c659cc280f9")
+        return True, False, r3["fail_reason"]
```

### Comparing `ryry_cli-1.6/ryry/ryry_widget.py` & `ryry_cli-1.7/ryry/ryry_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "1.6"
+    data["version"] = "1.7"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
```

### Comparing `ryry_cli-1.6/ryry/script_template/main.py` & `ryry_cli-1.7/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/server_func.py` & `ryry_cli-1.7/ryry/server_func.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/store.py` & `ryry_cli-1.7/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/task.py` & `ryry_cli-1.7/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/taskUtils.py` & `ryry_cli-1.7/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/upload.py` & `ryry_cli-1.7/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry/utils.py` & `ryry_cli-1.7/ryry/utils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-1.7/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.6
+Version: 1.7
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.6/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-1.7/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.6/setup.py` & `ryry_cli-1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "1.6"
+ryry_version = "1.7"
 ryry_build_number = int(ryry_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "ryry", "constant.py")
 try:
     # result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     # if result.returncode == 0:
@@ -20,15 +20,15 @@
 app_bulld_number={ryry_build_number}
 app_bulld_anchor="{build_user}_{build_pts}"
 app_name="ryry-cli"
 ''')
 except:
     with open(constanspy, 'w') as f:
         f.write(f'''#!!!!! do not change this file !!!!!
-app_version="1.6"
+app_version="1.7"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```
