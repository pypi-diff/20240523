# Comparing `tmp/pypomes_security-0.1.3.tar.gz` & `tmp/pypomes_security-0.1.4.tar.gz`

## Comparing `pypomes_security-0.1.3.tar` & `pypomes_security-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/src/pypomes_security/__init__.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/src/pypomes_security/access_pomes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pypomes_security-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/src/pypomes_security/__init__.py
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/src/pypomes_security/access_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pypomes_security-0.1.4/PKG-INFO
```

### Comparing `pypomes_security-0.1.3/src/pypomes_security/access_pomes.py` & `pypomes_security-0.1.4/src/pypomes_security/access_pomes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 import requests
 import sys
 from datetime import datetime, timedelta
 from logging import Logger
-from pypomes_core import (
-    APP_PREFIX, TIMEZONE_LOCAL,
-    env_get_str, exc_format
-)
+from pypomes_core import TIMEZONE_LOCAL, exc_format
 from requests import Response
 
-SECURITY_KEY_USER_ID: str = env_get_str(f"{APP_PREFIX}_SECURITY_TAG_USER_ID")
-SECURITY_KEY_USER_PWD: str = env_get_str(f"{APP_PREFIX}_SECURITY_TAG_USER_PWD")
-SECURITY_URL_GET_TOKEN: str = env_get_str(f"{APP_PREFIX}_SECURITY_URL_GET_TOKEN")
-SECURITY_USER_ID: str = env_get_str(f"{APP_PREFIX}_SECURITY_USER_ID")
-SECURITY_USER_PWD: str = env_get_str(f"{APP_PREFIX}_SECURITY_USER_PWD")
-
 
 # initial data for <access_url> in '__access_tokens':
 # {
 #   <access_url> = {
 #     "token": None,
 #     "expiration": datetime(year=2000,
 #                            month=1,
@@ -30,21 +21,21 @@
 #   },
 #   ...
 # }
 __access_tokens: dict = {}
 
 
 def access_set_parameters(service_url: str,
-                          user_id: str, user_pwd: str,
-                          key_user_id: str, key_user_pwd: str) -> None:
+                          user_id: str,
+                          user_pwd: str,
+                          key_user_id: str,
+                          key_user_pwd: str) -> None:
     """
     Set the parameters to use in the service invocation to obtain the access token for *service_url*.
 
-    Note that one set of parameters can optionally be provided as environment variables.
-
     :param service_url: the reference URL for obtaining the access token
     :param user_id: id of user in request
     :param user_pwd: password of user in request
     :param key_user_id: key for sending user id in request
     :param key_user_pwd: key for sending user password in request
     """
     # build the access token structure
@@ -69,16 +60,18 @@
     Remove from storage and return the parameters associated with *service_url*.
 
     :param service_url: the reference URL
     """
     return __access_tokens.pop(service_url)
 
 
-def access_get_token(errors: list[str], service_url: str,
-                     timeout: int | None = None, logger: Logger = None) -> str:
+def access_get_token(errors: list[str],
+                     service_url: str,
+                     timeout: int = None,
+                     logger: Logger = None) -> str:
     """
     Obtain and return an access token for further interaction with a protected resource.
 
     The current token is inspected to determine whether its expiration timestamp requires
     it to be refreshed.
 
     :param errors: incidental error messages
@@ -90,15 +83,15 @@
     # inicialize the return variable
     result: str | None = None
 
     # initialize the local error message
     err_msg: str | None = None
 
     # obtain the token data for the given URL
-    url_token_data: dict = __get_url_token_data(service_url)
+    url_token_data: dict = __access_tokens.get(service_url)
 
     # has the token data been obtained ?
     if url_token_data:
         # yes, proceed
         token_expiration: datetime = url_token_data.get("expiration")
 
         # establish the current date and time
@@ -139,15 +132,15 @@
                     if logger:
                         logger.info(f"Access token obtained: {reply}")
                 else:
                     # no, retrieve the reason for the failure
                     reply = response.reason
 
                 # was the access token retrieved ?
-                if token is not None and len(token) > 0:
+                if token:
                     # yes, proceed
                     url_token_data["token"] = token
                     duration: int = reply.get("expires_in")
                     url_token_data["expiration"] = just_now + timedelta(seconds=duration)
                     result = token
                 else:
                     # no, report the problem
@@ -158,26 +151,11 @@
     else:
         # no, report the problem
         err_msg = f"Parameters for obtaining access token from '{service_url}' have not been defined"
 
     if err_msg:
         if logger:
             logger.error(err_msg)
-        errors.append(err_msg)
-
-    return result
-
-
-def __get_url_token_data(service_url: str) -> dict:
-
-    # obtain the data for the given service URL
-    result: dict = __access_tokens.get(service_url)
-
-    # no data found for URL, but environment data matches it ?
-    if not result and service_url == SECURITY_URL_GET_TOKEN:
-        # yes, store the data
-        access_set_parameters(service_url,
-                              SECURITY_USER_ID, SECURITY_USER_PWD,
-                              SECURITY_KEY_USER_ID, SECURITY_KEY_USER_PWD)
-        result: dict = __access_tokens.get(service_url)
+        if isinstance(errors, list):
+            errors.append(err_msg)
 
     return result
```

### Comparing `pypomes_security-0.1.3/LICENSE` & `pypomes_security-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_security-0.1.3/pyproject.toml` & `pypomes_security-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_security"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (security modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
-    "pip>=23.3.1",
-    "pypomes_core>=0.6.4",
-    "setuptools>=68.0.0",
+    "pip>=24.0",
+    "pypomes_core>=1.0.6",
+    "setuptools>=69.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Security"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-Security/issues"
```

### Comparing `pypomes_security-0.1.3/PKG-INFO` & `pypomes_security-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypomes_security
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (security modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Security
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Security/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: pip>=23.3.1
-Requires-Dist: pypomes-core>=0.6.4
-Requires-Dist: setuptools>=68.0.0
+Requires-Dist: pip>=24.0
+Requires-Dist: pypomes-core>=1.0.6
+Requires-Dist: setuptools>=69.0.0
 Requires-Dist: wheel>=0.41.0
```

