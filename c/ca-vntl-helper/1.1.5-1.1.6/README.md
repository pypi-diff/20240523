# Comparing `tmp/ca_vntl_helper-1.1.5.tar.gz` & `tmp/ca_vntl_helper-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ca_vntl_helper-1.1.5.tar", last modified: Mon May 20 09:32:29 2024, max compression
+gzip compressed data, was "ca_vntl_helper-1.1.6.tar", last modified: Thu May 23 07:24:30 2024, max compression
```

## Comparing `ca_vntl_helper-1.1.5.tar` & `ca_vntl_helper-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:32:29.289429 ca_vntl_helper-1.1.5/
--rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.5/LICENSE
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 09:32:29.289156 ca_vntl_helper-1.1.5/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.5/README.md
--rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-20 09:32:26.000000 ca_vntl_helper-1.1.5/pyproject.toml
--rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-20 09:32:29.289502 ca_vntl_helper-1.1.5/setup.cfg
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:32:29.286639 ca_vntl_helper-1.1.5/src/
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:32:29.287379 ca_vntl_helper-1.1.5/src/ca_vntl_helper/
--rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper/__init__.py
--rw-r--r--   0 s19404     (502) staff       (20)     3860 2024-05-20 09:32:16.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper/decorator.py
-drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-20 09:32:29.288805 ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/
--rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-20 09:32:29.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/PKG-INFO
--rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-20 09:32:29.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/SOURCES.txt
--rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-20 09:32:29.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/dependency_links.txt
--rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-20 09:32:29.000000 ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/top_level.txt
--rw-r--r--   0 s19404     (502) staff       (20)     1712 2024-05-20 09:20:26.000000 ca_vntl_helper-1.1.5/src/test.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-23 07:24:30.353411 ca_vntl_helper-1.1.6/
+-rw-r--r--   0 s19404     (502) staff       (20)     1073 2024-05-10 16:06:44.000000 ca_vntl_helper-1.1.6/LICENSE
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-23 07:24:30.353114 ca_vntl_helper-1.1.6/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)     6548 2024-05-14 13:06:42.000000 ca_vntl_helper-1.1.6/README.md
+-rw-r--r--   0 s19404     (502) staff       (20)      643 2024-05-23 07:24:16.000000 ca_vntl_helper-1.1.6/pyproject.toml
+-rw-r--r--   0 s19404     (502) staff       (20)       38 2024-05-23 07:24:30.353464 ca_vntl_helper-1.1.6/setup.cfg
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-23 07:24:30.350661 ca_vntl_helper-1.1.6/src/
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-23 07:24:30.351441 ca_vntl_helper-1.1.6/src/ca_vntl_helper/
+-rw-r--r--   0 s19404     (502) staff       (20)       75 2024-05-14 09:42:20.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper/__init__.py
+-rw-r--r--   0 s19404     (502) staff       (20)     4285 2024-05-23 07:18:07.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper/decorator.py
+drwxr-xr-x   0 s19404     (502) staff       (20)        0 2024-05-23 07:24:30.352718 ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/
+-rw-r--r--   0 s19404     (502) staff       (20)     7123 2024-05-23 07:24:30.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/PKG-INFO
+-rw-r--r--   0 s19404     (502) staff       (20)      275 2024-05-23 07:24:30.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 s19404     (502) staff       (20)        1 2024-05-23 07:24:30.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 s19404     (502) staff       (20)       20 2024-05-23 07:24:30.000000 ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/top_level.txt
+-rw-r--r--   0 s19404     (502) staff       (20)     1723 2024-05-23 07:11:36.000000 ca_vntl_helper-1.1.6/src/test.py
```

### Comparing `ca_vntl_helper-1.1.5/LICENSE` & `ca_vntl_helper-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.5/PKG-INFO` & `ca_vntl_helper-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.5
+Version: 1.1.6
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.5/README.md` & `ca_vntl_helper-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ca_vntl_helper-1.1.5/pyproject.toml` & `ca_vntl_helper-1.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ca-vntl-helper"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Bui Ngoc Huy Van", email="bui_ngoc_huy_van@ca-adv.co.jp" },
 ]
 description = "Some useful functions, classes to help work. Create by Van of Techlab CA team."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ca_vntl_helper-1.1.5/src/ca_vntl_helper/decorator.py` & `ca_vntl_helper-1.1.6/src/ca_vntl_helper/decorator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import traceback
 import sys
 import inspect
 import linecache
 import logging
 
-def create_message_detail(error_detail, params, root_cause=None):
+def create_message_detail(error_detail, params, limit_param_char=32,root_cause=None):
     text_code = linecache.getline(error_detail.filename, error_detail.lineno)
     text_code = text_code.replace("\n", "")
     if root_cause:
         root_cause = f"\t-->ROOT CAUSE: {root_cause} \n"
     else:
         root_cause = ""
     # check file contain site-packages or pyt
     if "site-packages" in error_detail.filename:
         note_message = "site-packages"
     else:
         note_message = "your code"
+
+    # except self, and crop value too long
+    params = {key: value if len(str(value)) < limit_param_char else str(value)[:limit_param_char] + "..." for key, value in params.items() if key != "self"}
     message = f"===================================================\n" \
               f"Filename: {error_detail.filename},\n" \
               f"Function name: {error_detail.name}, params: {params}\n" \
               f"\t-----\n" \
               f"\tLine: {error_detail.lineno}, {text_code}\n {root_cause}" \
               f"\t-----\n" \
               f"\tNote: This error is from {note_message}\n"
@@ -42,26 +45,27 @@
             messages = f"Error in function {func.__name__} \n"
             for idx, (frame, error_detail) in enumerate(zip(frames, errors_detail)):
                 if idx == 0:
                     continue
                 argvalues = inspect.getargvalues(frame[0])
                 params = argvalues.locals
                 if idx == len(frames) - 1:
-                    message = create_message_detail(error_detail, params, formatted_lines[-1])
+                    message = create_message_detail(error_detail, params, limit_param_char=32, root_cause=formatted_lines[-1])
                 else:
-                    message = create_message_detail(error_detail, params)
+                    message = create_message_detail(error_detail, params, limit_param_char=32, root_cause=None)
                 messages += message
             logging.error(messages)
             # raise e
     return wrapper
 
 class ErrorTrackerWithCallBacks:
-    def __init__(self, callback_functions=None, is_raise_error=True):
+    def __init__(self, callback_functions=None, is_raise_error=False, limit_param_char=32):
         self.callback_functions = callback_functions
         self.is_raise_error = is_raise_error
+        self.limit_param_char = limit_param_char
     def error_tracking_decorator(self, func):
         def wrapper(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as e:
                 # if python version >= 3.10, use sys.exc_info() instead of sys.exception()
 
@@ -75,17 +79,17 @@
                 messages = f"Error in function {func.__name__} \n"
                 for idx, (frame, error_detail) in enumerate(zip(frames, errors_detail)):
                     if idx == 0:
                         continue
                     argvalues = inspect.getargvalues(frame[0])
                     params = argvalues.locals
                     if idx == len(frames) - 1:
-                        message = create_message_detail(error_detail, params, formatted_lines[-1])
+                        message = create_message_detail(error_detail, params, self.limit_param_char, formatted_lines[-1])
                     else:
-                        message = create_message_detail(error_detail, params)
+                        message = create_message_detail(error_detail, params, self.limit_param_char, root_cause=None)
                     messages += message
                 if self.callback_functions:
                     for callback_function in self.callback_functions:
                         callback_function(messages)
                 else:
                     logging.error(messages)
                 if self.is_raise_error:
```

### Comparing `ca_vntl_helper-1.1.5/src/ca_vntl_helper.egg-info/PKG-INFO` & `ca_vntl_helper-1.1.6/src/ca_vntl_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ca-vntl-helper
-Version: 1.1.5
+Version: 1.1.6
 Summary: Some useful functions, classes to help work. Create by Van of Techlab CA team.
 Author-email: Bui Ngoc Huy Van <bui_ngoc_huy_van@ca-adv.co.jp>
 Project-URL: Homepage, https://github.com/vanbnh/ca-vntl-helper
 Project-URL: Issues, https://github.com/vanbnh/ca-vntl-helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ca_vntl_helper-1.1.5/src/test.py` & `ca_vntl_helper-1.1.6/src/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ca_vntl_helper import ErrorTrackerWithCallBacks
+from ca_vntl_helper import ErrorTrackerWithCallBacks, error_tracking_decorator
 from datetime import datetime, timedelta
 import requests
 
 def notify_to_slack(message, slack_token=None):
     url = f"https://hooks.slack.com/services/{slack_token}"
     data = {
         "text": message
@@ -38,15 +38,15 @@
     return divide(second_inner_a, second_inner_b)
 
 
 def first_inner_function(first_inner_a, first_inner_b):
     return second_inner_function(first_inner_a, first_inner_b)
 
 
-@error_tracking_decorator_with_callbacks  # Just place the decorator here
+@error_tracking_decorator  # Just place the decorator here
 def outer_function(outer_a, outer_b):
     return first_inner_function(outer_a, outer_b)
 
 
 if __name__ == "__main__":
     # The process will get an error when dividing by 0
     try:
```

