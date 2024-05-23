# Comparing `tmp/openi-2.0.0b0.tar.gz` & `tmp/openi-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-2.0.0b0.tar", last modified: Wed May 22 03:01:03 2024, max compression
+gzip compressed data, was "openi-2.0.0b1.tar", last modified: Thu May 23 03:18:08 2024, max compression
```

## Comparing `openi-2.0.0b0.tar` & `openi-2.0.0b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.710951 openi-2.0.0b0/
--rw-rw-rw-   0        0        0     2102 2024-05-22 03:01:03.709960 openi-2.0.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b0/README.md
--rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 03:01:03.711906 openi-2.0.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1005 2024-05-22 03:00:51.000000 openi-2.0.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.588225 openi-2.0.0b0/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.678837 openi-2.0.0b0/src/openi/
--rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/__init__.py
--rw-rw-rw-   0        0        0    10892 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_dataclass.py
--rw-rw-rw-   0        0        0     7945 2024-05-22 02:53:31.000000 openi-2.0.0b0/src/openi/_exceptions.py
--rw-rw-rw-   0        0        0     7070 2024-05-20 09:08:09.000000 openi-2.0.0b0/src/openi/_file.py
--rw-rw-rw-   0        0        0     4370 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_login.py
--rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b0/src/openi/_session.py
--rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/_tqdm.py
--rw-rw-rw-   0        0        0    36274 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/api.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.691877 openi-2.0.0b0/src/openi/commands/
--rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/__init__.py
--rw-rw-rw-   0        0        0     6792 2024-05-20 09:40:07.000000 openi-2.0.0b0/src/openi/commands/dataset.py
--rw-rw-rw-   0        0        0     8386 2024-05-20 09:40:07.000000 openi-2.0.0b0/src/openi/commands/model.py
--rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/openi_cli.py
--rw-rw-rw-   0        0        0     2512 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/commands/user.py
--rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/constants.py
--rw-rw-rw-   0        0        0    10572 2024-05-20 09:44:06.000000 openi-2.0.0b0/src/openi/downloader.py
--rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/log.py
--rw-rw-rw-   0        0        0     9514 2024-05-22 02:59:11.000000 openi-2.0.0b0/src/openi/uploader.py
--rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b0/src/openi/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.708952 openi-2.0.0b0/src/openi.egg-info/
--rw-rw-rw-   0        0        0     2102 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-22 03:01:03.000000 openi-2.0.0b0/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 03:01:03.707951 openi-2.0.0b0/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b0/test/test.py
--rw-rw-rw-   0        0        0      124 2024-04-28 08:58:09.000000 openi-2.0.0b0/test/test_openi.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.158169 openi-2.0.0b1/
+-rw-rw-rw-   0        0        0     2102 2024-05-23 03:18:08.156168 openi-2.0.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b1/README.md
+-rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:18:08.159165 openi-2.0.0b1/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2024-05-22 07:31:03.000000 openi-2.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.045983 openi-2.0.0b1/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.106352 openi-2.0.0b1/src/openi/
+-rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/__init__.py
+-rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b1/src/openi/_dataclass.py
+-rw-rw-rw-   0        0        0     7945 2024-05-22 02:53:31.000000 openi-2.0.0b1/src/openi/_exceptions.py
+-rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b1/src/openi/_file.py
+-rw-rw-rw-   0        0        0     4576 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/_login.py
+-rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b1/src/openi/_session.py
+-rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/_tqdm.py
+-rw-rw-rw-   0        0        0    36678 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/api.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.133064 openi-2.0.0b1/src/openi/commands/
+-rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/commands/__init__.py
+-rw-rw-rw-   0        0        0     6802 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/commands/dataset.py
+-rw-rw-rw-   0        0        0     8608 2024-05-23 03:18:05.000000 openi-2.0.0b1/src/openi/commands/model.py
+-rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/commands/openi_cli.py
+-rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b1/src/openi/commands/user.py
+-rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/constants.py
+-rw-rw-rw-   0        0        0    10840 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi/downloader.py
+-rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/log.py
+-rw-rw-rw-   0        0        0     9731 2024-05-23 03:18:05.000000 openi-2.0.0b1/src/openi/uploader.py
+-rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b1/src/openi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.153163 openi-2.0.0b1/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     2102 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 03:18:07.000000 openi-2.0.0b1/src/openi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:18:08.152154 openi-2.0.0b1/test/
+-rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b1/test/test.py
+-rw-rw-rw-   0        0        0      179 2024-05-23 03:08:38.000000 openi-2.0.0b1/test/test_openi.py
```

### Comparing `openi-2.0.0b0/PKG-INFO` & `openi-2.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-2.0.0b0/README.md` & `openi-2.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/setup.py` & `openi-2.0.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi",
-    version="2.0.0.b0",
+    version="2.0.0.b1",
     description="A package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-2.0.0b0/src/openi/_dataclass.py` & `openi-2.0.0b1/src/openi/_dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,17 @@
         self.owner = UserInfo(**kwargs.pop("owner"))
         self.name = kwargs.pop("name")
         self.repo_id = kwargs.pop("full_name")
 
         self.size = kwargs.pop("size", None)
         self.html_url = kwargs.pop("html_url", None)
         permissions = kwargs.pop("permissions", None)
-        self.permissions = RepoPermission(**permissions) if permissions else None
+        self.permissions = (
+            RepoPermission(**permissions) if permissions else None
+        )
 
         created_at = kwargs.pop("created_at", None)
         self.created_at = parse_time(created_at) if created_at else None
         updated_at = kwargs.pop("updated_at", None)
         self.updated_at = parse_time(updated_at) if updated_at else None
 
 
@@ -331,14 +333,15 @@
     userName: Optional[str]
     isCanOper: Optional[bool]
     isCanDelete: Optional[bool]
     isCanDownload: Optional[bool]
     repoName: Optional[str]
     repoOwnerName: Optional[str]
     modelFileList: Optional[List[ModelFile]]
+    modelType: Optional[int]
 
     def __init__(self, **kwargs):
         self.id = kwargs.pop("id", None)
         self.name = kwargs.pop("name", None)
         self.size = kwargs.pop("size", None)
         self.path = kwargs.pop("path", None)
         self.repo_id = kwargs.pop("repo_id", None)
@@ -355,14 +358,16 @@
         if modelFileList:
             for data in modelFileList:
                 data.update({"repo_id": self.repo_id, "model_id": self.id})
             self.modelFileList = [ModelFile(**data) for data in modelFileList]
         else:
             self.modelFileList = None
 
+        self.modelType = kwargs.pop("modelType", None)
+
 
 @dataclass
 class ModelCreate:
     code: str
     msg: Optional[str] = None
     id: Optional[int] = None
```

### Comparing `openi-2.0.0b0/src/openi/_exceptions.py` & `openi-2.0.0b1/src/openi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/_file.py` & `openi-2.0.0b1/src/openi/_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     if isinstance(filepath, str):
         filepath = Path(filepath).absolute()
 
     filename = filepath.name.split(".")
     stem, suffix = filename[0], ".".join(filename[1:])
     new_filepath = filepath
 
-    i = 0
+    i = 1
     while new_filepath.exists():
         new_filepath = filepath.with_name(f"{stem}({i}).{suffix}")
         i += 1
 
     return new_filepath
 
 
@@ -216,39 +216,39 @@
 def get_local_dir_files(local_dir: Path) -> List[Path]:
     """
     Returns a list of filepath in given directory.
     """
     return [file for file in local_dir.rglob("*") if file.is_file()]
 
 
-def get_local_dir_zipfiles(local_dir: Union[Path, str]) -> List[UploadFile]:
-    """
-    Returns a list of dictionaries containing file information.
-
-    Args:
-        folder_path (Path): Path to the folder to process.
-
-    Returns:
-        list: A list of dictionaries with the following structure:
-            {
-                "path": Path object representing the file path,
-                "name": Relative path of the file from the given folder
-            }
-    """
-    if isinstance(local_dir, str):
-        local_dir = Path(local_dir).absolute()
-
-    if not local_dir.is_dir():
-        raise LocalDirNotFound(f"{local_dir} is not a directory")
-
-    file_list = list()
-    for file in local_dir.rglob("*"):
-        if file.is_file() and is_zip(file):
-            path = file
-            name = file.name
-            size = get_file_size(file)
-
-            file_obj = UploadFile(path=path, name=name, size=size)
-
-            file_list.append(file_obj)
-
-    return file_list
+# def get_local_dir_zipfiles(local_dir: Union[Path, str]) -> List[UploadFile]:
+#     """
+#     Returns a list of dictionaries containing file information.
+#
+#     Args:
+#         folder_path (Path): Path to the folder to process.
+#
+#     Returns:
+#         list: A list of dictionaries with the following structure:
+#             {
+#                 "path": Path object representing the file path,
+#                 "name": Relative path of the file from the given folder
+#             }
+#     """
+#     if isinstance(local_dir, str):
+#         local_dir = Path(local_dir).absolute()
+#
+#     if not local_dir.is_dir():
+#         raise LocalDirNotFound(f"{local_dir} is not a directory")
+#
+#     file_list = list()
+#     for file in local_dir.rglob("*"):
+#         if file.is_file() and is_zip(file):
+#             path = file
+#             name = file.name
+#             size = get_file_size(file)
+#
+#             file_obj = UploadFile(path=path, name=name, size=size)
+#
+#             file_list.append(file_obj)
+#
+#     return file_list
```

### Comparing `openi-2.0.0b0/src/openi/_login.py` & `openi-2.0.0b1/src/openi/_login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 import json
+import os
 import re
-from getpass import getpass
 from typing import Optional
 
+from pwinput import pwinput
 from requests.exceptions import ConnectionError, ProxyError
 
 from ._exceptions import UnauthorizedError
 from .api import OpenIApi, UserInfo
-from .constants import DEFAULT_BASE_URL, OPENI_LOGO_ASCII, TOKEN_FILE_PATH, TOKEN_REGEX
+from .constants import (
+    DEFAULT_BASE_URL,
+    OPENI_LOGO_ASCII,
+    TOKEN_FILE_PATH,
+    TOKEN_REGEX,
+)
 
 
 def _display_token_input_box(endpoint: str) -> str:
     """Display the token input prompt
 
     Args:
         endpoint (str): OpenI server endpoint
 
     Returns:
         str: input token
     """
     print(OPENI_LOGO_ASCII)
-    print(f"点击链接获取令牌并复制粘贴到下列输入栏 {endpoint}/user/settings/applications \n")
+    print(
+        f"点击链接获取令牌并复制粘贴到下列输入栏 {endpoint}/user/settings/applications \n"
+    )
     print(
         f"[WARNING] 若本机已保存登录令牌，本次输入的令牌会将其覆盖 \n",
         "          建议使用鼠标右键粘贴，避免输入多余字符\n",
     )
-    return getpass(prompt="  🔒 token: ")
+    return pwinput(prompt="  🔒 token: ")
 
 
 def _save_token(endpoint: str, token: str, username: str) -> None:
     """Save the token to local machine
 
     Args:
         endpoint (str): OpenI server endpoint
         token (str): access_token
     """
-    TOKEN_FILE_PATH.write_text(json.dumps({"endpoint": endpoint, "token": token}))
+    TOKEN_FILE_PATH.write_text(
+        json.dumps({"endpoint": endpoint, "token": token})
+    )
     print(f"\nYour token was saved to `{TOKEN_FILE_PATH}`")
     print(f"Successfully log in as `{username}` @{endpoint}!\n")
 
 
 def _bad_token(token: str) -> None:
     if not re.match(TOKEN_REGEX, token):
         print(f"\n❌ 输入的令牌格式有误！\n")
@@ -50,15 +60,17 @@
     print(f"\n❌ 登陆失败！此令牌无效 `{token}`\n")
 
 
 def _bad_network() -> None:
     print("\n❌ 登陆失败！请检查网络或代理设置\n")
 
 
-def login(token: Optional[str] = None, endpoint: Optional[str] = DEFAULT_BASE_URL):
+def login(
+    token: Optional[str] = None, endpoint: Optional[str] = DEFAULT_BASE_URL
+):
     """Login to OpenI on local machine
 
     For the first time use, you need to provide the token and endpoint.
     Will first check with the provided token and endpoint, if valid, save it to local machine
     on `/home/.openi/token.json` and print out the success message.
     If there is a saved token on local machine, will be replaced by the new one.
 
@@ -134,11 +146,15 @@
     return user
 
 
 def logout():
     """Remove the token saved on local machine"""
     try:
         TOKEN_FILE_PATH.unlink()
+        OPENI_TOKEN = os.environ.get("OPENI_TOKEN", None)
+        if OPENI_TOKEN:
+            del os.environ["OPENI_TOKEN"]
+
     except FileNotFoundError:
         print("You are not logged in yet!")
     else:
         print(f"Successfully logged out!")
```

### Comparing `openi-2.0.0b0/src/openi/_session.py` & `openi-2.0.0b1/src/openi/_session.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/_tqdm.py` & `openi-2.0.0b1/src/openi/_tqdm.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/api.py` & `openi-2.0.0b1/src/openi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,17 @@
         return DatasetInfo(**resp.data) or None
 
     def list_dataset_files(
         self,
         repo_id: str,
         upload_type: int = 1,
     ) -> Optional[List[DatasetFile]]:
-        dataset_info = self.get_dataset_info(repo_id=repo_id, upload_type=upload_type)
+        dataset_info = self.get_dataset_info(
+            repo_id=repo_id, upload_type=upload_type
+        )
 
         if dataset_info is None:
             raise DatasetNotFound(repo_id, self.get_dataset_url(repo_id))
 
         return dataset_info.attachments
 
     def query_dataset_file(
@@ -248,46 +250,56 @@
                 engine=engine,
                 isPrivate=is_private,
             ),
         )
         resp = r.json()
         return ModelCreate(**resp)
 
-    def get_model_info(self, repo_id: str, model_name: str) -> Optional[ModelInfo]:
+    def get_model_info(
+        self, repo_id: str, model_name: str
+    ) -> Optional[ModelInfo]:
         params: dict = {"name": model_name}
         r = self.session.get(
             f"/{repo_id}/sdk/get_model",
             params=params,
         )
         resp = BasicResp(**r.json())
         if resp.code == -1:
-            raise ModelNotFoundError(model_name, self.get_repo_models_url(repo_id))
+            raise ModelNotFoundError(
+                model_name, self.get_repo_models_url(repo_id)
+            )
 
         resp.data["repo_id"] = repo_id
         return ModelInfo(**resp.data) or None
 
     def list_model_files(
         self,
         repo_id: str,
         model_name: str,
     ) -> Optional[List[ModelFile]]:
-        model_info = self.get_model_info(repo_id=repo_id, model_name=model_name)
+        model_info = self.get_model_info(
+            repo_id=repo_id, model_name=model_name
+        )
 
         if model_info is None:
-            raise ModelNotFoundError(repo_id, self.get_repo_models_url(repo_id))
+            raise ModelNotFoundError(
+                repo_id, self.get_repo_models_url(repo_id)
+            )
 
         return filter_model_version_file(model_info.modelFileList)
 
     def query_model_file(
         self,
         repo_id: str,
         model_name: str,
         filename: str,
     ) -> Optional[ModelFile]:
-        model_files = self.list_model_files(repo_id=repo_id, model_name=model_name)
+        model_files = self.list_model_files(
+            repo_id=repo_id, model_name=model_name
+        )
 
         if model_files is None:
             return None
 
         try:
             return next(f for f in model_files if f.FileName == filename)
         except StopIteration:
@@ -553,15 +565,17 @@
             uuid=uuid,
             uploadID=upload_id,
             type=upload_type,
             chunkNumber=chunk_number,
             size=chunk_size,
         )
         if upload_mode == "dataset":
-            params.update({f"{id_param}": dataset_or_model_id, "file_name": filename})
+            params.update(
+                {f"{id_param}": dataset_or_model_id, "file_name": filename}
+            )
 
         resp = self.session.get(
             route,
             params=params,
         )
         data = dict()
         if resp.status_code == 200:
@@ -666,15 +680,17 @@
         logger.info(f"`{upload_name}` {get_chunks}")
 
         if get_chunks.uploaded:
             if get_chunks.fileName and get_chunks.fileName != upload_name:
                 existing_filename = get_chunks.fileName
             else:
                 existing_filename = None
-            logger.warning(f"{upload_name} already uploaded as {existing_filename}")
+            logger.warning(
+                f"{upload_name} already uploaded as {existing_filename}"
+            )
             raise ServerFileExistsError(
                 filename=upload_name,
                 existing_filename=existing_filename,
             )
 
         # new multipart
         if not get_chunks.uuid or not get_chunks.uploadID:
@@ -685,15 +701,17 @@
                 md5=file_md5,
                 filesize=file_size,
                 total_chunks_counts=total_chunks_count,
                 upload_mode=upload_mode,
             )
             if not new_multipart or new_multipart.result_code == -1:
                 if new_multipart.msg:
-                    msg = f"new multipart failed with error: {new_multipart.msg}"
+                    msg = (
+                        f"new multipart failed with error: {new_multipart.msg}"
+                    )
                 else:
                     msg = f"new multipart failed with unknown error."
                 logger.error(msg)
                 raise UploadError(msg)
 
             get_chunks.uploadID = new_multipart.uploadID
             get_chunks.uuid = new_multipart.uuid
@@ -718,15 +736,18 @@
                 upload_id=get_chunks.uploadID,
                 upload_mode=upload_mode,
                 upload_type=upload_type,
                 chunk_size=len(chunk_data),
                 filename=upload_name,
             )
             if not multipart_url.url:
-                msg = f"get multipart url failed with" f" error {multipart_url.msg}."
+                msg = (
+                    f"get multipart url failed with"
+                    f" error {multipart_url.msg}."
+                )
                 logger.error(msg)
                 raise UploadError(msg)
             logger.info(f"`{upload_name}` {multipart_url}")
 
             etag = self.session.put_upload(
                 url=multipart_url.url,
                 filedata=chunk_data,
@@ -735,15 +756,18 @@
             if not etag:
                 raise UploadError("put upload failed")
 
             yield len(chunk_data)
             etags.append(etag)
 
         if len(etags) != total_chunks_count - start_from_chunk + 1:
-            msg = f"some chunk failed to upload, can not complete upload " f"process."
+            msg = (
+                f"some chunk failed to upload, can not complete upload "
+                f"process."
+            )
             logger.error(msg)
             raise UploadError(msg)
 
         # complete multipart
         complete = self.upload_complete_multipart(
             dataset_or_model_id=dataset_or_model_id,
             upload_mode=upload_mode,
@@ -1009,15 +1033,17 @@
         Args:
             repo_id (str): Repository ID in `Username/Reponame` format
             model_id (str): model_id of the model to retrieve
 
         Returns:
             dict: model files info in json format of the response from OpenI
         """
-        model_info = self.get_model_info(repo_id=repo_id, model_name=model_name)
+        model_info = self.get_model_info(
+            repo_id=repo_id, model_name=model_name
+        )
         if not model_info:
             return None
 
         print(model_info)
         model_id: str = model_info.id
 
         resp = self.session.get(
```

### Comparing `openi-2.0.0b0/src/openi/commands/dataset.py` & `openi-2.0.0b1/src/openi/commands/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
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
@@ -48,31 +50,31 @@
     def register_subcommand(subparsers_dataset):
         """
         download subcommand
         """
         download_parser = subparsers_dataset.add_parser(
             "download",
             help="下载数据集, openi dataset download -h 查看更多说明",
-            usage="openi dataset download FILENAME REPO_ID [--cluster CLUSTER] [--save_path PATH] [--force]",
+            usage="openi dataset download REPO_ID FILENAME [--cluster CLUSTER] [--save_path PATH] [--force]",
             description="下载数据集，需指定仓库路径及文件，下载公开数据集无需登陆",
         )
         download_parser._action_groups.pop()
 
         """
         arguments
         """
         download_parser_args = download_parser.add_argument_group("arguments")
         download_parser_args.add_argument(
-            "filename",
-            help="数据集文件名称",
-        )
-        download_parser_args.add_argument(
             "repo_id",
             help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限",
         )
+        download_parser_args.add_argument(
+            "filename",
+            help="数据集文件名称",
+        )
 
         """
         optional arguments
         """
         download_parser_optional_args = download_parser.add_argument_group(
             "optional arguments"
         )
```

### Comparing `openi-2.0.0b0/src/openi/commands/model.py` & `openi-2.0.0b1/src/openi/commands/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 
         """
         arguments
         """
         download_parser_args = download_parser.add_argument_group("arguments")
         download_parser_args.add_argument(
             "repo_id",
-            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
         )
         download_parser_args.add_argument(
             "model_name",
-            help="网页端模型名称",
+            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
         )
 
         """
         optional arguments
         """
         download_parser_optional_args = download_parser.add_argument_group(
             "optional arguments"
@@ -173,19 +173,19 @@
         upload_parser_args = upload_parser.add_argument_group("arguments")
         upload_parser_args.add_argument(
             "file_path",
             help="本地路径，可传入`本地文件`或`本地文件夹`路径；上传`文件夹`时将包含所有文件与子目录文件",
         )
         upload_parser_args.add_argument(
             "repo_id",
-            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限",
+            help="所在仓库路径，格式为`拥有者/仓库名`，用户需要拥有此仓库权限；可在网页端一键复制",
         )
         upload_parser_args.add_argument(
             "model_name",
-            help="网页端模型名称",
+            help="网页端模型名称，可在网页端一键复制；注意区分大小写，否则无法找到模型",
         )
 
         """
         optional arguments
         """
         upload_parser_optional_args = upload_parser.add_argument_group(
             "optional arguments"
```

### Comparing `openi-2.0.0b0/src/openi/commands/openi_cli.py` & `openi-2.0.0b1/src/openi/commands/openi_cli.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/commands/user.py` & `openi-2.0.0b1/src/openi/commands/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,25 @@
             help="使用启智社区令牌登录并保存到本地",
             description="使用启智社区网页端生成的令牌登录: https://openi.pcl.ac.cn/user/settings/applications",
         )
         login_parser.add_argument(
             "-t",
             "--token",
             dest="token",
+            metavar="",
             default=None,
             type=str,
             required=False,
             help="选填: 启智社区令牌，填写此参数将会跳过命令行输入",
         )
         login_parser.add_argument(
             "-e",
             "--endpoint",
             dest="endpoint",
+            metavar="",
             default=DEFAULT_BASE_URL,
             type=str,
             required=False,
             help="选填: 仅内部使用",  # "For internal distribution only",
         )
         login_parser.set_defaults(func=lambda args: LoginCommand(args))
```

### Comparing `openi-2.0.0b0/src/openi/constants.py` & `openi-2.0.0b1/src/openi/constants.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/downloader.py` & `openi-2.0.0b1/src/openi/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,14 +213,17 @@
     )
     if not model_file:
         model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
         raise ServerFileNotFoundError(
             f" `{model_name}` 模型内未找到 `{file}` 文件; 请在网页端查看: {model_url}",
         )
 
+    if not isinstance(save_path, Path):
+        save_path = Path(save_path)
+
     if save_path == DEFAULT_SAVE_PATH:
         save_path = DEFAULT_SAVE_PATH / model_name
 
     subdir, filename = split_subdir_name(model_file.FileName)
     save_path = save_path / subdir
 
     cache_file: CacheFile = CacheFile(
@@ -285,25 +288,31 @@
     )
     if not model_file_list:
         model_url = api.get_model_url(repo_id=repo_id, model_name=model_name)
         raise ServerFileNotFoundError(
             f"模型 `{model_name}` 内无任何文件; 请在网页端查看: {model_url}",
         )
 
+    if not isinstance(save_path, Path):
+        save_path = Path(save_path)
+
     if save_path == DEFAULT_SAVE_PATH:
         save_path = DEFAULT_SAVE_PATH / model_name
 
     model_file_list.sort(key=lambda x: x.Size)
     pbar_list = list()
     cache_file_list = list()
     for pos, f in enumerate(model_file_list):
+        subdir, filename = split_subdir_name(f.FileName)
+        file_save_path = save_path / subdir
+
         cache_file: CacheFile = CacheFile(
-            name=f.FileName,
+            name=filename,
             size=f.Size,
-            save_path=save_path,
+            save_path=file_save_path,
             force=force,
         )
         cache_file_list.append(cache_file)
 
         pbar: FileProgressBar = create_pbar(
             display_name=cache_file.name,
             size=cache_file.size,
```

### Comparing `openi-2.0.0b0/src/openi/log.py` & `openi-2.0.0b1/src/openi/log.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi/uploader.py` & `openi-2.0.0b1/src/openi/uploader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 from pathlib import Path
 from typing import (
-    List,
-    Literal,
-    Optional,
-    Union,
+    List, Literal, Optional, Union,
 )
 
 from ._exceptions import (
-    DatasetNotFound,
-    EmptyFolderError,
-    FileSizeError,
-    FileTypeError,
-    KeyboardInterruptError,
-    LocalDirNotFound,
-    LocalPathNotFound,
-    ModelNotFoundError,
-    OpenIError,
-    ServerFileExistsError,
-    UnauthorizedError,
-    UploadError,
-    validate_openi_args,
+    DatasetNotFound, EmptyFolderError, FileSizeError, FileTypeError,
+    KeyboardInterruptError, LocalDirNotFound, LocalPathNotFound,
+    ModelNotFoundError, OpenIError, ServerFileExistsError, UnauthorizedError,
+    UploadError, validate_openi_args,
 )
 from ._file import (
-    get_local_dir_files,
-    is_zip,
-    UploadFile,
+    get_local_dir_files, is_zip, UploadFile,
 )
 from ._tqdm import (
-    create_pbar,
-    FileProgressBar,
+    create_pbar, FileProgressBar,
 )
 from .api import OpenIApi
 from .constants import MAX_FILE_SIZE
 from .log import setup_logger
 from .utils import convert_bytes
 
 logger = setup_logger()
@@ -188,14 +173,18 @@
     if not aimodel:
         raise ModelNotFoundError(
             model_name=model_name,
             model_list_url=api.get_repo_models_url(repo_id=repo_id),
         )
     if not aimodel.isCanOper:
         raise UnauthorizedError()
+    if aimodel.modelType != 2:
+        raise UploadError(
+            f"模型类型不正确，只能上传本地导入的模型",
+        )
 
     local_file: UploadFile = UploadFile(path=file)
     upload_name = (
         local_file.name if not upload_name else upload_name.lstrip("/")
     )
 
     if not local_file.exists():
@@ -249,14 +238,18 @@
     if not aimodel:
         raise ModelNotFoundError(
             model_name=model_name,
             model_list_url=api.get_repo_models_url(repo_id=repo_id),
         )
     if not aimodel.isCanOper:
         raise UnauthorizedError()
+    if aimodel.modelType != 2:
+        raise UploadError(
+            f"模型类型不正确，只能上传本地导入的模型",
+        )
 
     local_dir = folder
     if not isinstance(local_dir, Path):
         local_dir = Path(local_dir).absolute()
 
     if not local_dir.is_dir():
         raise LocalDirNotFound(local_dir)
```

### Comparing `openi-2.0.0b0/src/openi/utils.py` & `openi-2.0.0b1/src/openi/utils.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/src/openi.egg-info/PKG-INFO` & `openi-2.0.0b1/src/openi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b0
+Version: 2.0.0b1
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-2.0.0b0/src/openi.egg-info/SOURCES.txt` & `openi-2.0.0b1/src/openi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b0/test/test.py` & `openi-2.0.0b1/test/test.py`

 * *Files identical despite different names*

