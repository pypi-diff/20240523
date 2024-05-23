# Comparing `tmp/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar.gz` & `tmp/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar", last modified: Tue May 14 02:40:03 2024, max compression
+gzip compressed data, was "dist/antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1.tar", last modified: Thu May 23 02:27:02 2024, max compression
```

## Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0.tar` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/__init__.py
--rw-r--r--   0 root         (0) root         (0)   131808 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py
--rw-r--r--   0 root         (0) root         (0)   201784 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-14 02:40:03.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-05-14 02:40:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   141146 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py
+-rw-r--r--   0 root         (0) root         (0)   212236 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 02:27:02.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-23 02:27:01.000000 antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/setup.py
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/LICENSE` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/PKG-INFO` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_195dff03d395462ea294bafdba69df3f
-Version: 1.3.0
+Version: 1.3.1
 Summary: Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README-CN.md` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/README.md` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-195dff03d395462ea294bafdba69df3f
-Version: 1.3.0
+Version: 1.3.1
 Summary: Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_ak_195dff03d395462ea294bafdba69df3f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.0',
+                    'sdk_version': '1.3.1',
                     '_prod_code': 'ak_195dff03d395462ea294bafdba69df3f',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.0',
+                    'sdk_version': '1.3.1',
                     '_prod_code': 'ak_195dff03d395462ea294bafdba69df3f',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -668,41 +668,41 @@
         )
 
     def create_antchain_ato_withhold_sign(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_antchain_ato_withhold_sign_ex(request, headers, runtime)
 
     async def create_antchain_ato_withhold_sign_async(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_antchain_ato_withhold_sign_ex_async(request, headers, runtime)
 
     def create_antchain_ato_withhold_sign_ex(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse(),
             self.do_request('1.0', 'antchain.ato.withhold.sign.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -710,15 +710,15 @@
     async def create_antchain_ato_withhold_sign_ex_async(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntchainAtoWithholdSignResponse(),
             await self.do_request_async('1.0', 'antchain.ato.withhold.sign.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -948,58 +948,66 @@
         )
 
     def repay_antchain_ato_withhold_plan(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse:
         """
-        Description: 代扣计划清偿/清欠，通过其他收款后通过子接口通知
-        Summary: 代扣计划清偿/清欠
+        Description: ● 重要说明：
+        ①这个接口是取消订单某一期代扣计划中以其他方式还款的金额，取消之后代扣不再执行该期计划。
+        ②对通过其他方式还款的第三方单号留存;例如：银行流水号或微信流水号。
+        Summary: 单期代扣取消
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.repay_antchain_ato_withhold_plan_ex(request, headers, runtime)
 
     async def repay_antchain_ato_withhold_plan_async(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse:
         """
-        Description: 代扣计划清偿/清欠，通过其他收款后通过子接口通知
-        Summary: 代扣计划清偿/清欠
+        Description: ● 重要说明：
+        ①这个接口是取消订单某一期代扣计划中以其他方式还款的金额，取消之后代扣不再执行该期计划。
+        ②对通过其他方式还款的第三方单号留存;例如：银行流水号或微信流水号。
+        Summary: 单期代扣取消
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.repay_antchain_ato_withhold_plan_ex_async(request, headers, runtime)
 
     def repay_antchain_ato_withhold_plan_ex(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse:
         """
-        Description: 代扣计划清偿/清欠，通过其他收款后通过子接口通知
-        Summary: 代扣计划清偿/清欠
+        Description: ● 重要说明：
+        ①这个接口是取消订单某一期代扣计划中以其他方式还款的金额，取消之后代扣不再执行该期计划。
+        ②对通过其他方式还款的第三方单号留存;例如：银行流水号或微信流水号。
+        Summary: 单期代扣取消
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse(),
             self.do_request('1.0', 'antchain.ato.withhold.plan.repay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def repay_antchain_ato_withhold_plan_ex_async(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse:
         """
-        Description: 代扣计划清偿/清欠，通过其他收款后通过子接口通知
-        Summary: 代扣计划清偿/清欠
+        Description: ● 重要说明：
+        ①这个接口是取消订单某一期代扣计划中以其他方式还款的金额，取消之后代扣不再执行该期计划。
+        ②对通过其他方式还款的第三方单号留存;例如：银行流水号或微信流水号。
+        Summary: 单期代扣取消
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.RepayAntchainAtoWithholdPlanResponse(),
             await self.do_request_async('1.0', 'antchain.ato.withhold.plan.repay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
@@ -2523,14 +2531,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.QueryAntchainAtoWithholdRefundResponse(),
             await self.do_request_async('1.0', 'antchain.ato.withhold.refund.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def update_antchain_ato_trade_userpromise(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_antchain_ato_trade_userpromise_ex(request, headers, runtime)
+
+    async def update_antchain_ato_trade_userpromise_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_antchain_ato_trade_userpromise_ex_async(request, headers, runtime)
+
+    def update_antchain_ato_trade_userpromise_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse(),
+            self.do_request('1.0', 'antchain.ato.trade.userpromise.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_antchain_ato_trade_userpromise_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.UpdateAntchainAtoTradeUserpromiseResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.trade.userpromise.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def notify_antchain_ato_fund_flow(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse:
         """
         Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
         Summary: 资方合同文件已上传确认接口
@@ -2579,14 +2643,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__195dff_03d_395462ea_294bafdba_69df_3f_models.NotifyAntchainAtoFundFlowResponse(),
             await self.do_request_async('1.0', 'antchain.ato.fund.flow.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def sync_antchain_ato_front_indirectorder(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_antchain_ato_front_indirectorder_ex(request, headers, runtime)
+
+    async def sync_antchain_ato_front_indirectorder_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_antchain_ato_front_indirectorder_ex_async(request, headers, runtime)
+
+    def sync_antchain_ato_front_indirectorder_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse(),
+            self.do_request('1.0', 'antchain.ato.front.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_antchain_ato_front_indirectorder_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoFrontIndirectorderResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.front.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_antchain_ato_trade_indirectorder(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_antchain_ato_trade_indirectorder_ex(request, headers, runtime)
+
+    async def sync_antchain_ato_trade_indirectorder_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderRequest,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_antchain_ato_trade_indirectorder_ex_async(request, headers, runtime)
+
+    def sync_antchain_ato_trade_indirectorder_ex(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse(),
+            self.do_request('1.0', 'antchain.ato.trade.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_antchain_ato_trade_indirectorder_ex_async(
+        self,
+        request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__195dff_03d_395462ea_294bafdba_69df_3f_models.SyncAntchainAtoTradeIndirectorderResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.trade.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_antcloud_gatewayx_file_upload(
         self,
         request: ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> ak__195dff_03d_395462ea_294bafdba_69df_3f_models.CreateAntcloudGatewayxFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/antchain_sdk_ak_195dff03d395462ea294bafdba69df3f/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -944,15 +944,14 @@
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
         self.validate_required(self.user_id_type, 'user_id_type')
         self.validate_required(self.user_id_number, 'user_id_number')
         self.validate_required(self.user_name, 'user_name')
         self.validate_required(self.business_scene, 'business_scene')
         self.validate_required(self.template_list, 'template_list')
-        self.validate_required(self.alipay_user_id, 'alipay_user_id')
         if self.alipay_user_id is not None:
             self.validate_max_length(self.alipay_user_id, 'alipay_user_id', 20)
         self.validate_required(self.merchant_name, 'merchant_name')
         if self.merchant_name is not None:
             self.validate_max_length(self.merchant_name, 'merchant_name', 256)
         if self.merchant_tag is not None:
             self.validate_max_length(self.merchant_tag, 'merchant_tag', 32)
@@ -1297,41 +1296,46 @@
         auth_token: str = None,
         product_instance_id: str = None,
         order_id: str = None,
         alipay_merchant_id: str = None,
         alipay_merchant_name: str = None,
         alipay_merchant_service_name: str = None,
         alipay_merchant_service_description: str = None,
+        alipay_user_id: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 订单id 长度不可超过50
         self.order_id = order_id
         # 支付宝商户id，使用签约能力前时候进行向平台申请
         self.alipay_merchant_id = alipay_merchant_id
         # 支付宝商户名称，会展示在支付并签约界面
         self.alipay_merchant_name = alipay_merchant_name
         # 支付宝商户服务名称，会展示在支付并签约界面
         self.alipay_merchant_service_name = alipay_merchant_service_name
         # 支付宝商户服务描述，会展示在支付并签约界面
         self.alipay_merchant_service_description = alipay_merchant_service_description
+        # 支付宝uid，非必填
+        self.alipay_user_id = alipay_user_id
 
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         if self.alipay_merchant_id is not None:
             self.validate_max_length(self.alipay_merchant_id, 'alipay_merchant_id', 20)
         if self.alipay_merchant_name is not None:
             self.validate_max_length(self.alipay_merchant_name, 'alipay_merchant_name', 50)
         if self.alipay_merchant_service_name is not None:
             self.validate_max_length(self.alipay_merchant_service_name, 'alipay_merchant_service_name', 50)
         if self.alipay_merchant_service_description is not None:
             self.validate_max_length(self.alipay_merchant_service_description, 'alipay_merchant_service_description', 150)
+        if self.alipay_user_id is not None:
+            self.validate_max_length(self.alipay_user_id, 'alipay_user_id', 128)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1345,14 +1349,16 @@
             result['alipay_merchant_id'] = self.alipay_merchant_id
         if self.alipay_merchant_name is not None:
             result['alipay_merchant_name'] = self.alipay_merchant_name
         if self.alipay_merchant_service_name is not None:
             result['alipay_merchant_service_name'] = self.alipay_merchant_service_name
         if self.alipay_merchant_service_description is not None:
             result['alipay_merchant_service_description'] = self.alipay_merchant_service_description
+        if self.alipay_user_id is not None:
+            result['alipay_user_id'] = self.alipay_user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -1363,14 +1369,16 @@
             self.alipay_merchant_id = m.get('alipay_merchant_id')
         if m.get('alipay_merchant_name') is not None:
             self.alipay_merchant_name = m.get('alipay_merchant_name')
         if m.get('alipay_merchant_service_name') is not None:
             self.alipay_merchant_service_name = m.get('alipay_merchant_service_name')
         if m.get('alipay_merchant_service_description') is not None:
             self.alipay_merchant_service_description = m.get('alipay_merchant_service_description')
+        if m.get('alipay_user_id') is not None:
+            self.alipay_user_id = m.get('alipay_user_id')
         return self
 
 
 class CreateAntchainAtoWithholdSignResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -1859,26 +1867,26 @@
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 订单id 长度不可超过50
         self.order_id = order_id
         # 第几期
         self.period_num = period_num
-        # 扣款时间
+        # 其他方式还款的时间
         self.gmt_pay = gmt_pay
-        # 清偿清欠金额，单位为分
+        # 取消订单某一期代扣计划中以其他方式还款金额，单位为分
         self.pay_off_amount = pay_off_amount
-        # 清偿清欠方式
+        # 变更其他方式还款
         # WECHAT:微信;
         # BANK:银行
         # ALIPAY:支付宝
         self.pay_off_type = pay_off_type
-        # 清偿清欠单号,通过其他方式清偿的第三方单号;例如银行流水号或微信流水号
+        # 通过其他方式还款单号;例如银行流水号或微信流水号
         self.pay_off_no = pay_off_no
-        # 清偿清欠银行名称,方式为银行时必填
+        # 其他方式还款银行名称，还款方式为银行时必填
         self.pay_off_bank_name = pay_off_bank_name
 
     def validate(self):
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 50)
         self.validate_required(self.period_num, 'period_num')
@@ -1886,18 +1894,16 @@
             self.validate_minimum(self.period_num, 'period_num', 1)
         self.validate_required(self.gmt_pay, 'gmt_pay')
         if self.gmt_pay is not None:
             self.validate_pattern(self.gmt_pay, 'gmt_pay', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         self.validate_required(self.pay_off_amount, 'pay_off_amount')
         if self.pay_off_amount is not None:
             self.validate_minimum(self.pay_off_amount, 'pay_off_amount', 0)
-        self.validate_required(self.pay_off_type, 'pay_off_type')
         if self.pay_off_type is not None:
             self.validate_max_length(self.pay_off_type, 'pay_off_type', 64)
-        self.validate_required(self.pay_off_no, 'pay_off_no')
         if self.pay_off_no is not None:
             self.validate_max_length(self.pay_off_no, 'pay_off_no', 64)
         if self.pay_off_bank_name is not None:
             self.validate_max_length(self.pay_off_bank_name, 'pay_off_bank_name', 64)
 
     def to_map(self):
         _map = super().to_map()
@@ -2085,15 +2091,14 @@
             self.validate_max_length(self.user_id_type, 'user_id_type', 40)
         self.validate_required(self.user_id_number, 'user_id_number')
         self.validate_required(self.user_name, 'user_name')
         self.validate_required(self.business_scene, 'business_scene')
         if self.business_scene is not None:
             self.validate_max_length(self.business_scene, 'business_scene', 200)
         self.validate_required(self.template_list, 'template_list')
-        self.validate_required(self.alipay_user_id, 'alipay_user_id')
         if self.alipay_user_id is not None:
             self.validate_max_length(self.alipay_user_id, 'alipay_user_id', 24)
         self.validate_required(self.merchant_name, 'merchant_name')
         if self.merchant_tag is not None:
             self.validate_max_length(self.merchant_tag, 'merchant_tag', 32)
         self.validate_required(self.merchant_id_type, 'merchant_id_type')
         if self.merchant_id_type is not None:
@@ -5149,14 +5154,148 @@
         if m.get('send_back_amount') is not None:
             self.send_back_amount = m.get('send_back_amount')
         if m.get('gmt_refund_pay') is not None:
             self.gmt_refund_pay = m.get('gmt_refund_pay')
         return self
 
 
+class UpdateAntchainAtoTradeUserpromiseRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        order_id: str = None,
+        merchant_id: str = None,
+        term_idx: int = None,
+        updated_rental_money: int = None,
+        reason: str = None,
+        desc: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单id
+        self.order_id = order_id
+        # 商家社会信用代码
+        self.merchant_id = merchant_id
+        # 修改的用户履约期数
+        self.term_idx = term_idx
+        # 更新后的租金，单位为分
+        # 1234=12.34元
+        self.updated_rental_money = updated_rental_money
+        # 调整原因，枚举
+        # ● A01 : 违章罚金
+        # ● A02 : 水电煤费用
+        self.reason = reason
+        # 调整说明，本说明同步到支付宝账户备注中，需准确填写
+        self.desc = desc
+
+    def validate(self):
+        self.validate_required(self.order_id, 'order_id')
+        if self.order_id is not None:
+            self.validate_max_length(self.order_id, 'order_id', 49)
+        self.validate_required(self.merchant_id, 'merchant_id')
+        if self.merchant_id is not None:
+            self.validate_max_length(self.merchant_id, 'merchant_id', 199)
+        self.validate_required(self.term_idx, 'term_idx')
+        self.validate_required(self.updated_rental_money, 'updated_rental_money')
+        self.validate_required(self.reason, 'reason')
+        if self.reason is not None:
+            self.validate_max_length(self.reason, 'reason', 10)
+        self.validate_required(self.desc, 'desc')
+        if self.desc is not None:
+            self.validate_max_length(self.desc, 'desc', 64)
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.term_idx is not None:
+            result['term_idx'] = self.term_idx
+        if self.updated_rental_money is not None:
+            result['updated_rental_money'] = self.updated_rental_money
+        if self.reason is not None:
+            result['reason'] = self.reason
+        if self.desc is not None:
+            result['desc'] = self.desc
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('term_idx') is not None:
+            self.term_idx = m.get('term_idx')
+        if m.get('updated_rental_money') is not None:
+            self.updated_rental_money = m.get('updated_rental_money')
+        if m.get('reason') is not None:
+            self.reason = m.get('reason')
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
+        return self
+
+
+class UpdateAntchainAtoTradeUserpromiseResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class NotifyAntchainAtoFundFlowRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         merchant_id: str = None,
         order_id: str = None,
@@ -5222,14 +5361,180 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class SyncAntchainAtoFrontIndirectorderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_content: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务参数,json.toString
+        self.biz_content = biz_content
+
+    def validate(self):
+        self.validate_required(self.biz_content, 'biz_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_content is not None:
+            result['biz_content'] = self.biz_content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_content') is not None:
+            self.biz_content = m.get('biz_content')
+        return self
+
+
+class SyncAntchainAtoFrontIndirectorderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class SyncAntchainAtoTradeIndirectorderRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_content: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务参数,json.toString
+        self.biz_content = biz_content
+
+    def validate(self):
+        self.validate_required(self.biz_content, 'biz_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_content is not None:
+            result['biz_content'] = self.biz_content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_content') is not None:
+            self.biz_content = m.get('biz_content')
+        return self
+
+
+class SyncAntchainAtoTradeIndirectorderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
```

### Comparing `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.0/setup.py` & `antchain_ak_195dff03d395462ea294bafdba69df3f-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_195dff03d395462ea294bafdba69df3f.
 
-Created on 14/05/2024
+Created on 23/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_195dff03d395462ea294bafdba69df3f"
 NAME = "antchain_ak_195dff03d395462ea294bafdba69df3f" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_195dff03d395462ea294bafdba69df3f SDK Library for Python"
```

