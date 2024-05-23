# Comparing `tmp/eurmlsdk-0.1.203.tar.gz` & `tmp/eurmlsdk-0.1.205.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.203.tar", last modified: Fri May 17 13:00:26 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.205.tar", last modified: Thu May 23 08:43:17 2024, max compression
```

## Comparing `eurmlsdk-0.1.203.tar` & `eurmlsdk-0.1.205.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 13:00:26.252549 eurmlsdk-0.1.203/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.203/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.203/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 13:00:26.252549 eurmlsdk-0.1.203/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       10 2024-05-07 10:55:35.000000 eurmlsdk-0.1.203/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 13:00:26.252549 eurmlsdk-0.1.203/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.203/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6150 2024-05-16 10:16:43.000000 eurmlsdk-0.1.203/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9571 2024-05-17 11:59:06.000000 eurmlsdk-0.1.203/eurmlsdk/eur_sdk.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.203/eurmlsdk/pytorch.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1209 2024-05-17 13:00:02.000000 eurmlsdk-0.1.203/eurmlsdk/yolo.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-17 13:00:26.252549 eurmlsdk-0.1.203/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      384 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      335 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       53 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      130 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-17 13:00:26.000000 eurmlsdk-0.1.203/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-17 13:00:26.252549 eurmlsdk-0.1.203/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      897 2024-05-17 13:00:09.000000 eurmlsdk-0.1.203/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.205/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.205/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      665 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:05.000000 eurmlsdk-0.1.205/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.205/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6424 2024-05-21 10:12:39.000000 eurmlsdk-0.1.205/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9564 2024-05-23 08:15:17.000000 eurmlsdk-0.1.205/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1441 2024-05-23 07:55:38.000000 eurmlsdk-0.1.205/eurmlsdk/hello.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      312 2024-05-23 07:57:34.000000 eurmlsdk-0.1.205/eurmlsdk/pt.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.205/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1508 2024-05-23 08:18:45.000000 eurmlsdk-0.1.205/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      665 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      368 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       52 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      136 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      914 2024-05-23 08:41:21.000000 eurmlsdk-0.1.205/setup.py
```

### Comparing `eurmlsdk-0.1.203/eurmlsdk/__main__.py` & `eurmlsdk-0.1.205/eurmlsdk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
     print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
     print(" <username>     : Remote Server username")
 
 def main():
-    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
+    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate' ,'visualize']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
             print("Version: 0.0.902")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
@@ -78,14 +78,22 @@
                 print("Too many arguments")
                 print("Usage: eurmlsdk predict <model path> <dataset path>")
                 exit(1)
             modelPath = argv[2]
             predictData = argv[3]
             yoloSDK = ModelYolo()
             yoloSDK.predict_model(modelPath, predictData)
+            
+        elif command == "visualize":
+            if argLen < 3:
+                print("Missing model file argument")
+                exit(1)
+            modelPath = argv[2]
+            yoloSDK = ModelYolo()
+            yoloSDK.visualize(modelPath)
 
         elif command == "pt-predict":
             if argLen <3 :
                 print("Missing required arguments")
                 print("<model_path> <dataset_path>")
                 exit(1)
             else:
```

### Comparing `eurmlsdk-0.1.203/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.205/eurmlsdk/eur_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     #         return super().get(remotepath, localpath, callback=_callback, confirm=confirm)
         
 class EurBaseSDK():
     def get_model(self, filepath) ->str:
         extension = filepath.split(".")
         if extension[1] != "pt" and extension[1] != "tflite":
             print("Not supported file path")
-            return ""
+            return ""  
         
         if os.path.exists(filepath):
             print("Model file exist and ready to load")
             return filepath        
         else: 
             print("Model file is not available in the given path")
             return ""
@@ -144,15 +144,15 @@
                 return op
             if err:
                 print(err)
                 return ""
         except Exception as err:
             print("Error Executing the script: ", err)
             exit(1)
-            
+
     def deploy_pytorch_model(self, scriptFile, modelFile, hostname, username, password):
         ssh_client = self.connect_ssh_client(hostname, username, password)
         home_path = self.execute_ssh_script(ssh_client, 'pwd')
         if home_path == "":
             exit(1)
         script_path = (f'{home_path}/{scriptFile}').replace('\n', "").strip()
         script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile}'
@@ -202,8 +202,8 @@
         # download prediction results to local
         predict_path = "/runs/detect"
         download_to = os.getcwd() + "/"
         download_from = (f"{home_path}{predict_path}").replace('\n', "").strip()
         # self.download_file(ssh_client, '', os.getcwd(), home_path + '/runs/detect/')
         self.download_file(ssh_client, download_to, download_from)
         ssh_client.close()
-        exit()
+        exit()
```

### Comparing `eurmlsdk-0.1.203/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.205/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.203/setup.py` & `eurmlsdk-0.1.205/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.203',
+    version='0.1.205',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
@@ -15,14 +15,15 @@
         'tqdm',
         'ultralytics',
         'torch',
         'timm',
         'torchvision',
         'menpo',
         'opencv-contrib-python'    
+        'netron'
 ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
             "eurmlsdk = eurmlsdk.__main__:main"
```

