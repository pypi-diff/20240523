# Comparing `tmp/test_nvf_builds-0.0.3.6.tar.gz` & `tmp/test_nvf_builds-0.0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_nvf_builds-0.0.3.6.tar", last modified: Wed May 22 13:21:18 2024, max compression
+gzip compressed data, was "test_nvf_builds-0.0.3.7.tar", last modified: Thu May 23 08:43:35 2024, max compression
```

## Comparing `test_nvf_builds-0.0.3.6.tar` & `test_nvf_builds-0.0.3.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.126642 test_nvf_builds-0.0.3.6/
--rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.6/LICENSE
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-22 13:21:18.126561 test_nvf_builds-0.0.3.6/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.6/README.md
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122629 test_nvf_builds-0.0.3.6/oasysnow/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.6/oasysnow/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122730 test_nvf_builds-0.0.3.6/oasysnow/federated/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.122828 test_nvf_builds-0.0.3.6/oasysnow/federated/client/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123191 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2484 2024-05-16 12:49:15.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2471 2024-05-06 15:57:38.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123413 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4653 2024-05-15 14:56:42.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/trainer.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123567 test_nvf_builds-0.0.3.6/oasysnow/federated/common/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.123887 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1596 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/server.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1324 2024-05-15 14:50:41.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/verification.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124290 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/gennet_model.py
--rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/global_model.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124437 test_nvf_builds-0.0.3.6/oasysnow/federated/server/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/__init__.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.124817 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2501 2024-05-15 14:51:04.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_data.py
--rw-r--r--   0 mostafa    (501) staff       (20)     2475 2024-04-19 21:41:54.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_results.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.125087 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/model_runner.py
--rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.6/requirements.txt
--rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-22 13:21:18.126897 test_nvf_builds-0.0.3.6/setup.cfg
--rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.6/setup.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-22 13:21:18.126320 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/requires.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-22 13:21:18.000000 test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.872050 test_nvf_builds-0.0.3.7/
+-rw-r--r--   0 mostafa    (501) staff       (20)    11357 2024-05-07 07:57:47.000000 test_nvf_builds-0.0.3.7/LICENSE
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 08:43:35.871952 test_nvf_builds-0.0.3.7/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)       85 2024-05-06 07:53:59.000000 test_nvf_builds-0.0.3.7/README.md
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868681 test_nvf_builds-0.0.3.7/oasysnow/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:25.000000 test_nvf_builds-0.0.3.7/oasysnow/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868776 test_nvf_builds-0.0.3.7/oasysnow/federated/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:50:57.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.868872 test_nvf_builds-0.0.3.7/oasysnow/federated/client/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:25:11.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869198 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:35.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2241 2024-05-23 08:40:50.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2190 2024-05-23 08:41:25.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869418 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 10:44:41.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4477 2024-05-23 08:41:46.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/trainer.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869547 test_nvf_builds-0.0.3.7/oasysnow/federated/common/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-15 14:50:33.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.869868 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-03 14:56:34.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1707 2024-05-23 08:37:40.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/server.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1338 2024-05-23 08:42:14.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/verification.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870199 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:36:02.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1803 2024-05-15 14:55:57.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/gennet_model.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     1288 2024-05-15 14:55:47.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/global_model.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870321 test_nvf_builds-0.0.3.7/oasysnow/federated/server/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:11.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/__init__.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870657 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:44:45.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2311 2024-05-23 08:42:28.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_data.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     2132 2024-05-23 08:42:43.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_results.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.870875 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2024-05-02 11:45:46.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)     4843 2024-05-15 14:56:24.000000 test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/model_runner.py
+-rw-r--r--   0 mostafa    (501) staff       (20)       29 2024-05-15 14:24:19.000000 test_nvf_builds-0.0.3.7/requirements.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)      479 2024-05-23 08:43:35.872558 test_nvf_builds-0.0.3.7/setup.cfg
+-rw-r--r--   0 mostafa    (501) staff       (20)      322 2024-05-06 15:10:01.000000 test_nvf_builds-0.0.3.7/setup.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2024-05-23 08:43:35.871721 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)      480 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)     1220 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       28 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/requires.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        9 2024-05-23 08:43:35.000000 test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/top_level.txt
```

### Comparing `test_nvf_builds-0.0.3.6/LICENSE` & `test_nvf_builds-0.0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_data.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,11 +46,9 @@
 
         attestation_service = VerificationServer(audience=client_name, nonces=[nonce])
         verified_attestation = attestation_service.verify(attestation_report)
         if not verified_attestation:
             raise Exception("Attestation Failed: Invalid report")
 
         # TODO: replace dxo.get_meta_prop with direct fl_ctx.get_peer_context
-        test_props = fl_ctx.get_peer_context().get_prop("test")
-        print(f"\n>>>>>>> FILTER_DATA_CLIENT client_name: {client_name}; current_round: {current_round}; nonce: {nonce} server_nonce: {server_nonce}; test_props: {test_props}\n")
 
         return shareable
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/client/filters/filter_results.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/client/filters/filter_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,14 @@
             self.log_debug(fl_ctx, "I cannot handle {}".format(dxo.data_kind))
             return shareable
 
         if dxo.data is None:
             self.log_debug(fl_ctx, "no data to filter")
             return shareable
 
-        client_name = fl_ctx.get_identity_name()
-        current_round = shareable.get_cookie(AppConstants.CONTRIBUTION_ROUND)
-
         public_key_server_bytes = fl_ctx.get_prop(f"server_pk")
         if not public_key_server_bytes:
             raise Exception("Attestation Failed!", public_key_server_bytes)
         server_pk = ser.load_pem_public_key(public_key_server_bytes)
 
         private_key = ec.generate_private_key(ec.SECP384R1())
         public_key_bytes = private_key.public_key().public_bytes(ser.Encoding.PEM, ser.PublicFormat.SubjectPublicKeyInfo)
@@ -50,10 +47,9 @@
         weights = dxo.data
         weights_bytes = pickle.dumps(weights)
         weights_enc = f_client.encrypt(weights_bytes)
 
         dxo.data = {'weights_enc': weights_enc}
         dxo.set_meta_prop("client_pk", public_key_bytes)
 
-        print(f"\n>>>>>>> FILTER_RESULT_CLIENT, client_name: {client_name}; current_round: {current_round}, derived_key_client: {derived_key_client}\n")
 
         return dxo.update_shareable(shareable)
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/client/trainer/trainer.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/client/trainer/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,25 +26,21 @@
         super().__init__()
         self.epochs_per_round = epochs_per_round
         self.train_images, self.train_labels = None, None
         self.test_images, self.test_labels = None, None
         self.model = None
         self.datapath = os.getcwd() + "/"
 
-        print('selfdatapath', self.datapath)
-
 
     def handle_event(self, event_type: str, fl_ctx: FLContext):
         if event_type == EventType.START_RUN:
             self.setup(fl_ctx)
         if event_type == EventType.BEFORE_PULL_TASK :
-            client_name = fl_ctx.get_identity_name()
             r1 = random.randint(0, 100)
             fl_ctx.set_prop("nonce", r1, False, False)
-            print("\n\n\t\t>>>>>> random BEFORE_PULL_TASK", client_name, r1)
 
     def setup(self, fl_ctx: FLContext):
         client_name = fl_ctx.get_identity_name()
 
         scope_properties = fl_ctx.get_prop(FLContextKey.SCOPE_PROPERTIES)
         print(">>>>>>>>>SCOPE", client_name, scope_properties)
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/server.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     def get_custom_attestation(self, nonces: List[str], audience: str):
         token_request = {"nonces": nonces, "audience": audience, "token_type": "OIDC"}
         custom_json = json.dumps(token_request).encode('utf-8')
         self.options["headers"]['Content-Length'] = len(custom_json)
         
         response = self._make_request(custom_json)
+        print(">>>>get_custom_attestation", audience, nonces)
+        print(">>>>AttestationServer", response)
         return response
 
     def _make_request(self, custom_json):
         if "socketPath" in self.options:
             conn = http.client.HTTPConnection(
                 self.options["host"],
                 port=http.client.HTTPConnection.default_port,
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/common/attestation_service/verification.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/common/attestation_service/verification.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 class VerificationServer:
     def __init__(self, audience: str, nonces: List[str]):
         self.audience = audience
         self.nonces = nonces
 
     def verify(self, report: str) -> bool:
         try:
+            print(">>>>report", report)
             issuer_url = "https://confidentialcomputing.googleapis.com/.well-known/openid-configuration"
             issuer = json.loads(requests.get(issuer_url).text)
             jwks_uri = issuer['jwks_uri']
             supported_algs = issuer['id_token_signing_alg_values_supported']
             optional_custom_headers = {"User-agent": "custom-user-agent"}
             supported_algs = issuer['id_token_signing_alg_values_supported']
             jwks_client = jwt.PyJWKClient(jwks_uri, headers=optional_custom_headers)
             signing_key = jwks_client.get_signing_key_from_jwt(report)
             data = jwt.decode(
                 report,
                 signing_key.key,
                 algorithms=supported_algs,
                 audience=self.audience,
             )
-            print(report)
             print(json.dumps(data, indent=2))
             print('>>>>>> Attestation SUCCEEDED')
             return True
         except Exception as e:
             print('>>>>>> Attestation FAILED')
             print(e)
             return False
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/gennet_model.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/gennet_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/common/model/global_model.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/common/model/global_model.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_data.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,15 +31,14 @@
             self.log_debug(fl_ctx, "no data to filter")
             return shareable
 
 
         contributor_name = fl_ctx.get_peer_context().get_identity_name()
         nonce = fl_ctx.get_peer_context().get_prop("nonce")
         current_round = shareable.get_cookie(AppConstants.CONTRIBUTION_ROUND)
-        job_id = fl_ctx.get_job_id()
 
         private_key_server = ec.generate_private_key(ec.SECP384R1())
         public_key_server_bytes = private_key_server.public_key().public_bytes(ser.Encoding.PEM, ser.PublicFormat.SubjectPublicKeyInfo)
 
         attestation_service = AttestationServer()
         # TODO: add the hash of public key of server to the attestation report
         attestation_report = attestation_service.get_custom_attestation(nonces=[nonce], audience=contributor_name)
@@ -49,10 +48,9 @@
         # TODO: replace dxo.get_meta_prop with direct fl_ctx.get_peer_context
         fl_ctx.set_prop(f"test", f"{current_round}:{nonce}", False, False)
 
         dxo.set_meta_prop(f"server_pk_{contributor_name}", public_key_server_bytes)
         dxo.set_meta_prop(f"nonce_{contributor_name}", nonce)
         dxo.set_meta_prop(f"attestation_report_{contributor_name}", attestation_report)
 
-        print(f"\n>>>>>>> FILTER_DATA_SERVER, contributor_name: {contributor_name}; current_round: {current_round}; job_id: {job_id}; nonce: {nonce}\n")
 
         return dxo.update_shareable(shareable)
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/server/filters/filter_results.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/server/filters/filter_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from nvflare.apis.dxo import DXO, DataKind, from_shareable
 from nvflare.apis.filter import Filter
 from nvflare.apis.fl_context import FLContext
 from nvflare.apis.shareable import Shareable
-from nvflare.app_common.app_constant import AppConstants
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 import cryptography.hazmat.primitives.serialization as ser
 import base64
@@ -29,17 +28,15 @@
             self.log_debug(fl_ctx, "I cannot handle {}".format(dxo.data_kind))
             return shareable
 
         if dxo.data is None:
             self.log_debug(fl_ctx, "no data to filter")
             return shareable
 
-        print(">>>>>>>DXO_SERVER", dxo.data)
         contributor_name = fl_ctx.get_peer_context().get_identity_name()
-        current_round = shareable.get_cookie(AppConstants.CONTRIBUTION_ROUND)
 
         client_pk_bytes = dxo.get_meta_prop("client_pk")
         if not client_pk_bytes:
             raise Exception("No public key found for this client")
 
         private_key_server = fl_ctx.get_prop(f"server_sk_{contributor_name}")
         if not private_key_server:
@@ -51,10 +48,9 @@
 
         f_server = Fernet(base64.b64encode(derived_key_server))
         enc_data = dxo.data['weights_enc']
         data_bytes = f_server.decrypt(enc_data)
         weights = pickle.loads(data_bytes)
 
         dxo.data = weights
-        print(f"\n>>>>>>> FILTER_RESULT_SERVER; contributor_name: {contributor_name}, current_round: {current_round}; derived_key_server: {derived_key_server}\n")
 
         return dxo.update_shareable(shareable)
```

### Comparing `test_nvf_builds-0.0.3.6/oasysnow/federated/server/model_runner/model_runner.py` & `test_nvf_builds-0.0.3.7/oasysnow/federated/server/model_runner/model_runner.py`

 * *Files identical despite different names*

### Comparing `test_nvf_builds-0.0.3.6/test_nvf_builds.egg-info/SOURCES.txt` & `test_nvf_builds-0.0.3.7/test_nvf_builds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

