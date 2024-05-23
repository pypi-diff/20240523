# Comparing `tmp/prelude_sdk-1.7.3.tar.gz` & `tmp/prelude_sdk-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude_sdk-1.7.3.tar", last modified: Thu Apr 25 22:31:47 2024, max compression
+gzip compressed data, was "prelude_sdk-1.7.4.tar", last modified: Thu May 23 12:53:08 2024, max compression
```

## Comparing `prelude_sdk-1.7.3.tar` & `prelude_sdk-1.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.276436 prelude_sdk-1.7.3/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-25 22:31:47.276377 prelude_sdk-1.7.3/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude_sdk-1.7.3/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.269545 prelude_sdk-1.7.3/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.272638 prelude_sdk-1.7.3/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     6020 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6626 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     1080 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/generate_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      580 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/http_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     8288 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3727 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      559 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.273334 prelude_sdk-1.7.3/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude_sdk-1.7.3/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     4564 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.276036 prelude_sdk-1.7.3/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      865 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-25 22:31:47.000000 prelude_sdk-1.7.3/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_sdk-1.7.3/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-25 22:31:47.276652 prelude_sdk-1.7.3/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.275728 prelude_sdk-1.7.3/tests/
--rw-r--r--   0 pack       (501) staff       (20)     5494 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-25 22:31:47.275880 prelude_sdk-1.7.3/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude_sdk-1.7.3/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10423 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_build.py
--rw-r--r--   0 pack       (501) staff       (20)     6295 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/tests/test_detect.py
--rw-r--r--   0 pack       (501) staff       (20)     1936 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8372 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_iam.py
--rw-r--r--   0 pack       (501) staff       (20)    13032 2024-04-25 18:56:47.000000 prelude_sdk-1.7.3/tests/test_partner.py
--rw-r--r--   0 pack       (501) staff       (20)     4587 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/test_probe.py
--rw-r--r--   0 pack       (501) staff       (20)     2073 2024-04-17 18:29:22.000000 prelude_sdk-1.7.3/tests/testutils.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.838086 prelude_sdk-1.7.4/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_sdk-1.7.4/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-05-23 12:53:08.838002 prelude_sdk-1.7.4/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude_sdk-1.7.4/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.829632 prelude_sdk-1.7.4/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.4/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.832983 prelude_sdk-1.7.4/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     6020 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6626 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     1080 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/generate_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      580 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/http_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     8240 2024-05-22 22:38:32.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3727 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      559 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.833624 prelude_sdk-1.7.4/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.4/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude_sdk-1.7.4/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     4563 2024-05-23 12:45:08.000000 prelude_sdk-1.7.4/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.837781 prelude_sdk-1.7.4/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-05-23 12:53:08.000000 prelude_sdk-1.7.4/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      865 2024-05-23 12:53:08.000000 prelude_sdk-1.7.4/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-05-23 12:53:08.000000 prelude_sdk-1.7.4/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2024-05-23 12:53:08.000000 prelude_sdk-1.7.4/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-05-23 12:53:08.000000 prelude_sdk-1.7.4/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_sdk-1.7.4/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2024-05-23 12:53:08.838307 prelude_sdk-1.7.4/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.836470 prelude_sdk-1.7.4/tests/
+-rw-r--r--   0 pack       (501) staff       (20)     5499 2024-05-22 22:38:32.000000 prelude_sdk-1.7.4/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:08.836638 prelude_sdk-1.7.4/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude_sdk-1.7.4/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10423 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/tests/test_build.py
+-rw-r--r--   0 pack       (501) staff       (20)     6295 2024-04-25 18:56:47.000000 prelude_sdk-1.7.4/tests/test_detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2077 2024-05-20 17:59:14.000000 prelude_sdk-1.7.4/tests/test_generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8383 2024-05-22 22:38:32.000000 prelude_sdk-1.7.4/tests/test_iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    13018 2024-05-03 19:12:34.000000 prelude_sdk-1.7.4/tests/test_partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     4587 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/tests/test_probe.py
+-rw-r--r--   0 pack       (501) staff       (20)     2073 2024-04-17 18:29:22.000000 prelude_sdk-1.7.4/tests/testutils.py
```

### Comparing `prelude_sdk-1.7.3/LICENSE` & `prelude_sdk-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/PKG-INFO` & `prelude_sdk-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_sdk-1.7.3/README.md` & `prelude_sdk-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/build_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/detect_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/generate_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/generate_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/http_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/http_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/iam_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/iam_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,18 @@
 class IAMController(HttpController):
 
     def __init__(self, account):
         super().__init__()
         self.account = account
 
     @verify_credentials
-    def new_account(self, user_email: str, user_name: str = None, company: str = None, slug: str = None):
-        body = dict(handle=user_email)
+    def new_account(self, user_email: str, company: str, user_name: str = None, slug: str = None):
+        body = dict(handle=user_email, company=company)
         if user_name:
             body['user_name'] = user_name
-        if company:
-            body['company'] = company
         if slug:
             body['slug'] = slug
 
         res = self._session.post(
             url=f'{self.account.hq}/iam/account',
             json=body,
             headers=self.account.headers,
```

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/partner_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/controllers/probe_controller.py` & `prelude_sdk-1.7.4/prelude_sdk/controllers/probe_controller.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/models/account.py` & `prelude_sdk-1.7.4/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/prelude_sdk/models/codes.py` & `prelude_sdk-1.7.4/prelude_sdk/models/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,24 +71,24 @@
     TIMED_OUT = 102
     FAILED_CLEANUP = 103
     TEST_NOT_RELEVANT = 104
     DYNAMIC_QUARANTINE = 105
     BLOCKED_AT_PERIMETER = 106
     EXPLOIT_PREVENTED = 107
     ENDPOINT_NOT_RELEVANT = 108
-    OS_PREVENTED_EXECUTION = 126
+    PREVENTED_EXECUTION = 126
     STATIC_QUARANTINE = 127
     BLOCKED = 137
     UNEXPECTED_ERROR = 256
 
     @classmethod
     def _missing_(cls, value):
         if value and not isinstance(value, int):
             return cls(int(value))
-        logging.warning('Unknown ExitCode: %d', value)
+        logging.warning('Unknown ExitCode: %s', str(value))
         return ExitCode.MISSING
 
     @property
     def state(self):
         for k, v in State.mapping().items():
             if self in v:
                 return k
@@ -119,15 +119,15 @@
                 ExitCode.TEST_NOT_RELEVANT,
             ],
             State.PROTECTED: [
                 ExitCode.BLOCKED,
                 ExitCode.BLOCKED_AT_PERIMETER,
                 ExitCode.DYNAMIC_QUARANTINE,
                 ExitCode.EXPLOIT_PREVENTED,
-                ExitCode.OS_PREVENTED_EXECUTION,
+                ExitCode.PREVENTED_EXECUTION,
                 ExitCode.PROCESS_BLOCKED,
                 ExitCode.PROCESS_BLOCKED_GRACEFULLY,
                 ExitCode.PROTECTED,
                 ExitCode.STATIC_QUARANTINE,
             ],
             State.UNPROTECTED: [
                 ExitCode.UNPROTECTED,
```

### Comparing `prelude_sdk-1.7.3/prelude_sdk.egg-info/PKG-INFO` & `prelude_sdk-1.7.4/prelude_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.3
+Version: 1.7.4
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude_sdk-1.7.3/prelude_sdk.egg-info/SOURCES.txt` & `prelude_sdk-1.7.4/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/setup.cfg` & `prelude_sdk-1.7.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.7.3
+version = 1.7.4
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude_sdk-1.7.3/tests/conftest.py` & `prelude_sdk-1.7.4/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     if existing_account:
         pytest.account.headers['account'] = existing_account['account_id']
         pytest.account.headers['token'] = existing_account['token']
         print(f'[account_id: {existing_account["account_id"]}]', end=' ')
         pytest.expected_account = unwrap(iam.get_account)(iam)
         return
 
-    res = unwrap(iam.new_account)(iam, user_email=email, user_name='Bob')
+    res = unwrap(iam.new_account)(iam, company='pysdk-tests', user_email=email, user_name='Bob')
     if manual:
         with pause_for_manual_action:
             input("Press ENTER to continue testing after verifying the account...\n")
 
     pytest.account.headers['account'] = res['account_id']
     pytest.account.headers['token'] = res['token']
     print(f'[account_id: {res["account_id"]}]', end=' ')
@@ -139,14 +139,13 @@
     title: Suspicious Command Line Usage in Windows
     description: Detects suspicious use of cmd.exe or powershell.exe with commands often used for reconnaissance like directory listing, tree viewing, or searching for sensitive files.
     logsource:
         category: process_creation
         product: windows
     detection:
         selection:
-            ParentImage:
-                - 'cmd.exe'
+            ParentImage: 'cmd.exe'
         condition: selection
     level: medium
     """
 
     pytest.expected_detection = unwrap(build.create_detection)(build, rule=pytest.detection_rule, test_id=pytest.test_id, detection_id=pytest.detection_id, rule_id=str(uuid.uuid4()))
```

### Comparing `prelude_sdk-1.7.3/tests/test_build.py` & `prelude_sdk-1.7.4/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/tests/test_detect.py` & `prelude_sdk-1.7.4/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/tests/test_generate.py` & `prelude_sdk-1.7.4/tests/test_generate.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,17 +33,19 @@
     def test_get_threat_intel(self, unwrap):
         while True:
             time.sleep(5)
             res = unwrap(self.generate.get_threat_intel)(self.generate, job_id=pytest.job_id)
             match status := res.get('status'):
                 case 'RUNNING':
                     if res['step'] == 'GENERATE':
-                        assert 9 == res['num_tasks'], json.dumps(res)
+                        assert 2 == res['num_tasks'], json.dumps(res)
                 case 'COMPLETE':
-                    assert 9 == len(res['output']), json.dumps(res)
-                    assert {'go_code', 'name', 'sigma_rules', 'status', 'technique'} == set(res['output'][0].keys()), json.dumps(res)
+                    assert 14 == len(res['output']), json.dumps(res)
+                    for output in res['output']:
+                        assert {'status', 'technique'} < set(output.keys()), json.dumps(output)
+                        assert 'ai_generated' in output or 'existing_test' in output or 'excluded' in output, json.dumps(output)
                     return
                 case 'FAILED':
                     assert False, f'threat_gen FAILED: {json.dumps(res)}'
                 case _:
                     assert False, f' Unexpected status: {status}\n Response: {json.dumps(res)}'
```

### Comparing `prelude_sdk-1.7.3/tests/test_iam.py` & `prelude_sdk-1.7.4/tests/test_iam.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         assert check_if_string_is_uuid(pytest.account.headers['token'])
         assert email == created['whoami']
 
         pytest.expected_account = dict(
             account_id=created['account_id'],
             whoami=email,
             slug=created['account_id'],
-            company='',
+            company='pysdk-tests',
             mode=Mode.AUTOPILOT.value,
             controls=[],
             users=[
                 dict(
                     handle=email,
                     permission=Permission.ADMIN.value,
                     name='Bob',
```

### Comparing `prelude_sdk-1.7.3/tests/test_partner.py` & `prelude_sdk-1.7.4/tests/test_partner.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             pytest.skip("DETECTIONS feature not enabled")
 
         res = unwrap(self.partner.block)(self.partner, partner=control, test_id=pytest.test_id)
         if control == Control.CROWDSTRIKE:
             assert 1 == len(res)
             assert pytest.expected_detection['rule']['logsource']['product'] == res[0]['platform']
             assert 1 == len(res[0]['rules'])
-            assert f'{pytest.expected_detection["rule"]["title"]} ({pytest.detection_id[:8]}) (0)' == res[0]['rules'][0]['name']
+            assert f'{pytest.expected_test["name"]} ({pytest.detection_id[:8]}) (0)' == res[0]['rules'][0]['name']
             assert res[0]['rules'][0]['status'] in ['ALREADY_EXISTS', 'CREATED']
         else:
             assert 5 == len(res)
             assert {'file', 'ioc_id'} == res[0].keys()
             assert res[0]['file'].startswith(pytest.test_id)
 
     def test_detach(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
```

### Comparing `prelude_sdk-1.7.3/tests/test_probe.py` & `prelude_sdk-1.7.4/tests/test_probe.py`

 * *Files identical despite different names*

### Comparing `prelude_sdk-1.7.3/tests/testutils.py` & `prelude_sdk-1.7.4/tests/testutils.py`

 * *Files identical despite different names*

