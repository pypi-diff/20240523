# Comparing `tmp/ls_api_clients-0.15.0.tar.gz` & `tmp/ls_api_clients-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls_api_clients-0.15.0.tar", last modified: Thu May 23 11:45:49 2024, max compression
+gzip compressed data, was "ls_api_clients-0.16.0.tar", last modified: Thu May 23 13:53:33 2024, max compression
```

## Comparing `ls_api_clients-0.15.0.tar` & `ls_api_clients-0.16.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:49.621310 ls_api_clients-0.15.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 11:42:31.000000 ls_api_clients-0.15.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 11:45:49.621310 ls_api_clients-0.15.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-05-23 11:42:31.000000 ls_api_clients-0.15.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:49.621310 ls_api_clients-0.15.0/ls_api_clients/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-23 11:42:31.000000 ls_api_clients-0.15.0/ls_api_clients/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10433 2024-05-23 11:42:31.000000 ls_api_clients-0.15.0/ls_api_clients/ls_api_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 11:45:49.621310 ls_api_clients-0.15.0/ls_api_clients.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 11:45:49.000000 ls_api_clients-0.15.0/ls_api_clients.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-05-23 11:45:49.000000 ls_api_clients-0.15.0/ls_api_clients.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 11:45:49.000000 ls_api_clients-0.15.0/ls_api_clients.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-05-23 11:45:49.000000 ls_api_clients-0.15.0/ls_api_clients.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-23 11:45:49.000000 ls_api_clients-0.15.0/ls_api_clients.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      707 2024-05-23 11:45:42.000000 ls_api_clients-0.15.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 11:45:49.621310 ls_api_clients-0.15.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11350 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      111 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/ls_api_clients/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       53 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/ls_api_clients/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10340 2024-05-23 13:50:00.000000 ls_api_clients-0.16.0/ls_api_clients/ls_api_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/ls_api_clients.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      732 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      280 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      100 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2024-05-23 13:53:33.000000 ls_api_clients-0.16.0/ls_api_clients.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      707 2024-05-23 13:53:24.000000 ls_api_clients-0.16.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 13:53:33.014967 ls_api_clients-0.16.0/setup.cfg
```

### Comparing `ls_api_clients-0.15.0/LICENSE` & `ls_api_clients-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ls_api_clients-0.15.0/PKG-INFO` & `ls_api_clients-0.16.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.15.0
+Version: 0.16.0
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_api_clients-0.15.0/ls_api_clients/ls_api_client.py` & `ls_api_clients-0.16.0/ls_api_clients/ls_api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import msgpack
 from ls_cred_storage import LSCredStorage
 from laser_mind_client_meta import MessageKeys
 
 
 class LSAPIClient:
 
-    USER_KEY = 'user'
+    USER_KEY = 'userToken'
     USER_ID_KEY = 'userId'
     TIMESTAMP_KEY = 'timestamp'
     SESSION_TOKEN_KEY = 'sessionToken'
     ACCESS_TOKEN_KEY = 'accessToken'
     MAX_TOKEN_RETENTION_TIME_SECS = 3500
 
     SOLVER_REQUEST_HEADERS = {'accept' : 'application/octet-stream',
@@ -29,32 +29,31 @@
 
     URL_REQUEST_HEADERS = {
         'accept' : 'application/msgpack',
         'content-type' : 'application/msgpack',
         'accept-encoding' : 'gzip, deflate, br'
     }
 
-    def __init__(self, username = None, password = None, printTiming = False, logLevel = logging.INFO, authEnabled = True):
+    def __init__(self, usertoken = None, printTiming = False, logLevel = logging.INFO, authEnabled = True):
         self.LS_API_RUN_URL = os.environ['LS_API_RUN_URL'] if 'LS_API_RUN_URL' in os.environ else 'http://solve.lightsolver.com/api/v1/commands/run'
         self.LS_API_RUN_SECURED_URL = os.environ['LS_API_RUN_SECURED_URL'] if 'LS_API_RUN_SECURED_URL' in os.environ else 'https://solve.lightsolver.com/api/v1/commands/run'
         self.LS_API_GET_PRESIGNED_URL = os.environ['LS_API_GET_PRESIGNED_URL'] if 'LS_API_GET_PRESIGNED_URL' in os.environ else 'https://solve.lightsolver.com/api/v1/getposturl'
         self.LS_AUTH_URL = os.environ['LS_AUTH_URL'] if 'LS_AUTH_URL' in os.environ else 'https://auth.devfront.lightsolver.com/authorize-solver-usage'
         self.LS_REQUEST_URL = os.environ['LS_REQUEST_URL'] if 'LS_REQUEST_URL' in os.environ else 'https://solve.lightsolver.com/api/v1/getsolution'
 
         logging.basicConfig(
             filename="laser-mind.log",
             level=logLevel,
             format='%(asctime)s %(message)s', datefmt='%m/%d/%Y %H:%M:%S')
         self.printTiming = printTiming
         self.authEnabled = authEnabled
         if authEnabled:
-            if username == None or password == None:
-                raise ValueError("You must input a username and password when authREnabled = True")
-            self.username = username
-            self.password = password
+            if usertoken == None :
+                raise ValueError("You must input a usertoken when authREnabled = True")
+            self.usertoken = usertoken
             self.credStorage = LSCredStorage()
             token_dic = self.check_and_get_persisted_tokens() #TODO @markin is this duplication with check_is_token_valid() in refresh_tokens_if_needed?
 
             if token_dic == None:
                 self.refresh_tokens_if_needed()
                 logging.info('Got new session/access tokens')
             logging.info('LSAPIClient created,connection is authenticated and authorized')
@@ -71,22 +70,21 @@
         except Exception as e:
             return None
         return v
 
     def refresh_tokens_if_needed(self):
         if self.authEnabled and not self.check_is_token_valid():
             newTokenDic = self.GetTokensFromServer()
-            logging.info(f'got tokens for user {self.username}')
+            logging.info(f'got tokens for usertoken {self.usertoken}')
             self.credStorage.update_current_token(newTokenDic)
-            self.credStorage.store_token(self.username, newTokenDic)
+            self.credStorage.store_token(self.usertoken, newTokenDic)
 
     def GetTokensFromServer(self):
         data = {
-            'user' : f'{self.username}',
-            'password' : f'{self.password}'
+            'userToken' : f'{self.usertoken}'
         }
 
         headers = {
             'accept' : 'application/json',
             'content-type' : 'application/json',
             }
         req = requests.post(self.LS_AUTH_URL, headers=headers, data=json.dumps(data))
@@ -94,23 +92,23 @@
         token = req.json()
         token_dic  = self.create_token_data_for_user(token)
         return token_dic
 
     def create_token_data_for_user(self, token):
         dic = {
             self.TIMESTAMP_KEY : time.time(),
-            self.USER_KEY : self.username,
+            self.USER_KEY : self.usertoken,
             self.SESSION_TOKEN_KEY : token[self.SESSION_TOKEN_KEY],
             self.ACCESS_TOKEN_KEY : token[self.ACCESS_TOKEN_KEY],
             self.USER_ID_KEY : token[self.USER_ID_KEY]
         }
         return dic
 
     def check_and_get_persisted_tokens(self):
-        storedToken = self.credStorage.get_stored_token(self.username)
+        storedToken = self.credStorage.get_stored_token(self.usertoken)
         if storedToken != None:
             if self.check_is_token_valid():
                 return storedToken
         return None
 
     def check_is_token_valid(self):
         if self.credStorage.currentTokenDic != None:
@@ -120,40 +118,40 @@
     def MakeDataForSolveRequest(self, commandName, param):
         data = {
             'name' : commandName,
             'param' : param,
             'creationTime' : time.time()
         }
         if self.authEnabled:
-            data['username'] = self.credStorage.currentTokenDic[self.USER_KEY]
+            data['userToken'] = self.credStorage.currentTokenDic[self.USER_KEY]
             data['userId'] = self.credStorage.currentTokenDic[self.USER_ID_KEY]
             data['sessionToken'] = self.credStorage.currentTokenDic[self.SESSION_TOKEN_KEY]
             data['accessToken'] = self.credStorage.currentTokenDic[self.ACCESS_TOKEN_KEY]
         return self.msgpack_encode(data)
 
     def MakeDataForUploadRequest(self, toUpload):
         data = {
             'param' : toUpload,
             'creationTime' : time.time()
         }
         if self.authEnabled:
-            data['username'] = self.credStorage.currentTokenDic[self.USER_KEY]
+            data['userToken'] = self.credStorage.currentTokenDic[self.USER_KEY]
             data['userId'] = self.credStorage.currentTokenDic[self.USER_ID_KEY]
             data['sessionToken'] = self.credStorage.currentTokenDic[self.SESSION_TOKEN_KEY]
             data['accessToken'] = self.credStorage.currentTokenDic[self.ACCESS_TOKEN_KEY]
         return self.msgpack_encode(data)
 
     def MakeDataForResultRequest(self, solutionId):
         data = {
             'solId' : solutionId,
             'creationTime' : time.time(),
             'userId' : 0
         }
         if self.authEnabled:
-            data['username'] = self.credStorage.currentTokenDic[self.USER_KEY]
+            data['userToken'] = self.credStorage.currentTokenDic[self.USER_KEY]
             data['userId'] = self.credStorage.currentTokenDic[self.USER_ID_KEY]
             data['sessionToken'] = self.credStorage.currentTokenDic[self.SESSION_TOKEN_KEY]
             data['accessToken'] = self.credStorage.currentTokenDic[self.ACCESS_TOKEN_KEY]
         return self.msgpack_encode(data)
 
     def MakeDataForGetURLRequest(self, inputPath = None):
         data = {
@@ -173,16 +171,16 @@
     def ValidateResponse(self, response):
         if MessageKeys.ERROR_KEY in response:
             raise Exception(response[MessageKeys.ERROR_KEY])
         return True
 
     def SendCommandRequest(self, commandName, input, secured = True):
         if self.authEnabled:
-            if not self.credStorage.is_cached_user(self.username):
-                raise SystemError("username doesn't match stored token, please reconnect LightSolver service")
+            if not self.credStorage.is_cached_user(self.usertoken):
+                raise SystemError("usertoken doesn't match stored session token, please reconnect LightSolver service")
             self.refresh_tokens_if_needed()
         if self.printTiming:
             startTime = time.time()
         data = self.MakeDataForSolveRequest(commandName, input)
         headers = self.SOLVER_REQUEST_HEADERS
         req_url = self.LS_API_RUN_SECURED_URL if secured else self.LS_API_RUN_URL
         response = requests.post(url = req_url, headers = headers, data = data)
```

### Comparing `ls_api_clients-0.15.0/ls_api_clients.egg-info/PKG-INFO` & `ls_api_clients-0.16.0/ls_api_clients.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls-api-clients
-Version: 0.15.0
+Version: 0.16.0
 Summary: A package for laser-mind clients
 Author-email: Assaf Kalinski <assaf@lightsolver.com>
 Project-URL: Homepage, https://lightsolver.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ls_api_clients-0.15.0/pyproject.toml` & `ls_api_clients-0.16.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ls-api-clients"
-version = "0.15.0"
+version = "0.16.0"
 description = "A package for laser-mind clients"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [ "urllib3==1.26.13", "requests>=2.23", "msgpack>=1.0.0", "ls-cred-storage>=0.1.9", "laser-mind-client-meta>=0.0.9",]
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "Assaf Kalinski"
```

