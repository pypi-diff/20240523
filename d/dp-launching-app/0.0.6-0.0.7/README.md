# Comparing `tmp/dp-launching-app-0.0.6.tar.gz` & `tmp/dp-launching-app-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-launching-app-0.0.6.tar", last modified: Mon May 20 10:17:34 2024, max compression
+gzip compressed data, was "dp-launching-app-0.0.7.tar", last modified: Thu May 23 08:05:00 2024, max compression
```

## Comparing `dp-launching-app-0.0.6.tar` & `dp-launching-app-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.144948 dp-launching-app-0.0.6/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/MANIFEST.in
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-20 10:17:34.144800 dp-launching-app-0.0.6/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/README.md
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137121 dp-launching-app-0.0.6/dp/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137426 dp-launching-app-0.0.6/dp/launching/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.137724 dp-launching-app-0.0.6/dp/launching/cli/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    12682 2024-05-16 07:06:32.000000 dp-launching-app-0.0.6/dp/launching/cli/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.138725 dp-launching-app-0.0.6/dp/launching/cli/api/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/model.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/api/persistent_service.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139260 dp-launching-app-0.0.6/dp/launching/cli/commands/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/launching.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.135382 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139513 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/basic.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.139767 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140014 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/dflow.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140504 dp-launching-app-0.0.6/dp/launching/cli/utils/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/utils/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/cli/utils/random.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.140762 dp-launching-app-0.0.6/dp/launching/report/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/report/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.142812 dp-launching-app-0.0.6/dp/launching/typing/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/__init__.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.143476 dp-launching-app-0.0.6/dp/launching/typing/addon/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/__init__.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/sysmbol.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/addon/ui.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.6/dp/launching/typing/basic.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/benchmark.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/bio.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)    10526 2024-05-20 09:36:59.000000 dp-launching-app-0.0.6/dp/launching/typing/bohrium.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      944 2024-05-20 10:13:32.000000 dp-launching-app-0.0.6/dp/launching/typing/dataset.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/dflow.py
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.6/dp/launching/typing/io.py
-drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-20 10:17:34.144611 dp-launching-app-0.0.6/dp_launching_app.egg-info/
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/PKG-INFO
--rw-r--r--   0 xiongyanfei   (502) staff       (20)     1123 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/SOURCES.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/dependency_links.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-20 10:17:33.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/entry_points.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/requires.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-20 10:17:34.000000 dp-launching-app-0.0.6/dp_launching_app.egg-info/top_level.txt
--rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-20 10:17:34.144983 dp-launching-app-0.0.6/setup.cfg
--rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-20 10:17:23.000000 dp-launching-app-0.0.6/setup.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.521910 dp-launching-app-0.0.7/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       94 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/MANIFEST.in
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-23 08:05:00.521730 dp-launching-app-0.0.7/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/README.md
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.512064 dp-launching-app-0.0.7/dp/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      154 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.512652 dp-launching-app-0.0.7/dp/launching/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       22 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.513067 dp-launching-app-0.0.7/dp/launching/cli/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    12658 2024-05-23 08:02:43.000000 dp-launching-app-0.0.7/dp/launching/cli/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.513976 dp-launching-app-0.0.7/dp/launching/cli/api/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    21712 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/model.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     5386 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/api/persistent_service.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514431 dp-launching-app-0.0.7/dp/launching/cli/commands/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1315 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/launching.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.509291 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514700 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1858 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/basic.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.514964 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2595 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/bohrium.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.515350 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2606 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/dflow.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.515803 dp-launching-app-0.0.7/dp/launching/cli/utils/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/utils/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      147 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/cli/utils/random.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.516048 dp-launching-app-0.0.7/dp/launching/report/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     2940 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/report/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.519213 dp-launching-app-0.0.7/dp/launching/typing/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      175 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/__init__.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.520120 dp-launching-app-0.0.7/dp/launching/typing/addon/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        0 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/__init__.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      867 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/sysmbol.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6866 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/addon/ui.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     7379 2024-05-11 02:54:01.000000 dp-launching-app-0.0.7/dp/launching/typing/basic.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      749 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/benchmark.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1774 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/bio.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)    10526 2024-05-20 09:36:59.000000 dp-launching-app-0.0.7/dp/launching/typing/bohrium.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      944 2024-05-20 10:13:32.000000 dp-launching-app-0.0.7/dp/launching/typing/dataset.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     4908 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/dflow.py
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     6371 2024-05-10 07:03:20.000000 dp-launching-app-0.0.7/dp/launching/typing/io.py
+drwxr-xr-x   0 xiongyanfei   (502) staff       (20)        0 2024-05-23 08:05:00.521475 dp-launching-app-0.0.7/dp_launching_app.egg-info/
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      156 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/PKG-INFO
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)     1123 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/SOURCES.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        1 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/dependency_links.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       75 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/entry_points.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      108 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/requires.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)        3 2024-05-23 08:05:00.000000 dp-launching-app-0.0.7/dp_launching_app.egg-info/top_level.txt
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)       38 2024-05-23 08:05:00.521952 dp-launching-app-0.0.7/setup.cfg
+-rw-r--r--   0 xiongyanfei   (502) staff       (20)      714 2024-05-23 08:04:09.000000 dp-launching-app-0.0.7/setup.py
```

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/__init__.py` & `dp-launching-app-0.0.7/dp/launching/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,21 +225,21 @@
                 )
 
         return sys.exit(super().__call__(args))
 
     def gen_schema(self, output_path):
         try:
             if hasattr(self, "model"):
-                fileName = self.model.__name__ + "_inputs"
+                fileName = self.model.__name__
                 gen_model_schema(self.model, output_path, fileName, "single")
                 print(
                     f"JSONSchema describe file for {fileName} has been generated successfully to {output_path}/{fileName}.json"
                 )
             if hasattr(self, "outputOptions") and self.outputOptions is not None:
-                fileName = self.outputOptions.__name__ + "_inputs"
+                fileName = self.outputOptions.__name__
                 gen_model_schema(self.outputOptions, output_path, fileName, "single")
                 print(
                     f"JSONSchema describe file for {fileName} has been generated successfully to {output_path}/{fileName}.json"
                 )
             print(
                 f"Verify your schema at Dev Assistant https://launching.mlops.dp.tech/?request=GET%3A%2Fdeveloper_assistant"
             )
```

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/api/model.py` & `dp-launching-app-0.0.7/dp/launching/cli/api/model.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/api/persistent_service.py` & `dp-launching-app-0.0.7/dp/launching/cli/api/persistent_service.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/commands/launching.py` & `dp-launching-app-0.0.7/dp/launching/cli/commands/launching.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/basic/basic.py` & `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/basic/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/bohrium/bohrium.py` & `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/bohrium/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/cli/commands/scaffold/dflow/dflow.py` & `dp-launching-app-0.0.7/dp/launching/cli/commands/scaffold/dflow/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/report/__init__.py` & `dp-launching-app-0.0.7/dp/launching/report/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/addon/sysmbol.py` & `dp-launching-app-0.0.7/dp/launching/typing/addon/sysmbol.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/addon/ui.py` & `dp-launching-app-0.0.7/dp/launching/typing/addon/ui.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/basic.py` & `dp-launching-app-0.0.7/dp/launching/typing/basic.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/benchmark.py` & `dp-launching-app-0.0.7/dp/launching/typing/benchmark.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/bio.py` & `dp-launching-app-0.0.7/dp/launching/typing/bio.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/bohrium.py` & `dp-launching-app-0.0.7/dp/launching/typing/bohrium.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/dataset.py` & `dp-launching-app-0.0.7/dp/launching/typing/dataset.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/dflow.py` & `dp-launching-app-0.0.7/dp/launching/typing/dflow.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp/launching/typing/io.py` & `dp-launching-app-0.0.7/dp/launching/typing/io.py`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/dp_launching_app.egg-info/SOURCES.txt` & `dp-launching-app-0.0.7/dp_launching_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dp-launching-app-0.0.6/setup.py` & `dp-launching-app-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dp-launching-app",
-    version="0.0.6",
+    version="0.0.7",
     author="",
     author_email="",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     entry_points={
```

