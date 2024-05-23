# Comparing `tmp/mlab.py-0.4.0.tar.gz` & `tmp/mlab_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab.py-0.4.0.tar", last modified: Wed May 22 23:58:12 2024, max compression
+gzip compressed data, was "mlab_py-0.4.1.tar", max compression
```

## Comparing `mlab.py-0.4.0.tar` & `mlab_py-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:58:12.224710 mlab.py-0.4.0/
--rw-r--r--   0 disal      (501) staff       (20)      563 2024-05-22 23:58:12.224098 mlab.py-0.4.0/PKG-INFO
--rw-r--r--   0 disal      (501) staff       (20)        8 2024-05-22 22:06:07.000000 mlab.py-0.4.0/README.md
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:58:12.220625 mlab.py-0.4.0/mlab.py.egg-info/
--rw-r--r--   0 disal      (501) staff       (20)      563 2024-05-22 23:58:12.000000 mlab.py-0.4.0/mlab.py.egg-info/PKG-INFO
--rw-r--r--   0 disal      (501) staff       (20)      229 2024-05-22 23:58:12.000000 mlab.py-0.4.0/mlab.py.egg-info/SOURCES.txt
--rw-r--r--   0 disal      (501) staff       (20)        1 2024-05-22 23:58:12.000000 mlab.py-0.4.0/mlab.py.egg-info/dependency_links.txt
--rw-r--r--   0 disal      (501) staff       (20)        7 2024-05-22 23:58:12.000000 mlab.py-0.4.0/mlab.py.egg-info/top_level.txt
-drwxr-xr-x   0 disal      (501) staff       (20)        0 2024-05-22 23:58:12.223334 mlab.py-0.4.0/pymlab/
--rw-r--r--   0 disal      (501) staff       (20)      183 2024-05-22 23:41:07.000000 mlab.py-0.4.0/pymlab/__init__.py
--rw-r--r--   0 disal      (501) staff       (20)     2628 2024-05-22 23:41:33.000000 mlab.py-0.4.0/pymlab/m_test.py
--rw-r--r--   0 disal      (501) staff       (20)     2426 2024-05-22 23:42:11.000000 mlab.py-0.4.0/pymlab/m_train.py
--rw-r--r--   0 disal      (501) staff       (20)     2291 2024-05-22 23:00:18.000000 mlab.py-0.4.0/pymlab/m_utils.py
--rw-r--r--   0 disal      (501) staff       (20)      317 2024-05-22 23:56:13.000000 mlab.py-0.4.0/pyproject.toml
--rw-r--r--   0 disal      (501) staff       (20)       38 2024-05-22 23:58:12.224847 mlab.py-0.4.0/setup.cfg
--rw-r--r--   0 disal      (501) staff       (20)     1108 2024-05-22 23:58:03.000000 mlab.py-0.4.0/setup.py
+-rw-r--r--   0        0        0        8 2024-05-22 22:06:07.525956 mlab_py-0.4.1/README.md
+-rw-r--r--   0        0        0      183 2024-05-22 23:41:07.584992 mlab_py-0.4.1/pymlab/__init__.py
+-rw-r--r--   0        0        0     2628 2024-05-22 23:41:33.152267 mlab_py-0.4.1/pymlab/m_test.py
+-rw-r--r--   0        0        0     2579 2024-05-23 07:44:35.413735 mlab_py-0.4.1/pymlab/m_train.py
+-rw-r--r--   0        0        0     2337 2024-05-23 07:44:20.219924 mlab_py-0.4.1/pymlab/m_utils.py
+-rw-r--r--   0        0        0      372 2024-05-23 07:45:07.768539 mlab_py-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 mlab_py-0.4.1/PKG-INFO
```

### Comparing `mlab.py-0.4.0/pymlab/m_test.py` & `mlab_py-0.4.1/pymlab/m_test.py`

 * *Files identical despite different names*

### Comparing `mlab.py-0.4.0/pymlab/m_train.py` & `mlab_py-0.4.1/pymlab/m_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,38 +22,41 @@
     and will return the results of training.
     """
 
     parameters = fetch_parameters(config_path=f"{model_path}/config.txt")
     DATASET_PATH = str(parameters["dataset_url"]).strip() # type: ignore
 
     train_model = getattr(__import__(f"{model_path}.model", fromlist=["train"]), "train")
+    print(train_model)
 
     try:
         async def main():
+            print("Training model")
             model: TrainResults = train_model(dataset_path=DATASET_PATH, parameters=parameters, result_id=result_id)
+            print(model)
             files = {}
 
             for file in model.files:
                 filename = file.name
                 files[filename] = file
 
             # Stringify metrics
             metrics = json.dumps(model.metrics)
             data = {
                 "result_id": result_id,
                 "metrics": metrics,
                 "pretrained_model": model.pretrained_model,
             }
 
-
+            print("Uploading results")
             response = requests.post(API_URL, data=data, files=files,timeout=120, verify=False)
 
             if response.status_code != 200:
                 raise requests.HTTPError(f"Error uploading results. Status code: {response.status_code}, error: {response.text}")
-
+        print("Running in dir")
         run_in_dir(model_path, [f"source {model_path}/venv/bin/activate", f"python -m asyncio.run {main()}"])
     except Exception as e:
         # Append error in error.txt file
         # First check if error.txt file exists
         if not os.path.exists(f"{result_id}/error.txt"):
             os.mkdir(result_id)
             with open(f"{result_id}/error.txt", "w", encoding="utf-8") as f:
```

### Comparing `mlab.py-0.4.0/pymlab/m_utils.py` & `mlab_py-0.4.1/pymlab/m_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+import subprocess
 
 def parse_list(value):
     # Check if the value is a list
     if value.startswith('[') and value.endswith(']'):
         # Remove brackets
         value = value[1:-1]
         result = []
@@ -63,8 +63,8 @@
                         parameters[param_name] = str(param_value)
 
     return parameters
 
 def run_in_dir(directory: str, commands: list[str]) -> None:
     os.chdir(directory)
     for command in commands:
-        os.system(command)
+        subprocess.run(command, shell=True, check=True)
```

