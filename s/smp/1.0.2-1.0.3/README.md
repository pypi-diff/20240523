# Comparing `tmp/smp-1.0.2.tar.gz` & `tmp/smp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-1.0.2.tar", max compression
+gzip compressed data, was "smp-1.0.3.tar", max compression
```

## Comparing `smp-1.0.2.tar` & `smp-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-05-20 23:28:26.282016 smp-1.0.2/LICENSE
--rw-r--r--   0        0        0     2312 2024-05-20 23:28:26.282016 smp-1.0.2/README.md
--rw-r--r--   0        0        0     1595 2024-05-20 23:28:26.282016 smp-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/__init__.py
--rw-r--r--   0        0        0      695 2024-05-20 23:28:26.282016 smp-1.0.2/smp/error.py
--rw-r--r--   0        0        0      471 2024-05-20 23:28:26.282016 smp-1.0.2/smp/exceptions.py
--rw-r--r--   0        0        0     5090 2024-05-20 23:28:26.282016 smp-1.0.2/smp/header.py
--rw-r--r--   0        0        0     6286 2024-05-20 23:28:26.282016 smp-1.0.2/smp/image_management.py
--rw-r--r--   0        0        0     4882 2024-05-20 23:28:26.282016 smp-1.0.2/smp/message.py
--rw-r--r--   0        0        0     7153 2024-05-20 23:28:26.282016 smp-1.0.2/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-05-20 23:28:26.282016 smp-1.0.2/smp/packet.py
--rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/py.typed
--rw-r--r--   0        0        0     1022 2024-05-20 23:28:26.282016 smp-1.0.2/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-05-20 23:28:26.282016 smp-1.0.2/smp/user/__init__.py
--rw-r--r--   0        0        0     1321 2024-05-20 23:28:26.282016 smp-1.0.2/smp/user/intercreate.py
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-05-23 00:03:27.238694 smp-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2312 2024-05-23 00:03:27.238694 smp-1.0.3/README.md
+-rw-r--r--   0        0        0     1595 2024-05-23 00:03:27.242694 smp-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/__init__.py
+-rw-r--r--   0        0        0     1811 2024-05-23 00:03:27.242694 smp-1.0.3/smp/error.py
+-rw-r--r--   0        0        0      471 2024-05-23 00:03:27.242694 smp-1.0.3/smp/exceptions.py
+-rw-r--r--   0        0        0     5090 2024-05-23 00:03:27.242694 smp-1.0.3/smp/header.py
+-rw-r--r--   0        0        0     6272 2024-05-23 00:03:27.242694 smp-1.0.3/smp/image_management.py
+-rw-r--r--   0        0        0     4882 2024-05-23 00:03:27.242694 smp-1.0.3/smp/message.py
+-rw-r--r--   0        0        0     7137 2024-05-23 00:03:27.242694 smp-1.0.3/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-05-23 00:03:27.242694 smp-1.0.3/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/py.typed
+-rw-r--r--   0        0        0     1003 2024-05-23 00:03:27.242694 smp-1.0.3/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/user/__init__.py
+-rw-r--r--   0        0        0     1308 2024-05-23 00:03:27.242694 smp-1.0.3/smp/user/intercreate.py
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.3/PKG-INFO
```

### Comparing `smp-1.0.2/LICENSE` & `smp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/README.md` & `smp-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/pyproject.toml` & `smp-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/smp/header.py` & `smp-1.0.3/smp/header.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/smp/image_management.py` & `smp-1.0.3/smp/image_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,13 +205,13 @@
     IMAGE_CONFIRMATION_DENIED = auto()
     """Confirmation of image has been denied"""
 
     IMAGE_SETTING_TEST_TO_ACTIVE_DENIED = auto()
     """Setting test to active slot is not allowed"""
 
 
-class ImageManagementErrorV0(error.ErrorV0[IMG_MGMT_ERR]):
+class ImageManagementErrorV0(error.ErrorV0):
     _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
 
 
 class ImageManagementErrorV1(error.ErrorV1[IMG_MGMT_ERR]):
     _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
```

### Comparing `smp-1.0.2/smp/message.py` & `smp-1.0.3/smp/message.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/smp/os_management.py` & `smp-1.0.3/smp/os_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,13 +239,13 @@
     RTC_NOT_SET = auto()
     """RTC is not set."""
 
     RTC_COMMAND_FAILED = auto()
     """RTC command failed."""
 
 
-class OSManagementErrorV0(error.ErrorV0[OS_MGMT_RET_RC]):
+class OSManagementErrorV0(error.ErrorV0):
     _GROUP_ID = header.GroupId.OS_MANAGEMENT
 
 
 class OSManagementErrorV1(error.ErrorV1[OS_MGMT_RET_RC]):
     _GROUP_ID = header.GroupId.OS_MANAGEMENT
```

### Comparing `smp-1.0.2/smp/packet.py` & `smp-1.0.3/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.2/smp/shell_management.py` & `smp-1.0.3/smp/shell_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     UNKNOWN = auto()
     """Unknown error occurred."""
 
     INVALID_FORMAT = auto()
     """The provided format value is not valid."""
 
 
-class ShellManagementErrorV0(error.ErrorV0[SHELL_MGMT_RET_RC]):
+class ShellManagementErrorV0(error.ErrorV0):
     _GROUP_ID = header.GroupId.SHELL_MANAGEMENT
 
 
 class ShellManagementErrorV1(error.ErrorV1[SHELL_MGMT_RET_RC]):
     _GROUP_ID = header.GroupId.SHELL_MANAGEMENT
```

### Comparing `smp-1.0.2/smp/user/intercreate.py` & `smp-1.0.3/smp/user/intercreate.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,13 +40,13 @@
     OK = 0
     """No error."""
 
     INVALID_IMAGE = auto()
     """No image matched the image provided."""
 
 
-class ErrorV0(error.ErrorV0[IC_MGMT_ERR]):
+class ErrorV0(error.ErrorV0):
     _GROUP_ID = header.UserGroupId.INTERCREATE
 
 
 class ErrorV1(error.ErrorV1[IC_MGMT_ERR]):
     _GROUP_ID = header.UserGroupId.INTERCREATE
```

### Comparing `smp-1.0.2/PKG-INFO` & `smp-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

