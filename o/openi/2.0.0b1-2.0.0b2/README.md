# Comparing `tmp/openi-2.0.0b1.tar.gz` & `tmp/openi-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-2.0.0b1.tar", last modified: Thu May 23 03:18:08 2024, max compression
+gzip compressed data, was "openi-2.0.0b2.tar", last modified: Thu May 23 06:51:20 2024, max compression
```

## Comparing `openi-2.0.0b1.tar` & `openi-2.0.0b2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.158169 openi-2.0.0b1/
--rw-rw-rw-   0        0        0     2102 2024-05-23 03:18:08.156168 openi-2.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b1/README.md
--rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 03:18:08.159165 openi-2.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     1005 2024-05-22 07:31:03.000000 openi-2.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.045983 openi-2.0.0b1/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.106352 openi-2.0.0b1/src/openi/
--rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/__init__.py
--rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b1/src/openi/_dataclass.py
--rw-rw-rw-   0        0        0     7945 2024-05-22 02:53:31.000000 openi-2.0.0b1/src/openi/_exceptions.py
--rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b1/src/openi/_file.py
--rw-rw-rw-   0        0        0     4576 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/_login.py
--rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b1/src/openi/_session.py
--rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/_tqdm.py
--rw-rw-rw-   0        0        0    36678 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.133064 openi-2.0.0b1/src/openi/commands/
--rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/commands/__init__.py
--rw-rw-rw-   0        0        0     6802 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/commands/dataset.py
--rw-rw-rw-   0        0        0     8608 2024-05-23 03:18:05.000000 openi-2.0.0b1/src/openi/commands/model.py
--rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/commands/openi_cli.py
--rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b1/src/openi/commands/user.py
--rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/constants.py
--rw-rw-rw-   0        0        0    10840 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/downloader.py
--rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/log.py
--rw-rw-rw-   0        0        0     9731 2024-05-23 03:18:05.000000 openi-2.0.0b1/src/openi/uploader.py
--rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.153163 openi-2.0.0b1/src/openi.egg-info/
--rw-rw-rw-   0        0        0     2102 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.152154 openi-2.0.0b1/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b1/test/test.py
--rw-rw-rw-   0        0        0      179 2024-05-23 03:08:38.000000 openi-2.0.0b1/test/test_openi.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.753149 openi-2.0.0b2/
+-rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.751138 openi-2.0.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b2/README.md
+-rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:51:20.753149 openi-2.0.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2024-05-23 06:47:17.000000 openi-2.0.0b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.695720 openi-2.0.0b2/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.725884 openi-2.0.0b2/src/openi/
+-rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/__init__.py
+-rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b2/src/openi/_dataclass.py
+-rw-rw-rw-   0        0        0     7895 2024-05-23 04:00:55.000000 openi-2.0.0b2/src/openi/_exceptions.py
+-rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b2/src/openi/_file.py
+-rw-rw-rw-   0        0        0     4576 2024-05-23 03:19:45.000000 openi-2.0.0b2/src/openi/_login.py
+-rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b2/src/openi/_session.py
+-rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/_tqdm.py
+-rw-rw-rw-   0        0        0    36678 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/api.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.743909 openi-2.0.0b2/src/openi/commands/
+-rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/__init__.py
+-rw-rw-rw-   0        0        0     6802 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/dataset.py
+-rw-rw-rw-   0        0        0     8628 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/model.py
+-rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/openi_cli.py
+-rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b2/src/openi/commands/user.py
+-rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/constants.py
+-rw-rw-rw-   0        0        0    10840 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/downloader.py
+-rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/log.py
+-rw-rw-rw-   0        0        0     9731 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi/uploader.py
+-rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.749653 openi-2.0.0b2/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.746944 openi-2.0.0b2/test/
+-rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b2/test/test.py
+-rw-rw-rw-   0        0        0      179 2024-05-23 03:08:38.000000 openi-2.0.0b2/test/test_openi.py
```

### Comparing `openi-2.0.0b1/PKG-INFO` & `openi-2.0.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: deprecated
+Requires-Dist: pwinput
 
 # OpenI
 
 > PYPI package for 启智 AI 协作平台。
 
 ## 安装
```

### Comparing `openi-2.0.0b1/README.md` & `openi-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/setup.py` & `openi-2.0.0b2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi",
-    version="2.0.0.b1",
+    version="2.0.0.b2",
     description="A package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
@@ -21,10 +21,10 @@
         "Topic :: Software Development :: Build Tools",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["openi = openi.commands.openi_cli:main"]
     },
-    install_requires=["requests", "tqdm", "deprecated"],
+    install_requires=["requests", "tqdm", "deprecated", "pwinput"],
     python_requires=">=3.8",
 )
```

### Comparing `openi-2.0.0b1/src/openi/_dataclass.py` & `openi-2.0.0b2/src/openi/_dataclass.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/_exceptions.py` & `openi-2.0.0b2/src/openi/_exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 
 
 class OpenIConnectionError(OpenIError):
     def __init__(self):
         self.msg = "无法连接网络，请检查网络设置"
 
 
+class InvalidTokenError(OpenIError):
+    def __init__(self):
+        self.msg = f"Invalid or broken OpenI token."
+
+
 class TokenNotFoundError(OpenIError):
     def __init__(self):
         self.msg = "未找到本地 token；请先使用 `openi.login` 保存启智账户 token 到本地以获取授权。"
 
 
 class UnauthorizedError(OpenIError):
     def __init__(self):
@@ -86,19 +91,14 @@
 
 
 class KeyboardInterruptError(OpenIError):
     def __init__(self, msg):
         self.msg = f"用户中断操作; {msg}"
 
 
-class InvalidTokenError(OpenIError):
-    def __init__(self):
-        self.msg = f"Invalid or broken OpenI token."
-
-
 class DatasetNotFound(OpenIError):
     def __init__(self, repo_id, dataset_url):
         self.msg = f"`{repo_id}` 仓库尚未创建数据集: {dataset_url}"
 
 
 class EmptyDataset(OpenIError):
     def __init__(self, repo_id, dataset_url):
@@ -120,31 +120,31 @@
 
 class ServerFileNotFoundError(OpenIError):
     def __init__(self, msg):
         self.msg = msg
 
 
 class EmptyFolderError(OpenIError):
-    def __init__(self, local_dir):
-        self.msg = f"空目录，未能找到任何本地文件: {local_dir.relative_to(Path.home())}"
+    def __init__(self, local_dir: Path):
+        self.msg = f"空目录，未能找到任何本地文件: {local_dir.absolute()}"
 
 
 class LocalPathNotFound(OpenIError):
     def __init__(self, filepath: Path):
-        self.msg = f"本地文件或目录不存在: {filepath.relative_to(Path.home())}"
+        self.msg = f"本地文件或目录不存在: {filepath.absolute()}"
 
 
 class LocalDirNotFound(OpenIError):
     def __init__(self, local_dir: Path):
-        self.msg = f"本地目录不存在: {local_dir.relative_to(Path.home())}"
+        self.msg = f"本地目录不存在: {local_dir.absolute()}"
 
 
 class FileTypeError(OpenIError):
     def __init__(self, filepath: Path):
-        self.msg = f"非压缩文件(`.zip` 或 `.tar.gz`): {filepath.relative_to(Path.home())}"
+        self.msg = f"非压缩文件(`.zip` 或 `.tar.gz`): {filepath.absolute()}"
 
 
 class FileSizeError(OpenIError):
     def __init__(self, msg):
         self.msg = msg
```

### Comparing `openi-2.0.0b1/src/openi/_file.py` & `openi-2.0.0b2/src/openi/_file.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/_login.py` & `openi-2.0.0b2/src/openi/_login.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/_session.py` & `openi-2.0.0b2/src/openi/_session.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/_tqdm.py` & `openi-2.0.0b2/src/openi/_tqdm.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/api.py` & `openi-2.0.0b2/src/openi/api.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/commands/dataset.py` & `openi-2.0.0b2/src/openi/commands/dataset.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/commands/model.py` & `openi-2.0.0b2/src/openi/commands/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from argparse import (
-    _SubParsersAction, Namespace, SUPPRESS,
+    _SubParsersAction,
+    Namespace,
+    SUPPRESS,
 )
 from pathlib import Path
 from typing import Optional
 
 from openi.commands import BaseOpeniCLICommand
 from .._exceptions import LocalPathNotFound
 from ..constants import DEFAULT_SAVE_PATH
 from ..downloader import (
-    download_model, download_model_file,
+    download_model,
+    download_model_file,
 )
 from ..log import setup_logger
 from ..uploader import (
-    upload_model, upload_model_file,
+    upload_model,
+    upload_model_file,
 )
 
 logger = setup_logger()
 
 
 class ModelCommands(BaseOpeniCLICommand):
     @staticmethod
```

### Comparing `openi-2.0.0b1/src/openi/commands/openi_cli.py` & `openi-2.0.0b2/src/openi/commands/openi_cli.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/commands/user.py` & `openi-2.0.0b2/src/openi/commands/user.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/constants.py` & `openi-2.0.0b2/src/openi/constants.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/downloader.py` & `openi-2.0.0b2/src/openi/downloader.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/log.py` & `openi-2.0.0b2/src/openi/log.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi/uploader.py` & `openi-2.0.0b2/src/openi/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     if not aimodel:
         raise ModelNotFoundError(
             model_name=model_name,
             model_list_url=api.get_repo_models_url(repo_id=repo_id),
         )
     if not aimodel.isCanOper:
         raise UnauthorizedError()
-    if aimodel.modelType != 2:
+    if aimodel.modelType != 1:
         raise UploadError(
             f"模型类型不正确，只能上传本地导入的模型",
         )
 
     local_file: UploadFile = UploadFile(path=file)
     upload_name = (
         local_file.name if not upload_name else upload_name.lstrip("/")
@@ -238,15 +238,15 @@
     if not aimodel:
         raise ModelNotFoundError(
             model_name=model_name,
             model_list_url=api.get_repo_models_url(repo_id=repo_id),
         )
     if not aimodel.isCanOper:
         raise UnauthorizedError()
-    if aimodel.modelType != 2:
+    if aimodel.modelType != 1:
         raise UploadError(
             f"模型类型不正确，只能上传本地导入的模型",
         )
 
     local_dir = folder
     if not isinstance(local_dir, Path):
         local_dir = Path(local_dir).absolute()
```

### Comparing `openi-2.0.0b1/src/openi/utils.py` & `openi-2.0.0b2/src/openi/utils.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/src/openi.egg-info/PKG-INFO` & `openi-2.0.0b2/src/openi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: deprecated
+Requires-Dist: pwinput
 
 # OpenI
 
 > PYPI package for 启智 AI 协作平台。
 
 ## 安装
```

### Comparing `openi-2.0.0b1/src/openi.egg-info/SOURCES.txt` & `openi-2.0.0b2/src/openi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b1/test/test.py` & `openi-2.0.0b2/test/test.py`

 * *Files identical despite different names*

