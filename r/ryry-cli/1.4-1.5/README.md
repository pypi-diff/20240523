# Comparing `tmp/ryry_cli-1.4.tar.gz` & `tmp/ryry_cli-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-1.4.tar", last modified: Wed May 22 14:20:43 2024, max compression
+gzip compressed data, was "ryry_cli-1.5.tar", last modified: Thu May 23 10:59:44 2024, max compression
```

## Comparing `ryry_cli-1.4.tar` & `ryry_cli-1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 14:20:43.699370 ryry_cli-1.4/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.4/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-22 14:20:43.698372 ryry_cli-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 14:20:43.689858 ryry_cli-1.4/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.4/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-22 14:20:42.000000 ryry_cli-1.4/ryry/constant.py
--rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.4/ryry/main.py
--rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.4/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.4/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8082 2024-05-22 14:20:00.000000 ryry_cli-1.4/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14641 2024-05-22 14:20:36.000000 ryry_cli-1.4/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:20:43.691858 ryry_cli-1.4/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.4/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.4/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.4/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2447 2024-05-21 10:23:27.000000 ryry_cli-1.4/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.4/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.4/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.4/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-1.4/ryry/upload.py
--rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.4/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:20:43.698372 ryry_cli-1.4/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 14:20:43.000000 ryry_cli-1.4/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 14:20:43.699370 ryry_cli-1.4/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-22 14:20:36.000000 ryry_cli-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:59:44.051786 ryry_cli-1.5/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.5/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-23 10:59:44.051786 ryry_cli-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 10:59:44.041267 ryry_cli-1.5/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.5/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry/constant.py
+-rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.5/ryry/main.py
+-rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.5/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.5/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8210 2024-05-23 10:59:25.000000 ryry_cli-1.5/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    14641 2024-05-23 10:59:37.000000 ryry_cli-1.5/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:59:44.044268 ryry_cli-1.5/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.5/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.5/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.5/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2374 2024-05-23 10:53:41.000000 ryry_cli-1.5/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.5/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.5/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.5/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3934 2024-05-22 14:20:29.000000 ryry_cli-1.5/ryry/upload.py
+-rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.5/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:59:44.050787 ryry_cli-1.5/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-23 10:59:43.000000 ryry_cli-1.5/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:59:44.052787 ryry_cli-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-23 10:59:37.000000 ryry_cli-1.5/setup.py
```

### Comparing `ryry_cli-1.4/LICENSE` & `ryry_cli-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/PKG-INFO` & `ryry_cli-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.4
+Version: 1.5
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.4/README.md` & `ryry_cli-1.5/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/main.py` & `ryry_cli-1.5/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/ryry_server_socket.py` & `ryry_cli-1.5/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/ryry_service.py` & `ryry_cli-1.5/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/ryry_webapi.py` & `ryry_cli-1.5/ryry/ryry_webapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     try:
         requests.adapters.DEFAULT_RETRIES = 2
         s.keep_alive = False
         s.headers.update({'Connection':'close'})
         s.headers.update({'Usertoken':"0cce7cfe3629e16ee9b3ea8563305d3a15c524804da1861db07c2c867d79da63"})
         if len(files) <= 0:
             s.headers.update({'Content-Type':'application/json'})
-        res = s.post(url=f"https://api.dalipen.com/{func}", data=params, files=files, timeout=timeout, verify=False)
+            res = s.post(url=f"https://api.dalipen.com/{func}", json=params, timeout=timeout, verify=False)
+        else:
+            res = s.post(url=f"https://api.dalipen.com/{func}", data=params, files=files, timeout=timeout, verify=False)
         if res.status_code == 200:
             result_data = json.loads(res.content)
             res.close()
             if result_data["code"] == 0:
                 return 0, "", result_data["data"]
             else:
                 return result_data["code"], result_data["msg"], ""
```

### Comparing `ryry_cli-1.4/ryry/ryry_widget.py` & `ryry_cli-1.5/ryry/ryry_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "1.4"
+    data["version"] = "1.5"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
```

### Comparing `ryry_cli-1.4/ryry/script_template/main.py` & `ryry_cli-1.5/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/server_func.py` & `ryry_cli-1.5/ryry/server_func.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,12 +63,8 @@
     def call(self):
         for t in self.thread_data.keys():
             self.thread_data[t]["thread"].join()
         result = []
         for t in self.thread_data.keys():
             result.append(self.thread_data[t]["result"])
         return result
-    
-    
-results = Task("Demo", [{
-    "func": "你好"
-}], "").call()
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ryry_cli-1.4/ryry/store.py` & `ryry_cli-1.5/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/task.py` & `ryry_cli-1.5/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/taskUtils.py` & `ryry_cli-1.5/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/upload.py` & `ryry_cli-1.5/ryry/upload.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry/utils.py` & `ryry_cli-1.5/ryry/utils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-1.5/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.4
+Version: 1.5
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.4/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-1.5/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.4/setup.py` & `ryry_cli-1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "1.4"
+ryry_version = "1.5"
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
-app_version="1.4"
+app_version="1.5"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

