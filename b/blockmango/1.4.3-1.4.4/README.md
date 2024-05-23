# Comparing `tmp/blockmango-1.4.3.tar.gz` & `tmp/blockmango-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.3.tar", last modified: Sat May 18 03:11:47 2024, max compression
+gzip compressed data, was "blockmango-1.4.4.tar", last modified: Thu May 23 13:02:11 2024, max compression
```

## Comparing `blockmango-1.4.3.tar` & `blockmango-1.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-18 03:11:47.309188 blockmango-1.4.3/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.3/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      425 2024-05-18 03:11:47.309188 blockmango-1.4.3/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.3/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-18 03:11:47.293188 blockmango-1.4.3/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.3/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4628 2024-05-17 15:51:44.000000 blockmango-1.4.3/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1477 2024-05-17 15:52:40.000000 blockmango-1.4.3/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2505 2024-05-17 15:53:00.000000 blockmango-1.4.3/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-17 15:53:21.000000 blockmango-1.4.3/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3674 2024-05-17 15:53:39.000000 blockmango-1.4.3/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2375 2024-05-17 15:53:55.000000 blockmango-1.4.3/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-18 03:11:47.305188 blockmango-1.4.3/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      425 2024-05-18 03:11:46.000000 blockmango-1.4.3/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      349 2024-05-18 03:11:46.000000 blockmango-1.4.3/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-18 03:11:46.000000 blockmango-1.4.3/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-18 03:11:46.000000 blockmango-1.4.3/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-18 03:11:46.000000 blockmango-1.4.3/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-18 03:11:47.309188 blockmango-1.4.3/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      498 2024-05-18 03:11:01.000000 blockmango-1.4.3/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.175326 blockmango-1.4.4/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.4/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      425 2024-05-23 13:02:11.171326 blockmango-1.4.4/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.4/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.151326 blockmango-1.4.4/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.4/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4628 2024-05-17 15:51:44.000000 blockmango-1.4.4/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     1477 2024-05-23 12:59:50.000000 blockmango-1.4.4/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2505 2024-05-17 15:53:00.000000 blockmango-1.4.4/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-17 15:53:21.000000 blockmango-1.4.4/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3674 2024-05-17 15:53:39.000000 blockmango-1.4.4/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2437 2024-05-23 12:58:39.000000 blockmango-1.4.4/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-23 13:02:11.167326 blockmango-1.4.4/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      425 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      349 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-23 13:02:10.000000 blockmango-1.4.4/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-23 13:02:11.175326 blockmango-1.4.4/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      498 2024-05-23 13:01:12.000000 blockmango-1.4.4/setup.py
```

### Comparing `blockmango-1.4.3/LICENSE.md` & `blockmango-1.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/README.md` & `blockmango-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/clan.py` & `blockmango-1.4.4/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/decoration.py` & `blockmango-1.4.4/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/friends.py` & `blockmango-1.4.4/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/groupchat.py` & `blockmango-1.4.4/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/http.py` & `blockmango-1.4.4/blockmango/http.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.3/blockmango/user.py` & `blockmango-1.4.4/blockmango/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from .http import HTTPMixin
 
 
 BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
 BASE_URL_ROUTE = "http://route.sandboxol.com/user/api"
-
+BASE_URL_USER_INFO = "http://modsgs.sandboxol.com/api"
 
 class User(HTTPMixin):
   __slots__ = ("headers",)
 
   def __init__(self, user_id, access_token):
     self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
 
   def get_user_info(self):
-    return self._get(f"{BASE_URL_USER}/v2/user/details/info", headers=self.headers)
+    return self._get(f"{BASE_URL_USER_INFO}/v2/user/details/info", headers=self.headers)
 
   def set_birthday(self, birthday):
-    endpoint = f"{BASE_URL_USER}/v1/user/info"
+    endpoint = f"{BASE_URL_USER}/user/info"
     json_data = { "birthday": birthday }
     return self._put(endpoint, headers=self.headers, json_data=json_data)
 
   def login(self, device_id, device_sign, password, userId):
     endpoint = f"{BASE_URL_ROUTE}/v1/app/login"
     headers = { **self.headers, "bmg-sign": device_sign, "bmg-device-id": device_id }
     json_data = { "password": password, "uid": userId }
     return self._post(endpoint, headers=headers, json_data=json_data)
 
   def change_name(self, new_name, old_name):
-    endpoint = f"{BASE_URL_USER}/v3/user/nickName"
+    endpoint = f"{BASE_URL_USER_INFO}/v3/user/nickName"
     params = { "newName": new_name, "oldName": old_name }
     return self._put(endpoint, headers=self.headers, params=params)
 
   def change_details(self, new_details):
-    endpoint = f"{BASE_URL_USER}/v1/user/info"
+    endpoint = f"{BASE_URL_USER_INFO}/v1/user/info"
     json_data = { "details": new_details }
     return self._put(endpoint, headers=self.headers, json_data=json_data)
 
   def change_pfp(self, pfp_url):
-    endpoint = f"{BASE_URL_USER}/v1/user/info"
+    endpoint = f"{BASE_URL_USER}/user/info"
     json_data = { "picUrl": pfp_url }
     return self._put(endpoint, headers=self.headers, json_data=json_data)
 
   def modify_password(self, old_password, new_password):
-    endpoint = f"{BASE_URL_USER}/v1/user/password/modify"
+    endpoint = f"{BASE_URL_USER}/user/password/modify"
     json_data = {"confirmPassword": "", "newPassword": new_password, "oldPassword": old_password}
     return self._post(endpoint, headers=self.headers, json_data=json_data)
 
   def bind_email(self, email, verify_code):
-    endpoint = f"{BASE_URL_USER}/v1/users/bind/email"
+    endpoint = f"{BASE_URL_USER}/users/bind/email"
     json_data = { "email": email, "verifyCode": verify_code }
     return self._post(endpoint, headers=self.headers, json_data=json_data)
 
   def unbind_email(self, verify_code, email):
-    endpoint = f"{BASE_URL_USER}/v2/users/{self.headers['userId']}/emails"
+    endpoint = f"{BASE_URL_USER_INFO}/v2/users/{self.headers['userId']}/emails"
     params = { "email": email, "verifyCode": verify_code }
     return self._delete(endpoint, headers=self.headers, params=params)
```

