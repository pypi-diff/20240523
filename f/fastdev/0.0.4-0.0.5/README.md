# Comparing `tmp/fastdev-0.0.4.tar.gz` & `tmp/fastdev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-0.0.4.tar", last modified: Wed May 22 08:13:50 2024, max compression
+gzip compressed data, was "fastdev-0.0.5.tar", last modified: Wed May 22 14:22:13 2024, max compression
```

## Comparing `fastdev-0.0.4.tar` & `fastdev-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      959 2024-05-22 08:13:50.105966 fastdev-0.0.4/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       45 2024-05-22 06:56:45.000000 fastdev-0.0.4/README.md
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      943 2024-05-22 08:13:08.000000 fastdev-0.0.4/pyproject.toml
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-22 08:13:50.105966 fastdev-0.0.4/setup.cfg
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.103966 fastdev-0.0.4/src/
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.103966 fastdev-0.0.4/src/fastdev/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.4/src/fastdev/constants.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/datasets/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/datasets/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17763 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/datasets/dexycb.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/fileio/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/__init__.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/fileio/handlers/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      501 2024-05-22 08:08:06.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/base_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      699 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/json_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1737 2024-05-22 07:11:50.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/yaml_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2789 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/fileio/io.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 07:27:36.000000 fastdev-0.0.4/src/fastdev/py.typed
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/robotics/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       90 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/robotics/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1028 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/robotics/urdf.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/smplx/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      275 2024-05-22 08:08:06.000000 fastdev-0.0.4/src/fastdev/smplx/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3996 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/smplx/smplx.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/transforms/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.4/src/fastdev/transforms/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17378 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/rotation.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     6452 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/transforms.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2964 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/utils.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/utils/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      123 2024-05-22 07:54:17.000000 fastdev-0.0.4/src/fastdev/utils/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      782 2024-05-22 07:31:36.000000 fastdev-0.0.4/src/fastdev/utils/dispatch.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1188 2024-05-17 08:54:36.000000 fastdev-0.0.4/src/fastdev/utils/geometry.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1339 2024-05-22 07:11:15.000000 fastdev-0.0.4/src/fastdev/utils/timer.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/visualization/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/visualization/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1803 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/visualization/image.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/src/fastdev.egg-info/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      959 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1054 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/SOURCES.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/dependency_links.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      158 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/requires.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/top_level.txt
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/tests/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-13 08:49:05.000000 fastdev-0.0.4/tests/test_fileio.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      663 2024-05-22 06:55:51.000000 fastdev-0.0.4/tests/test_transforms.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.365371 fastdev-0.0.5/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)     1777 2024-05-22 14:22:13.365371 fastdev-0.0.5/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      572 2024-05-22 14:12:30.000000 fastdev-0.0.5/README.md
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1075 2024-05-22 14:16:48.000000 fastdev-0.0.5/pyproject.toml
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-22 14:22:13.365371 fastdev-0.0.5/setup.cfg
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.362371 fastdev-0.0.5/src/
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.363371 fastdev-0.0.5/src/fastdev/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.5/src/fastdev/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.5/src/fastdev/constants.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.363371 fastdev-0.0.5/src/fastdev/datasets/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.5/src/fastdev/datasets/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17873 2024-05-22 14:13:10.000000 fastdev-0.0.5/src/fastdev/datasets/dexycb.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.363371 fastdev-0.0.5/src/fastdev/fileio/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      105 2024-05-22 13:16:15.000000 fastdev-0.0.5/src/fastdev/fileio/__init__.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/fileio/handlers/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.5/src/fastdev/fileio/handlers/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      501 2024-05-22 08:08:06.000000 fastdev-0.0.5/src/fastdev/fileio/handlers/base_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      727 2024-05-22 11:18:03.000000 fastdev-0.0.5/src/fastdev/fileio/handlers/json_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1765 2024-05-22 11:18:11.000000 fastdev-0.0.5/src/fastdev/fileio/handlers/yaml_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3721 2024-05-22 14:15:06.000000 fastdev-0.0.5/src/fastdev/fileio/io.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 07:27:36.000000 fastdev-0.0.5/src/fastdev/py.typed
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/robotics/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      115 2024-05-22 13:17:43.000000 fastdev-0.0.5/src/fastdev/robotics/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1335 2024-05-22 14:15:16.000000 fastdev-0.0.5/src/fastdev/robotics/urdf.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/smplx/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      275 2024-05-22 08:08:06.000000 fastdev-0.0.5/src/fastdev/smplx/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     4099 2024-05-22 13:54:52.000000 fastdev-0.0.5/src/fastdev/smplx/smplx.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/transforms/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.5/src/fastdev/transforms/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17859 2024-05-22 11:31:18.000000 fastdev-0.0.5/src/fastdev/transforms/rotation.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     6624 2024-05-22 11:21:07.000000 fastdev-0.0.5/src/fastdev/transforms/transforms.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3017 2024-05-22 11:21:53.000000 fastdev-0.0.5/src/fastdev/transforms/utils.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/utils/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      123 2024-05-22 07:54:17.000000 fastdev-0.0.5/src/fastdev/utils/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      795 2024-05-22 11:22:28.000000 fastdev-0.0.5/src/fastdev/utils/dispatch.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1215 2024-05-22 11:31:18.000000 fastdev-0.0.5/src/fastdev/utils/geometry.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1361 2024-05-22 11:22:49.000000 fastdev-0.0.5/src/fastdev/utils/timer.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev/visualization/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.5/src/fastdev/visualization/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1831 2024-05-22 11:23:08.000000 fastdev-0.0.5/src/fastdev/visualization/image.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/src/fastdev.egg-info/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)     1777 2024-05-22 14:22:13.000000 fastdev-0.0.5/src/fastdev.egg-info/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1054 2024-05-22 14:22:13.000000 fastdev-0.0.5/src/fastdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-22 14:22:13.000000 fastdev-0.0.5/src/fastdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      235 2024-05-22 14:22:13.000000 fastdev-0.0.5/src/fastdev.egg-info/requires.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-22 14:22:13.000000 fastdev-0.0.5/src/fastdev.egg-info/top_level.txt
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 14:22:13.364371 fastdev-0.0.5/tests/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-22 09:28:48.000000 fastdev-0.0.5/tests/test_fileio.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1185 2024-05-22 09:27:21.000000 fastdev-0.0.5/tests/test_transforms.py
```

### Comparing `fastdev-0.0.4/pyproject.toml` & `fastdev-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastdev"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "Jianglong Ye", email = "jianglong.yeh@gmail.com" }]
 description = "Type less, code more"
 readme = "README.md"
 license = { text = "MIT" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+    "typing-extensions",
     "fastcore",
     "msgspec[toml,yaml]",
     "rich",
     "fsspec",
     "universal_pathlib",
     "huggingface_hub[cli,hf_transfer]",
     "GitPython",
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine", "ipython", "ruff", "pytest", "mypy", "types-PyYAML"]
+doc = ["sphinx", "furo", "docutils", "sphinx-autoapi", "m2r2", "setuptools"]
 
 [project.urls]
 Repository = "https://github.com/jianglongye/fastdev"
 
 [tool.ruff]
 exclude = ["playground", "tests"]
 line-length = 120
 
 [tool.mypy]
 exclude = ["playground", "tests", "dexycb.py"]
+ignore_missing_imports = true
```

### Comparing `fastdev-0.0.4/src/fastdev/constants.py` & `fastdev-0.0.5/src/fastdev/constants.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.4/src/fastdev/datasets/dexycb.py` & `fastdev-0.0.5/src/fastdev/datasets/dexycb.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,20 +69,23 @@
 class DexYCBDatasetConfig:
     data_root: str = os.path.join(FDEV_DATASET_ROOT, "dexycb")
 
     split: Literal["train", "val", "test", "all"] = "train"
     hand_side: Literal["left", "right", "both"] = "left"
     setup: Literal["s0", "s1", "s2", "s3"] = "s0"
     """
-    s0: Seen subjects, camera views, grasped objects, unseen frames
-    s1: Unseen subjects
-    s2: Unseen camera views
-    s3: Unseen grasped objects
 
-    Ref: [here](https://github.com/NVlabs/dex-ycb-toolkit/blob/64551b001d360ad83bc383157a559ec248fb9100/dex_ycb_toolkit/dex_ycb.py#L126)
+    - [s0] Seen subjects, camera views, grasped objects, unseen frames
+    - [s1] Unseen subjects
+    - [s2] Unseen camera views
+    - [s3] Unseen grasped objects
+
+    Reference_
+
+    .. _Reference: https://github.com/NVlabs/dex-ycb-toolkit/blob/64551b001d360ad83bc383157a559ec248fb9100/dex_ycb_toolkit/dex_ycb.py#L126
     """
 
     return_color: bool = True
     return_depth: bool = False
     return_as_sequence: bool = False  # return the whole sequence instead of a single frame
     return_no_hand_frames: bool = True
     # if False, filter out frames where the hand is not visible (mano pose all zeros)
@@ -92,14 +95,16 @@
     force_rebuild_cache: bool = False
 
     def __post_init__(self) -> None:
         assert os.path.exists(self.data_root), f"Data root {self.data_root} does not exist."
 
 
 class DexYCBDataset(Dataset):
+    """DexYCBDataset."""
+
     ycb_classes = _YCB_CLASSES
 
     def __init__(self, config: DexYCBDatasetConfig) -> None:
         super().__init__()
 
         self.config = config
 
@@ -413,7 +418,10 @@
                     collated_batch[key] = default_collate([sample[key] for sample in batch])
             return collated_batch
 
         if not self.config.return_as_sequence:
             return default_collate
         else:
             return _seq_collate_fn
+
+
+__all__ = ["DexYCBDataset", "DexYCBDatasetConfig"]
```

### Comparing `fastdev-0.0.4/src/fastdev/fileio/handlers/json_handler.py` & `fastdev-0.0.5/src/fastdev/fileio/handlers/json_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,10 @@
 
     def dump_to_str(self, obj, **kwargs):
         # https://github.com/jcrist/msgspec/issues/514
         return self.encoder.encode(obj).decode("utf-8")
 
     def load_from_str(self, s: str, **kwargs):
         return self.decoder.decode(s)
+
+
+__all__ = ["JSONHandler"]
```

### Comparing `fastdev-0.0.4/src/fastdev/fileio/handlers/yaml_handler.py` & `fastdev-0.0.5/src/fastdev/fileio/handlers/yaml_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,7 +51,10 @@
 
     def dump_to_str(self, obj, **kwargs):
         # https://github.com/jcrist/msgspec/issues/514
         return msgspec_yaml_encode(obj).decode("utf-8")
 
     def load_from_str(self, s: str, **kwargs):
         return msgspec_yaml_decode(s)
+
+
+__all__ = ["YAMLHandler"]
```

### Comparing `fastdev-0.0.4/src/fastdev/fileio/io.py` & `fastdev-0.0.5/src/fastdev/fileio/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from functools import lru_cache
 from pathlib import Path
-from typing import IO, Any, Dict, Mapping, Optional, Type, Union, cast
+from typing import IO, Any, Dict, Literal, Mapping, Optional, Type, Union, cast
+
+from typing_extensions import TypeAlias
 
 import fsspec  # type: ignore
 
 from fastdev.fileio.handlers.base_handler import BaseFileHandler
 from fastdev.fileio.handlers.json_handler import JSONHandler
 from fastdev.fileio.handlers.yaml_handler import YAMLHandler
 
 FILE_HANDLER_CLASSES: Mapping[str, Type[BaseFileHandler]] = {
     "json": JSONHandler,
     "yaml": YAMLHandler,
     "yml": YAMLHandler,
 }
+FILE_EXTENSIONS: TypeAlias = Literal["json", "yaml", "yml"]
 FILE_HANDLERS: Dict[str, BaseFileHandler] = {}
 
 
 @lru_cache()
 def get_file_handler(file_format: str) -> BaseFileHandler:
     if file_format not in FILE_HANDLERS:
         if file_format not in FILE_HANDLER_CLASSES:
@@ -24,24 +27,36 @@
         else:
             FILE_HANDLERS[file_format] = FILE_HANDLER_CLASSES[file_format]()
     return FILE_HANDLERS[file_format]
 
 
 def load(
     file: Union[str, Path, IO],
-    file_format: Optional[str] = None,
+    file_format: Optional[FILE_EXTENSIONS] = None,
     **kwargs,
 ) -> Any:
-    """Load json/yaml/toml/pickle file from file."""
+    """Load json/yaml/toml/pickle file from file.
+
+    Args:
+        file (Union[str, Path, IO]): file path or io object.
+        file_format (Optional[FILE_EXTENSIONS], optional): file extension. Defaults to None.
+
+    Returns:
+        Any: loaded file.
+
+    Examples:
+        >>> load("assets/example.json")
+        {'hello': 'world'}
+    """
     # Parameters validation
     if isinstance(file, Path):
         file = str(file)
     if file_format is None:
         if isinstance(file, str):
-            file_format = file.split(".")[-1]
+            file_format = cast(FILE_EXTENSIONS, file.split(".")[-1])
         else:
             raise ValueError("file_format is required when file is not a string or path")
 
     # Get file handler
     file_handler = get_file_handler(file_format)
 
     # Load file
@@ -55,31 +70,46 @@
         raise TypeError("File must be a filepath str or a file object")
     return obj
 
 
 def dump(
     obj: Any,
     file: Union[str, Path, IO],
-    file_format: Optional[str] = None,
+    file_format: Optional[FILE_EXTENSIONS] = None,
     **kwargs,
 ):
-    """Dump obj to json/yaml/toml/pickle file."""
+    """Dump obj to json/yaml/toml/pickle file.
+
+    Args:
+        obj (Any): File object to dump.
+        file (Union[str, Path, IO]): File path or IO object.
+        file_format (Optional[FILE_EXTENSIONS], optional): File format. Defaults to None.
+
+    Examples:
+        >>> import tempfile
+        >>> with tempfile.NamedTemporaryFile(suffix=".json") as f:
+        ...     dump({"hello": "world"}, f.name)
+    """
+    "Dump obj to json/yaml/toml/pickle file."
     # Parameters validation
     if isinstance(file, Path):
         file = str(file)
     if file_format is None:
         if isinstance(file, str):
-            file_format = file.split(".")[-1]
+            file_format = cast(FILE_EXTENSIONS, file.split(".")[-1])
         else:
             raise ValueError("file_format is required when file is not a string or path")
 
     # Get file handler
     file_handler = get_file_handler(file_format)
 
     if isinstance(file, str):
         mode = "wb" if file_handler.str_or_bytes == "bytes" else "r"
         with fsspec.open(file, mode) as f:
             file_handler.dump_to_fileobj(obj, cast(IO, f), **kwargs)
     elif hasattr(file, "write"):
         file_handler.dump_to_fileobj(obj, cast(IO, file), **kwargs)
     else:
         raise TypeError("File must be a filepath str or a file object")
+
+
+__all__ = ["FILE_EXTENSIONS", "load", "dump"]
```

### Comparing `fastdev-0.0.4/src/fastdev/smplx/smplx.py` & `fastdev-0.0.5/src/fastdev/smplx/smplx.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,24 +98,29 @@
     mano: MANO,
     betas: torch.Tensor,
     global_orient: torch.Tensor,
     transl: torch.Tensor,
     tf_rot: torch.Tensor,
     tf_transl: Optional[torch.Tensor] = None,
 ) -> Tuple[torch.Tensor, torch.Tensor]:
-    """
-    Change mano parameters to new coordinate system
-    Ref: [here](https://www.dropbox.com/scl/fi/zkatuv5shs8d4tlwr8ecc/Change-parameters-to-new-coordinate-system.paper?rlkey=lotq1sh6wzkmyttisc05h0in0&dl=0
+    """Change mano parameters to the new coordinate system.
+
+    Reference_
+
+    .. _Reference: https://www.dropbox.com/scl/fi/zkatuv5shs8d4tlwr8ecc/Change-parameters-to-new-coordinate-system.paper?rlkey=lotq1sh6wzkmyttisc05h0in0&dl=
     """
     v_shaped = mano.v_template + blend_shapes(betas, mano.shapedirs)  # type: ignore
     pelvis = vertices2joints(mano.J_regressor[0:1], v_shaped).squeeze(dim=1)  # type: ignore
 
     new_global_orient = tf.matrix_to_axis_angle(
         tf.axis_angle_to_matrix(tf_rot) @ tf.axis_angle_to_matrix(global_orient)
     )
     if tf_transl is None:
         tf_transl = torch.zeros_like(transl)
     new_transl = (
         tf.rotate((pelvis + transl).unsqueeze(1), tf.axis_angle_to_matrix(tf_rot)).squeeze(1) - pelvis + tf_transl
     )
 
     return new_global_orient, new_transl
+
+
+__all__ = ["build_mano_layer", "build_mano_layer_manopth", "transform_mano_pose"]
```

### Comparing `fastdev-0.0.4/src/fastdev/transforms/__init__.py` & `fastdev-0.0.5/src/fastdev/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.4/src/fastdev/transforms/rotation.py` & `fastdev-0.0.5/src/fastdev/transforms/rotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     # fmt: on
     matrices = torch.reshape(matrices, quaternions.shape[:-1] + (3, 3))
     return matrices
 
 
 def matrix_to_quaternion(matrix):
     """
-    Convert rotation matrices to quaternions using Shepperds’s method.
+    Convert rotation matrices to quaternions using Shepperds's method.
 
     Args:
         matrix: (np.ndarray, torch.Tensor, list, tuple): rotation matrices, the shape could be ...3x3.
     Returns:
         quaternions with real part first, as tensor of shape (..., 4).
     Ref: http://www.iri.upc.edu/files/scidoc/2068-Accurate-Computation-of-Quaternions-from-Rotation-Matrices.pdf
         Note that the way to determine the best solution is slightly different from the PDF.
@@ -431,7 +431,27 @@
     [1] Zhou, Y., Barnes, C., Lu, J., Yang, J., & Li, H.
     On the Continuity of Rotation Representations in Neural Networks.
     IEEE Conference on Computer Vision and Pattern Recognition, 2019.
     Retrieved from http://arxiv.org/abs/1812.07035
     """
     batch_dim = matrix.shape[:-2]
     return torch.reshape(torch.clone(matrix[..., :2, :]), batch_dim + (6,))
+
+
+__all__ = [
+    "axis_angle_to_matrix",
+    "axis_angle_to_quaternion",
+    "compose_axis_angle",
+    "euler_angles_to_matrix",
+    "matrix_to_axis_angle",
+    "matrix_to_euler_angles",
+    "matrix_to_quaternion",
+    "matrix_to_rotation_6d",
+    "quaternion_real_to_first",
+    "quaternion_real_to_last",
+    "quaternion_to_axis_angle",
+    "quaternion_to_matrix",
+    "random_rotation_matrix",
+    "rotation_6d_to_matrix",
+    "split_axis_angle",
+    "standardize_quaternion",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastdev-0.0.4/src/fastdev/transforms/transforms.py` & `fastdev-0.0.5/src/fastdev/transforms/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,7 +201,20 @@
                 torch.tensor([0.0, 0.0, 0.0, 1.0], dtype=tf_mat.dtype, device=tf_mat.device).repeat(
                     tf_mat.shape[:-2] + (1, 1)
                 ),
             ],
             dim=-2,
         )
     return tf_mat
+
+
+__all__ = [
+    "transform",
+    "rotate",
+    "project",
+    "unproject",
+    "inverse",
+    "swap_major",
+    "rot_tl_to_tf_mat",
+    "to_homo",
+    "expand_tf_mat",
+]
```

### Comparing `fastdev-0.0.4/src/fastdev/transforms/utils.py` & `fastdev-0.0.5/src/fastdev/transforms/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,7 +81,10 @@
         fv: vertical focal length (height)
         cu: horizontal principal point (width)
         cv: vertical principal point (height)
         skew: skew coefficient, default to 0
     """
     intr_mat = np.array([[fu, skew, cu], [0.0, fv, cv], [0.0, 0.0, 1.0]], dtype=np.float32)
     return intr_mat
+
+
+__all__ = ["coord_conversion", "compose_intr_mat"]
```

### Comparing `fastdev-0.0.4/src/fastdev/utils/dispatch.py` & `fastdev-0.0.5/src/fastdev/utils/dispatch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from typing import Callable, DefaultDict, TypeVar
 
-from fastcore.dispatch import TypeDispatch  # type: ignore
+from fastcore.dispatch import TypeDispatch
 
 T = TypeVar("T")
 
 REGISTRY: DefaultDict[str, TypeDispatch] = defaultdict(TypeDispatch)
 
 
 def typedispatch(is_impl: bool = True) -> Callable[[T], T]:
@@ -20,7 +20,10 @@
         if isinstance(f, classmethod):
             f = f.__func__  # type: ignore
         if is_impl:
             REGISTRY[name].add(f)
         return REGISTRY[name]  # type: ignore
 
     return _inner
+
+
+__all__ = ["typedispatch"]
```

### Comparing `fastdev-0.0.4/src/fastdev/utils/geometry.py` & `fastdev-0.0.5/src/fastdev/utils/geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,7 +47,10 @@
 def create_box(
     half_size: Union[Sequence[float], np.ndarray] = [1.0, 1.0, 1.0],
 ) -> Dict[Literal["vertices", "faces"], np.ndarray]:
     vertices = np.asarray(box_data["vertices"], dtype=np.float32)
     vertices = (vertices - 0.5) * 2.0 * half_size
     faces = np.asarray(box_data["faces"], dtype=np.int32)
     return {"vertices": vertices, "faces": faces}
+
+
+__all__ = ["create_box"]
```

### Comparing `fastdev-0.0.4/src/fastdev/utils/timer.py` & `fastdev-0.0.5/src/fastdev/utils/timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,7 +43,10 @@
 
     def seconds(self):
         if self._is_paused:
             end_time = self._last
         else:
             end_time = perf_counter()
         return end_time - self._start - self._total_paused
+
+
+__all__ = ["Timer"]
```

### Comparing `fastdev-0.0.4/src/fastdev/visualization/image.py` & `fastdev-0.0.5/src/fastdev/visualization/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,7 +55,10 @@
             vis_img,
             center=tuple(pts[i].tolist()),
             color=tuple(color.tolist()),
             radius=radius,
             thickness=-1,
         )
     return vis_img
+
+
+__all__ = ["draw_points"]
```

### Comparing `fastdev-0.0.4/src/fastdev.egg-info/SOURCES.txt` & `fastdev-0.0.5/src/fastdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.4/tests/test_fileio.py` & `fastdev-0.0.5/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.4/tests/test_transforms.py` & `fastdev-0.0.5/tests/test_transforms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+import numpy as np
 from fastdev.transforms import rot_tl_to_tf_mat, transform
 
 
 def test_transforms():
     pts = torch.tensor([[1, 2, 3], [4, 5, 6]], dtype=torch.float32)
     rot_mat = torch.tensor([[0, 1, 0], [0, 0, 1], [1, 0, 0]], dtype=torch.float32)
     tl = torch.tensor([1, 2, 3], dtype=torch.float32)
@@ -12,10 +13,20 @@
 
     tgt_pts = torch.tensor([[3, 5, 4], [6, 8, 7]], dtype=torch.float32)
     assert torch.allclose(new_pts, tgt_pts)
 
     new_pts = transform(pts.numpy(), tf_mat.numpy())
     assert torch.allclose(torch.tensor(new_pts), tgt_pts)
 
+    new_pts = transform(pts[None], tf_mat[None])[0]
+    assert torch.allclose(new_pts, tgt_pts)
+
+    new_pts = transform(pts.to(dtype=torch.float16), tf_mat.to(dtype=torch.float16))
+    assert torch.allclose(new_pts, tgt_pts.to(dtype=torch.float16))
+    assert new_pts.dtype == torch.float16
+
+    new_pts = transform(pts.numpy().astype("float16"), tf_mat.numpy().astype("float16"))
+    assert new_pts.dtype == np.float16
+    assert torch.allclose(torch.tensor(new_pts), tgt_pts.to(dtype=torch.float16))
 
 if __name__ == "__main__":
     test_transforms()
```

