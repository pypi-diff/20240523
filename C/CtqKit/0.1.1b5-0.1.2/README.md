# Comparing `tmp/ctqkit-0.1.1b5.tar.gz` & `tmp/ctqkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctqkit-0.1.1b5.tar", max compression
+gzip compressed data, was "ctqkit-0.1.2.tar", max compression
```

## Comparing `ctqkit-0.1.1b5.tar` & `ctqkit-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,28 @@
--rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b5/LICENSE.txt
--rw-r--r--   0        0        0      953 2024-04-22 02:57:48.361735 ctqkit-0.1.1b5/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b5/README.md
--rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b5/src/CtqKit/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b5/src/CtqKit/account.py
--rw-r--r--   0        0        0    31282 2024-04-22 02:55:12.067746 ctqkit-0.1.1b5/src/CtqKit/platform.py
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ctqkit-0.1.1b5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      956 2024-05-23 09:14:19.393240 ctqkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.2/README.md
+-rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.2/src/CtqKit/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.2/src/CtqKit/account.py
+-rw-r--r--   0        0        0       92 2024-04-25 08:58:29.310258 ctqkit-0.1.2/src/CtqKit/circuit/__init__.py
+-rw-r--r--   0        0        0      542 2024-04-25 08:59:38.213625 ctqkit-0.1.2/src/CtqKit/circuit/barrier.py
+-rw-r--r--   0        0        0      408 2024-04-25 09:07:16.885102 ctqkit-0.1.2/src/CtqKit/circuit/gate/__init__.py
+-rw-r--r--   0        0        0     1393 2024-04-25 09:54:45.281271 ctqkit-0.1.2/src/CtqKit/circuit/gate/gate.py
+-rw-r--r--   0        0        0      365 2024-04-25 09:55:29.916726 ctqkit-0.1.2/src/CtqKit/circuit/gate/h.py
+-rw-r--r--   0        0        0      392 2024-04-25 09:57:13.755696 ctqkit-0.1.2/src/CtqKit/circuit/gate/i.py
+-rw-r--r--   0        0        0      561 2024-04-25 07:57:03.110911 ctqkit-0.1.2/src/CtqKit/circuit/gate/rx.py
+-rw-r--r--   0        0        0      676 2024-04-25 08:11:02.166345 ctqkit-0.1.2/src/CtqKit/circuit/gate/rxy.py
+-rw-r--r--   0        0        0      551 2024-04-25 07:58:07.284707 ctqkit-0.1.2/src/CtqKit/circuit/gate/ry.py
+-rw-r--r--   0        0        0      587 2024-04-25 08:28:07.056689 ctqkit-0.1.2/src/CtqKit/circuit/gate/rz.py
+-rw-r--r--   0        0        0      601 2024-04-25 09:55:29.893837 ctqkit-0.1.2/src/CtqKit/circuit/gate/s.py
+-rw-r--r--   0        0        0      656 2024-04-25 09:55:29.952290 ctqkit-0.1.2/src/CtqKit/circuit/gate/t.py
+-rw-r--r--   0        0        0      327 2024-04-25 09:55:29.945274 ctqkit-0.1.2/src/CtqKit/circuit/gate/x.py
+-rw-r--r--   0        0        0      431 2024-04-25 09:55:29.902247 ctqkit-0.1.2/src/CtqKit/circuit/gate/x2m.py
+-rw-r--r--   0        0        0      430 2024-04-25 09:55:29.876786 ctqkit-0.1.2/src/CtqKit/circuit/gate/x2p.py
+-rw-r--r--   0        0        0      330 2024-04-25 09:55:29.925444 ctqkit-0.1.2/src/CtqKit/circuit/gate/y.py
+-rw-r--r--   0        0        0      428 2024-04-25 09:55:29.937166 ctqkit-0.1.2/src/CtqKit/circuit/gate/y2m.py
+-rw-r--r--   0        0        0      425 2024-04-25 09:55:29.886773 ctqkit-0.1.2/src/CtqKit/circuit/gate/y2p.py
+-rw-r--r--   0        0        0      686 2024-04-25 09:55:29.931492 ctqkit-0.1.2/src/CtqKit/circuit/gate/z.py
+-rw-r--r--   0        0        0      561 2024-04-25 08:52:49.827958 ctqkit-0.1.2/src/CtqKit/circuit/instruction.py
+-rw-r--r--   0        0        0      547 2024-04-25 09:04:52.115202 ctqkit-0.1.2/src/CtqKit/circuit/measure.py
+-rw-r--r--   0        0        0    31282 2024-04-22 02:55:12.067746 ctqkit-0.1.2/src/CtqKit/platform.py
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 ctqkit-0.1.2/PKG-INFO
```

### Comparing `ctqkit-0.1.1b5/LICENSE.txt` & `ctqkit-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b5/pyproject.toml` & `ctqkit-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "CtqKit"
-version = "0.1.1-beta.5"
+version = "0.1.2"
 description = "中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)"
 authors = ["Gao Jianjian <jianjian001@outlook.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 documentation = "https://qc.zdxlz.com/informationSpace"
 homepage = "https://qc.zdxlz.com/"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.8",
     "Operating System :: OS Independent",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Libraries"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 requests = "^2.31.0"
 numpy = "^1.26.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.2"
```

### Comparing `ctqkit-0.1.1b5/src/CtqKit/account.py` & `ctqkit-0.1.2/src/CtqKit/account.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b5/src/CtqKit/platform.py` & `ctqkit-0.1.2/src/CtqKit/platform.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b5/PKG-INFO` & `ctqkit-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: CtqKit
-Version: 0.1.1b5
+Version: 0.1.2
 Summary: 中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)
 Home-page: https://qc.zdxlz.com/
 License: Apache 2.0
 Author: Gao Jianjian
 Author-email: jianjian001@outlook.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://qc.zdxlz.com/informationSpace
 Description-Content-Type: text/markdown
```

