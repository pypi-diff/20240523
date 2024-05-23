# Comparing `tmp/antchain_ato-1.7.26.tar.gz` & `tmp/antchain_ato-1.8.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ato-1.7.26.tar", last modified: Thu May  9 03:45:48 2024, max compression
+gzip compressed data, was "dist/antchain_ato-1.8.51.tar", last modified: Thu May 23 14:09:12 2024, max compression
```

## Comparing `antchain_ato-1.7.26.tar` & `antchain_ato-1.8.51.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_ato.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/antchain_sdk_ato/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126392 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/client.py
--rw-r--r--   0 root         (0) root         (0)   247593 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/antchain_sdk_ato/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 03:45:48.000000 antchain_ato-1.7.26/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2489 2024-05-09 03:45:47.000000 antchain_ato-1.7.26/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_ato.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/antchain_sdk_ato/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/antchain_sdk_ato/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   221086 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/antchain_sdk_ato/client.py
+-rw-r--r--   0 root         (0) root         (0)   444129 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/antchain_sdk_ato/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 14:09:12.000000 antchain_ato-1.8.51/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-05-23 14:09:11.000000 antchain_ato-1.8.51/setup.py
```

### Comparing `antchain_ato-1.7.26/LICENSE` & `antchain_ato-1.8.51/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.26/PKG-INFO` & `antchain_ato-1.8.51/antchain_ato.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_ato
-Version: 1.7.26
+Name: antchain-ato
+Version: 1.8.51
 Summary: Ant Chain ATO SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ato-1.7.26/README-CN.md` & `antchain_ato-1.8.51/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.26/README.md` & `antchain_ato-1.8.51/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ato-1.7.26/antchain_ato.egg-info/PKG-INFO` & `antchain_ato-1.8.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-ato
-Version: 1.7.26
+Name: antchain_ato
+Version: 1.8.51
 Summary: Ant Chain ATO SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ato-1.7.26/antchain_sdk_ato/client.py` & `antchain_ato-1.8.51/antchain_sdk_ato/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 订单还款计划
+            # 文件信息
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.26',
+                    'sdk_version': '1.8.51',
                     '_prod_code': 'ATO',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -210,15 +210,15 @@
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
                 'policy': UtilClient.default_string(runtime.backoff_policy, 'no'),
                 'period': UtilClient.default_number(runtime.backoff_period, 1)
             },
             'ignoreSSL': runtime.ignore_ssl,
-            # 订单还款计划
+            # 文件信息
         }
         _last_request = None
         _last_exception = None
         _now = time.time()
         _retry_times = 0
         while TeaCore.allow_retry(_runtime.get('retry'), _retry_times, _now):
             if _retry_times > 0:
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.7.26',
+                    'sdk_version': '1.8.51',
                     '_prod_code': 'ATO',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1257,14 +1257,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.GetFundOrderfullinfoResponse(),
             await self.do_request_async('1.0', 'antchain.ato.fund.orderfullinfo.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def notify_fund_flow(
+        self,
+        request: ato_models.NotifyFundFlowRequest,
+    ) -> ato_models.NotifyFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.notify_fund_flow_ex(request, headers, runtime)
+
+    async def notify_fund_flow_async(
+        self,
+        request: ato_models.NotifyFundFlowRequest,
+    ) -> ato_models.NotifyFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.notify_fund_flow_ex_async(request, headers, runtime)
+
+    def notify_fund_flow_ex(
+        self,
+        request: ato_models.NotifyFundFlowRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.NotifyFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.NotifyFundFlowResponse(),
+            self.do_request('1.0', 'antchain.ato.fund.flow.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def notify_fund_flow_ex_async(
+        self,
+        request: ato_models.NotifyFundFlowRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.NotifyFundFlowResponse:
+        """
+        Description: 用于资方将盖章后的合同文件上传给ISV后，ISV通过该接口通知资方已上传合同
+        Summary: 资方合同文件已上传确认接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.NotifyFundFlowResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.fund.flow.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def get_inner_product(
         self,
         request: ato_models.GetInnerProductRequest,
     ) -> ato_models.GetInnerProductResponse:
         """
         Description: 内部调用,商品信息获取
         Summary: 商品信息获取
@@ -1481,14 +1537,2030 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.SyncInnerMeterforagsignResponse(),
             await self.do_request_async('1.0', 'antchain.ato.inner.meterforagsign.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def all_inner_template(
+        self,
+        request: ato_models.AllInnerTemplateRequest,
+    ) -> ato_models.AllInnerTemplateResponse:
+        """
+        Description: 内部接口，根据租户查询合同模板列表
+        Summary: 查询模板列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.all_inner_template_ex(request, headers, runtime)
+
+    async def all_inner_template_async(
+        self,
+        request: ato_models.AllInnerTemplateRequest,
+    ) -> ato_models.AllInnerTemplateResponse:
+        """
+        Description: 内部接口，根据租户查询合同模板列表
+        Summary: 查询模板列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.all_inner_template_ex_async(request, headers, runtime)
+
+    def all_inner_template_ex(
+        self,
+        request: ato_models.AllInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.AllInnerTemplateResponse:
+        """
+        Description: 内部接口，根据租户查询合同模板列表
+        Summary: 查询模板列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.AllInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.all', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def all_inner_template_ex_async(
+        self,
+        request: ato_models.AllInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.AllInnerTemplateResponse:
+        """
+        Description: 内部接口，根据租户查询合同模板列表
+        Summary: 查询模板列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.AllInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.all', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_inner_template(
+        self,
+        request: ato_models.ListInnerTemplateRequest,
+    ) -> ato_models.ListInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询合同模板版本列表
+        Summary: 查询魔法库某一模板版本列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_inner_template_ex(request, headers, runtime)
+
+    async def list_inner_template_async(
+        self,
+        request: ato_models.ListInnerTemplateRequest,
+    ) -> ato_models.ListInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询合同模板版本列表
+        Summary: 查询魔法库某一模板版本列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_inner_template_ex_async(request, headers, runtime)
+
+    def list_inner_template_ex(
+        self,
+        request: ato_models.ListInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.ListInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询合同模板版本列表
+        Summary: 查询魔法库某一模板版本列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.ListInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_inner_template_ex_async(
+        self,
+        request: ato_models.ListInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.ListInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询合同模板版本列表
+        Summary: 查询魔法库某一模板版本列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.ListInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_inner_template(
+        self,
+        request: ato_models.DetailInnerTemplateRequest,
+    ) -> ato_models.DetailInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询指定版本的模板详情
+        Summary: 查询魔法库模板详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_inner_template_ex(request, headers, runtime)
+
+    async def detail_inner_template_async(
+        self,
+        request: ato_models.DetailInnerTemplateRequest,
+    ) -> ato_models.DetailInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询指定版本的模板详情
+        Summary: 查询魔法库模板详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_inner_template_ex_async(request, headers, runtime)
+
+    def detail_inner_template_ex(
+        self,
+        request: ato_models.DetailInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DetailInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询指定版本的模板详情
+        Summary: 查询魔法库模板详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DetailInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_inner_template_ex_async(
+        self,
+        request: ato_models.DetailInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DetailInnerTemplateResponse:
+        """
+        Description: 内部接口，根据模板code查询指定版本的模板详情
+        Summary: 查询魔法库模板详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DetailInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_inner_template(
+        self,
+        request: ato_models.CreateInnerTemplateRequest,
+    ) -> ato_models.CreateInnerTemplateResponse:
+        """
+        Description: 内部接口，创建魔法库模板
+        Summary: 创建模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_inner_template_ex(request, headers, runtime)
+
+    async def create_inner_template_async(
+        self,
+        request: ato_models.CreateInnerTemplateRequest,
+    ) -> ato_models.CreateInnerTemplateResponse:
+        """
+        Description: 内部接口，创建魔法库模板
+        Summary: 创建模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_inner_template_ex_async(request, headers, runtime)
+
+    def create_inner_template_ex(
+        self,
+        request: ato_models.CreateInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerTemplateResponse:
+        """
+        Description: 内部接口，创建魔法库模板
+        Summary: 创建模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_inner_template_ex_async(
+        self,
+        request: ato_models.CreateInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerTemplateResponse:
+        """
+        Description: 内部接口，创建魔法库模板
+        Summary: 创建模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def save_inner_template(
+        self,
+        request: ato_models.SaveInnerTemplateRequest,
+    ) -> ato_models.SaveInnerTemplateResponse:
+        """
+        Description: 内部接口，保存魔法库模板
+        Summary: 保存魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.save_inner_template_ex(request, headers, runtime)
+
+    async def save_inner_template_async(
+        self,
+        request: ato_models.SaveInnerTemplateRequest,
+    ) -> ato_models.SaveInnerTemplateResponse:
+        """
+        Description: 内部接口，保存魔法库模板
+        Summary: 保存魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.save_inner_template_ex_async(request, headers, runtime)
+
+    def save_inner_template_ex(
+        self,
+        request: ato_models.SaveInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SaveInnerTemplateResponse:
+        """
+        Description: 内部接口，保存魔法库模板
+        Summary: 保存魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SaveInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def save_inner_template_ex_async(
+        self,
+        request: ato_models.SaveInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SaveInnerTemplateResponse:
+        """
+        Description: 内部接口，保存魔法库模板
+        Summary: 保存魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SaveInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def save_inner_signfields(
+        self,
+        request: ato_models.SaveInnerSignfieldsRequest,
+    ) -> ato_models.SaveInnerSignfieldsResponse:
+        """
+        Description: 内部接口，保存魔法库模板签署区
+        Summary: 保存魔法库模板签署区
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.save_inner_signfields_ex(request, headers, runtime)
+
+    async def save_inner_signfields_async(
+        self,
+        request: ato_models.SaveInnerSignfieldsRequest,
+    ) -> ato_models.SaveInnerSignfieldsResponse:
+        """
+        Description: 内部接口，保存魔法库模板签署区
+        Summary: 保存魔法库模板签署区
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.save_inner_signfields_ex_async(request, headers, runtime)
+
+    def save_inner_signfields_ex(
+        self,
+        request: ato_models.SaveInnerSignfieldsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SaveInnerSignfieldsResponse:
+        """
+        Description: 内部接口，保存魔法库模板签署区
+        Summary: 保存魔法库模板签署区
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SaveInnerSignfieldsResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.signfields.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def save_inner_signfields_ex_async(
+        self,
+        request: ato_models.SaveInnerSignfieldsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SaveInnerSignfieldsResponse:
+        """
+        Description: 内部接口，保存魔法库模板签署区
+        Summary: 保存魔法库模板签署区
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SaveInnerSignfieldsResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.signfields.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def publish_inner_template(
+        self,
+        request: ato_models.PublishInnerTemplateRequest,
+    ) -> ato_models.PublishInnerTemplateResponse:
+        """
+        Description: 内部接口，发布魔法库模板
+        Summary: 发布魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.publish_inner_template_ex(request, headers, runtime)
+
+    async def publish_inner_template_async(
+        self,
+        request: ato_models.PublishInnerTemplateRequest,
+    ) -> ato_models.PublishInnerTemplateResponse:
+        """
+        Description: 内部接口，发布魔法库模板
+        Summary: 发布魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.publish_inner_template_ex_async(request, headers, runtime)
+
+    def publish_inner_template_ex(
+        self,
+        request: ato_models.PublishInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PublishInnerTemplateResponse:
+        """
+        Description: 内部接口，发布魔法库模板
+        Summary: 发布魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PublishInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.publish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def publish_inner_template_ex_async(
+        self,
+        request: ato_models.PublishInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PublishInnerTemplateResponse:
+        """
+        Description: 内部接口，发布魔法库模板
+        Summary: 发布魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PublishInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.publish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def preview_inner_template(
+        self,
+        request: ato_models.PreviewInnerTemplateRequest,
+    ) -> ato_models.PreviewInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code预览对应魔法库模板
+        Summary: 预览魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.preview_inner_template_ex(request, headers, runtime)
+
+    async def preview_inner_template_async(
+        self,
+        request: ato_models.PreviewInnerTemplateRequest,
+    ) -> ato_models.PreviewInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code预览对应魔法库模板
+        Summary: 预览魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.preview_inner_template_ex_async(request, headers, runtime)
+
+    def preview_inner_template_ex(
+        self,
+        request: ato_models.PreviewInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PreviewInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code预览对应魔法库模板
+        Summary: 预览魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PreviewInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def preview_inner_template_ex_async(
+        self,
+        request: ato_models.PreviewInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PreviewInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code预览对应魔法库模板
+        Summary: 预览魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PreviewInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def delete_inner_template(
+        self,
+        request: ato_models.DeleteInnerTemplateRequest,
+    ) -> ato_models.DeleteInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code删除对应魔法库模板
+        Summary: 删除魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_inner_template_ex(request, headers, runtime)
+
+    async def delete_inner_template_async(
+        self,
+        request: ato_models.DeleteInnerTemplateRequest,
+    ) -> ato_models.DeleteInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code删除对应魔法库模板
+        Summary: 删除魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_inner_template_ex_async(request, headers, runtime)
+
+    def delete_inner_template_ex(
+        self,
+        request: ato_models.DeleteInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DeleteInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code删除对应魔法库模板
+        Summary: 删除魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DeleteInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def delete_inner_template_ex_async(
+        self,
+        request: ato_models.DeleteInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DeleteInnerTemplateResponse:
+        """
+        Description: 内部接口，根据code删除对应魔法库模板
+        Summary: 删除魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DeleteInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def clone_inner_template(
+        self,
+        request: ato_models.CloneInnerTemplateRequest,
+    ) -> ato_models.CloneInnerTemplateResponse:
+        """
+        Description: 内部接口，复制一个魔法库模板
+        Summary: 复制魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.clone_inner_template_ex(request, headers, runtime)
+
+    async def clone_inner_template_async(
+        self,
+        request: ato_models.CloneInnerTemplateRequest,
+    ) -> ato_models.CloneInnerTemplateResponse:
+        """
+        Description: 内部接口，复制一个魔法库模板
+        Summary: 复制魔法库模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.clone_inner_template_ex_async(request, headers, runtime)
+
+    def clone_inner_template_ex(
+        self,
+        request: ato_models.CloneInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CloneInnerTemplateResponse:
+        """
+        Description: 内部接口，复制一个魔法库模板
+        Summary: 复制魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CloneInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.clone', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def clone_inner_template_ex_async(
+        self,
+        request: ato_models.CloneInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CloneInnerTemplateResponse:
+        """
+        Description: 内部接口，复制一个魔法库模板
+        Summary: 复制魔法库模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CloneInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.clone', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_inner_file(
+        self,
+        request: ato_models.UploadInnerFileRequest,
+    ) -> ato_models.UploadInnerFileResponse:
+        """
+        Description: ato文件上传
+        Summary: ato文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_inner_file_ex(request, headers, runtime)
+
+    async def upload_inner_file_async(
+        self,
+        request: ato_models.UploadInnerFileRequest,
+    ) -> ato_models.UploadInnerFileResponse:
+        """
+        Description: ato文件上传
+        Summary: ato文件上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_inner_file_ex_async(request, headers, runtime)
+
+    def upload_inner_file_ex(
+        self,
+        request: ato_models.UploadInnerFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadInnerFileResponse:
+        """
+        Description: ato文件上传
+        Summary: ato文件上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadInnerFileResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.file.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_inner_file_ex_async(
+        self,
+        request: ato_models.UploadInnerFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadInnerFileResponse:
+        """
+        Description: ato文件上传
+        Summary: ato文件上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadInnerFileResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.file.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def download_inner_file(
+        self,
+        request: ato_models.DownloadInnerFileRequest,
+    ) -> ato_models.DownloadInnerFileResponse:
+        """
+        Description: ato文件下载
+        Summary: ato文件下载
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.download_inner_file_ex(request, headers, runtime)
+
+    async def download_inner_file_async(
+        self,
+        request: ato_models.DownloadInnerFileRequest,
+    ) -> ato_models.DownloadInnerFileResponse:
+        """
+        Description: ato文件下载
+        Summary: ato文件下载
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.download_inner_file_ex_async(request, headers, runtime)
+
+    def download_inner_file_ex(
+        self,
+        request: ato_models.DownloadInnerFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DownloadInnerFileResponse:
+        """
+        Description: ato文件下载
+        Summary: ato文件下载
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DownloadInnerFileResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.file.download', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def download_inner_file_ex_async(
+        self,
+        request: ato_models.DownloadInnerFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.DownloadInnerFileResponse:
+        """
+        Description: ato文件下载
+        Summary: ato文件下载
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.DownloadInnerFileResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.file.download', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_inner_templateofficeurl(
+        self,
+        request: ato_models.GetInnerTemplateofficeurlRequest,
+    ) -> ato_models.GetInnerTemplateofficeurlResponse:
+        """
+        Description: 获取 webofficeURL（透传）
+        Summary: 获取 webofficeURL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_inner_templateofficeurl_ex(request, headers, runtime)
+
+    async def get_inner_templateofficeurl_async(
+        self,
+        request: ato_models.GetInnerTemplateofficeurlRequest,
+    ) -> ato_models.GetInnerTemplateofficeurlResponse:
+        """
+        Description: 获取 webofficeURL（透传）
+        Summary: 获取 webofficeURL
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_inner_templateofficeurl_ex_async(request, headers, runtime)
+
+    def get_inner_templateofficeurl_ex(
+        self,
+        request: ato_models.GetInnerTemplateofficeurlRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerTemplateofficeurlResponse:
+        """
+        Description: 获取 webofficeURL（透传）
+        Summary: 获取 webofficeURL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerTemplateofficeurlResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.templateofficeurl.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_inner_templateofficeurl_ex_async(
+        self,
+        request: ato_models.GetInnerTemplateofficeurlRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.GetInnerTemplateofficeurlResponse:
+        """
+        Description: 获取 webofficeURL（透传）
+        Summary: 获取 webofficeURL
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.GetInnerTemplateofficeurlResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.templateofficeurl.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def refresh_inner_templatetoken(
+        self,
+        request: ato_models.RefreshInnerTemplatetokenRequest,
+    ) -> ato_models.RefreshInnerTemplatetokenResponse:
+        """
+        Description: 魔法库控制台刷新token
+        Summary: 刷新token
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.refresh_inner_templatetoken_ex(request, headers, runtime)
+
+    async def refresh_inner_templatetoken_async(
+        self,
+        request: ato_models.RefreshInnerTemplatetokenRequest,
+    ) -> ato_models.RefreshInnerTemplatetokenResponse:
+        """
+        Description: 魔法库控制台刷新token
+        Summary: 刷新token
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.refresh_inner_templatetoken_ex_async(request, headers, runtime)
+
+    def refresh_inner_templatetoken_ex(
+        self,
+        request: ato_models.RefreshInnerTemplatetokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.RefreshInnerTemplatetokenResponse:
+        """
+        Description: 魔法库控制台刷新token
+        Summary: 刷新token
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.RefreshInnerTemplatetokenResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.templatetoken.refresh', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def refresh_inner_templatetoken_ex_async(
+        self,
+        request: ato_models.RefreshInnerTemplatetokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.RefreshInnerTemplatetokenResponse:
+        """
+        Description: 魔法库控制台刷新token
+        Summary: 刷新token
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.RefreshInnerTemplatetokenResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.templatetoken.refresh', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_inner_templatetextarea(
+        self,
+        request: ato_models.CreateInnerTemplatetextareaRequest,
+    ) -> ato_models.CreateInnerTemplatetextareaResponse:
+        """
+        Description: 创建文本域（组件）
+        Summary: 创建文本域
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_inner_templatetextarea_ex(request, headers, runtime)
+
+    async def create_inner_templatetextarea_async(
+        self,
+        request: ato_models.CreateInnerTemplatetextareaRequest,
+    ) -> ato_models.CreateInnerTemplatetextareaResponse:
+        """
+        Description: 创建文本域（组件）
+        Summary: 创建文本域
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_inner_templatetextarea_ex_async(request, headers, runtime)
+
+    def create_inner_templatetextarea_ex(
+        self,
+        request: ato_models.CreateInnerTemplatetextareaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerTemplatetextareaResponse:
+        """
+        Description: 创建文本域（组件）
+        Summary: 创建文本域
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerTemplatetextareaResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.templatetextarea.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_inner_templatetextarea_ex_async(
+        self,
+        request: ato_models.CreateInnerTemplatetextareaRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerTemplatetextareaResponse:
+        """
+        Description: 创建文本域（组件）
+        Summary: 创建文本域
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerTemplatetextareaResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.templatetextarea.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_templateimage(
+        self,
+        request: ato_models.QueryInnerTemplateimageRequest,
+    ) -> ato_models.QueryInnerTemplateimageResponse:
+        """
+        Description: 获取模板的图片列表
+        Summary: 获取模板的图片列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_templateimage_ex(request, headers, runtime)
+
+    async def query_inner_templateimage_async(
+        self,
+        request: ato_models.QueryInnerTemplateimageRequest,
+    ) -> ato_models.QueryInnerTemplateimageResponse:
+        """
+        Description: 获取模板的图片列表
+        Summary: 获取模板的图片列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_templateimage_ex_async(request, headers, runtime)
+
+    def query_inner_templateimage_ex(
+        self,
+        request: ato_models.QueryInnerTemplateimageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerTemplateimageResponse:
+        """
+        Description: 获取模板的图片列表
+        Summary: 获取模板的图片列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerTemplateimageResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.templateimage.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_templateimage_ex_async(
+        self,
+        request: ato_models.QueryInnerTemplateimageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerTemplateimageResponse:
+        """
+        Description: 获取模板的图片列表
+        Summary: 获取模板的图片列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerTemplateimageResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.templateimage.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_inner_funddividerelation(
+        self,
+        request: ato_models.CreateInnerFunddividerelationRequest,
+    ) -> ato_models.CreateInnerFunddividerelationResponse:
+        """
+        Description: 保存/编辑分账关系信息
+        Summary: 保存/编辑分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_inner_funddividerelation_ex(request, headers, runtime)
+
+    async def create_inner_funddividerelation_async(
+        self,
+        request: ato_models.CreateInnerFunddividerelationRequest,
+    ) -> ato_models.CreateInnerFunddividerelationResponse:
+        """
+        Description: 保存/编辑分账关系信息
+        Summary: 保存/编辑分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_inner_funddividerelation_ex_async(request, headers, runtime)
+
+    def create_inner_funddividerelation_ex(
+        self,
+        request: ato_models.CreateInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerFunddividerelationResponse:
+        """
+        Description: 保存/编辑分账关系信息
+        Summary: 保存/编辑分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerFunddividerelationResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.funddividerelation.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_inner_funddividerelation_ex_async(
+        self,
+        request: ato_models.CreateInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerFunddividerelationResponse:
+        """
+        Description: 保存/编辑分账关系信息
+        Summary: 保存/编辑分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerFunddividerelationResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.funddividerelation.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_inner_funddividerelation(
+        self,
+        request: ato_models.SubmitInnerFunddividerelationRequest,
+    ) -> ato_models.SubmitInnerFunddividerelationResponse:
+        """
+        Description: 提交分账关系信息
+        Summary: 提交分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_inner_funddividerelation_ex(request, headers, runtime)
+
+    async def submit_inner_funddividerelation_async(
+        self,
+        request: ato_models.SubmitInnerFunddividerelationRequest,
+    ) -> ato_models.SubmitInnerFunddividerelationResponse:
+        """
+        Description: 提交分账关系信息
+        Summary: 提交分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_inner_funddividerelation_ex_async(request, headers, runtime)
+
+    def submit_inner_funddividerelation_ex(
+        self,
+        request: ato_models.SubmitInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SubmitInnerFunddividerelationResponse:
+        """
+        Description: 提交分账关系信息
+        Summary: 提交分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SubmitInnerFunddividerelationResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.funddividerelation.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_inner_funddividerelation_ex_async(
+        self,
+        request: ato_models.SubmitInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SubmitInnerFunddividerelationResponse:
+        """
+        Description: 提交分账关系信息
+        Summary: 提交分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SubmitInnerFunddividerelationResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.funddividerelation.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_funddividerelation(
+        self,
+        request: ato_models.QueryInnerFunddividerelationRequest,
+    ) -> ato_models.QueryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系信息
+        Summary: 查询分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_funddividerelation_ex(request, headers, runtime)
+
+    async def query_inner_funddividerelation_async(
+        self,
+        request: ato_models.QueryInnerFunddividerelationRequest,
+    ) -> ato_models.QueryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系信息
+        Summary: 查询分账关系信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_funddividerelation_ex_async(request, headers, runtime)
+
+    def query_inner_funddividerelation_ex(
+        self,
+        request: ato_models.QueryInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系信息
+        Summary: 查询分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerFunddividerelationResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.funddividerelation.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_funddividerelation_ex_async(
+        self,
+        request: ato_models.QueryInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系信息
+        Summary: 查询分账关系信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerFunddividerelationResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.funddividerelation.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_inner_funddividerelation(
+        self,
+        request: ato_models.PagequeryInnerFunddividerelationRequest,
+    ) -> ato_models.PagequeryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系分页列表
+        Summary: 查询分账关系分页列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_inner_funddividerelation_ex(request, headers, runtime)
+
+    async def pagequery_inner_funddividerelation_async(
+        self,
+        request: ato_models.PagequeryInnerFunddividerelationRequest,
+    ) -> ato_models.PagequeryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系分页列表
+        Summary: 查询分账关系分页列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_inner_funddividerelation_ex_async(request, headers, runtime)
+
+    def pagequery_inner_funddividerelation_ex(
+        self,
+        request: ato_models.PagequeryInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系分页列表
+        Summary: 查询分账关系分页列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerFunddividerelationResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.funddividerelation.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_inner_funddividerelation_ex_async(
+        self,
+        request: ato_models.PagequeryInnerFunddividerelationRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerFunddividerelationResponse:
+        """
+        Description: 查询分账关系分页列表
+        Summary: 查询分账关系分页列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerFunddividerelationResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.funddividerelation.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_inner_merchantagreement(
+        self,
+        request: ato_models.CreateInnerMerchantagreementRequest,
+    ) -> ato_models.CreateInnerMerchantagreementResponse:
+        """
+        Description: 保存租户签约信息
+        Summary: 保存租户签约信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_inner_merchantagreement_ex(request, headers, runtime)
+
+    async def create_inner_merchantagreement_async(
+        self,
+        request: ato_models.CreateInnerMerchantagreementRequest,
+    ) -> ato_models.CreateInnerMerchantagreementResponse:
+        """
+        Description: 保存租户签约信息
+        Summary: 保存租户签约信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_inner_merchantagreement_ex_async(request, headers, runtime)
+
+    def create_inner_merchantagreement_ex(
+        self,
+        request: ato_models.CreateInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerMerchantagreementResponse:
+        """
+        Description: 保存租户签约信息
+        Summary: 保存租户签约信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerMerchantagreementResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantagreement.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_inner_merchantagreement_ex_async(
+        self,
+        request: ato_models.CreateInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerMerchantagreementResponse:
+        """
+        Description: 保存租户签约信息
+        Summary: 保存租户签约信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerMerchantagreementResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantagreement.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_merchantagreement(
+        self,
+        request: ato_models.QueryInnerMerchantagreementRequest,
+    ) -> ato_models.QueryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约信息
+        Summary: 查询租户签约信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_merchantagreement_ex(request, headers, runtime)
+
+    async def query_inner_merchantagreement_async(
+        self,
+        request: ato_models.QueryInnerMerchantagreementRequest,
+    ) -> ato_models.QueryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约信息
+        Summary: 查询租户签约信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_merchantagreement_ex_async(request, headers, runtime)
+
+    def query_inner_merchantagreement_ex(
+        self,
+        request: ato_models.QueryInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约信息
+        Summary: 查询租户签约信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerMerchantagreementResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantagreement.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_merchantagreement_ex_async(
+        self,
+        request: ato_models.QueryInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约信息
+        Summary: 查询租户签约信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerMerchantagreementResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantagreement.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_inner_merchantagreement(
+        self,
+        request: ato_models.PagequeryInnerMerchantagreementRequest,
+    ) -> ato_models.PagequeryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约协议分页列表
+        Summary: 查询租户签约协议分页列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_inner_merchantagreement_ex(request, headers, runtime)
+
+    async def pagequery_inner_merchantagreement_async(
+        self,
+        request: ato_models.PagequeryInnerMerchantagreementRequest,
+    ) -> ato_models.PagequeryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约协议分页列表
+        Summary: 查询租户签约协议分页列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_inner_merchantagreement_ex_async(request, headers, runtime)
+
+    def pagequery_inner_merchantagreement_ex(
+        self,
+        request: ato_models.PagequeryInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约协议分页列表
+        Summary: 查询租户签约协议分页列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerMerchantagreementResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantagreement.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_inner_merchantagreement_ex_async(
+        self,
+        request: ato_models.PagequeryInnerMerchantagreementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerMerchantagreementResponse:
+        """
+        Description: 查询租户签约协议分页列表
+        Summary: 查询租户签约协议分页列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerMerchantagreementResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantagreement.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_inner_merchantpayexpand(
+        self,
+        request: ato_models.CreateInnerMerchantpayexpandRequest,
+    ) -> ato_models.CreateInnerMerchantpayexpandResponse:
+        """
+        Description: 保存/编辑进件信息
+        Summary: 保存/编辑进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_inner_merchantpayexpand_ex(request, headers, runtime)
+
+    async def create_inner_merchantpayexpand_async(
+        self,
+        request: ato_models.CreateInnerMerchantpayexpandRequest,
+    ) -> ato_models.CreateInnerMerchantpayexpandResponse:
+        """
+        Description: 保存/编辑进件信息
+        Summary: 保存/编辑进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_inner_merchantpayexpand_ex_async(request, headers, runtime)
+
+    def create_inner_merchantpayexpand_ex(
+        self,
+        request: ato_models.CreateInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerMerchantpayexpandResponse:
+        """
+        Description: 保存/编辑进件信息
+        Summary: 保存/编辑进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerMerchantpayexpandResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantpayexpand.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_inner_merchantpayexpand_ex_async(
+        self,
+        request: ato_models.CreateInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CreateInnerMerchantpayexpandResponse:
+        """
+        Description: 保存/编辑进件信息
+        Summary: 保存/编辑进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CreateInnerMerchantpayexpandResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantpayexpand.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_inner_merchantpayexpand(
+        self,
+        request: ato_models.SubmitInnerMerchantpayexpandRequest,
+    ) -> ato_models.SubmitInnerMerchantpayexpandResponse:
+        """
+        Description: 提交进件信息
+        Summary: 提交进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_inner_merchantpayexpand_ex(request, headers, runtime)
+
+    async def submit_inner_merchantpayexpand_async(
+        self,
+        request: ato_models.SubmitInnerMerchantpayexpandRequest,
+    ) -> ato_models.SubmitInnerMerchantpayexpandResponse:
+        """
+        Description: 提交进件信息
+        Summary: 提交进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_inner_merchantpayexpand_ex_async(request, headers, runtime)
+
+    def submit_inner_merchantpayexpand_ex(
+        self,
+        request: ato_models.SubmitInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SubmitInnerMerchantpayexpandResponse:
+        """
+        Description: 提交进件信息
+        Summary: 提交进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SubmitInnerMerchantpayexpandResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantpayexpand.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_inner_merchantpayexpand_ex_async(
+        self,
+        request: ato_models.SubmitInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SubmitInnerMerchantpayexpandResponse:
+        """
+        Description: 提交进件信息
+        Summary: 提交进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SubmitInnerMerchantpayexpandResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantpayexpand.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_merchantpayexpand(
+        self,
+        request: ato_models.QueryInnerMerchantpayexpandRequest,
+    ) -> ato_models.QueryInnerMerchantpayexpandResponse:
+        """
+        Description: 查询进件信息
+        Summary: 查询进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_merchantpayexpand_ex(request, headers, runtime)
+
+    async def query_inner_merchantpayexpand_async(
+        self,
+        request: ato_models.QueryInnerMerchantpayexpandRequest,
+    ) -> ato_models.QueryInnerMerchantpayexpandResponse:
+        """
+        Description: 查询进件信息
+        Summary: 查询进件信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_merchantpayexpand_ex_async(request, headers, runtime)
+
+    def query_inner_merchantpayexpand_ex(
+        self,
+        request: ato_models.QueryInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerMerchantpayexpandResponse:
+        """
+        Description: 查询进件信息
+        Summary: 查询进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerMerchantpayexpandResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantpayexpand.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_merchantpayexpand_ex_async(
+        self,
+        request: ato_models.QueryInnerMerchantpayexpandRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerMerchantpayexpandResponse:
+        """
+        Description: 查询进件信息
+        Summary: 查询进件信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerMerchantpayexpandResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantpayexpand.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_inner_merchantagent(
+        self,
+        request: ato_models.PagequeryInnerMerchantagentRequest,
+    ) -> ato_models.PagequeryInnerMerchantagentResponse:
+        """
+        Description: 查询代理商户分页列表-间连商户使用
+        Summary: 查询代理商户分页列表-间连商户使用
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_inner_merchantagent_ex(request, headers, runtime)
+
+    async def pagequery_inner_merchantagent_async(
+        self,
+        request: ato_models.PagequeryInnerMerchantagentRequest,
+    ) -> ato_models.PagequeryInnerMerchantagentResponse:
+        """
+        Description: 查询代理商户分页列表-间连商户使用
+        Summary: 查询代理商户分页列表-间连商户使用
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_inner_merchantagent_ex_async(request, headers, runtime)
+
+    def pagequery_inner_merchantagent_ex(
+        self,
+        request: ato_models.PagequeryInnerMerchantagentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerMerchantagentResponse:
+        """
+        Description: 查询代理商户分页列表-间连商户使用
+        Summary: 查询代理商户分页列表-间连商户使用
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerMerchantagentResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.merchantagent.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_inner_merchantagent_ex_async(
+        self,
+        request: ato_models.PagequeryInnerMerchantagentRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.PagequeryInnerMerchantagentResponse:
+        """
+        Description: 查询代理商户分页列表-间连商户使用
+        Summary: 查询代理商户分页列表-间连商户使用
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.PagequeryInnerMerchantagentResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.merchantagent.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def clone_inner_templatefileaddress(
+        self,
+        request: ato_models.CloneInnerTemplatefileaddressRequest,
+    ) -> ato_models.CloneInnerTemplatefileaddressResponse:
+        """
+        Description: 拷贝模板文件，可用于保存模板的入参
+        Summary: 拷贝模板文件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.clone_inner_templatefileaddress_ex(request, headers, runtime)
+
+    async def clone_inner_templatefileaddress_async(
+        self,
+        request: ato_models.CloneInnerTemplatefileaddressRequest,
+    ) -> ato_models.CloneInnerTemplatefileaddressResponse:
+        """
+        Description: 拷贝模板文件，可用于保存模板的入参
+        Summary: 拷贝模板文件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.clone_inner_templatefileaddress_ex_async(request, headers, runtime)
+
+    def clone_inner_templatefileaddress_ex(
+        self,
+        request: ato_models.CloneInnerTemplatefileaddressRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CloneInnerTemplatefileaddressResponse:
+        """
+        Description: 拷贝模板文件，可用于保存模板的入参
+        Summary: 拷贝模板文件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CloneInnerTemplatefileaddressResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.templatefileaddress.clone', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def clone_inner_templatefileaddress_ex_async(
+        self,
+        request: ato_models.CloneInnerTemplatefileaddressRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.CloneInnerTemplatefileaddressResponse:
+        """
+        Description: 拷贝模板文件，可用于保存模板的入参
+        Summary: 拷贝模板文件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.CloneInnerTemplatefileaddressResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.templatefileaddress.clone', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_signfields(
+        self,
+        request: ato_models.QueryInnerSignfieldsRequest,
+    ) -> ato_models.QueryInnerSignfieldsResponse:
+        """
+        Description: 查询签署区
+        Summary: 查询签署区
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_signfields_ex(request, headers, runtime)
+
+    async def query_inner_signfields_async(
+        self,
+        request: ato_models.QueryInnerSignfieldsRequest,
+    ) -> ato_models.QueryInnerSignfieldsResponse:
+        """
+        Description: 查询签署区
+        Summary: 查询签署区
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_signfields_ex_async(request, headers, runtime)
+
+    def query_inner_signfields_ex(
+        self,
+        request: ato_models.QueryInnerSignfieldsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerSignfieldsResponse:
+        """
+        Description: 查询签署区
+        Summary: 查询签署区
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerSignfieldsResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.signfields.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_signfields_ex_async(
+        self,
+        request: ato_models.QueryInnerSignfieldsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerSignfieldsResponse:
+        """
+        Description: 查询签署区
+        Summary: 查询签署区
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerSignfieldsResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.signfields.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_inner_template(
+        self,
+        request: ato_models.SyncInnerTemplateRequest,
+    ) -> ato_models.SyncInnerTemplateResponse:
+        """
+        Description: 同步已发布的模板
+        Summary: 同步已发布的模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_inner_template_ex(request, headers, runtime)
+
+    async def sync_inner_template_async(
+        self,
+        request: ato_models.SyncInnerTemplateRequest,
+    ) -> ato_models.SyncInnerTemplateResponse:
+        """
+        Description: 同步已发布的模板
+        Summary: 同步已发布的模板
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_inner_template_ex_async(request, headers, runtime)
+
+    def sync_inner_template_ex(
+        self,
+        request: ato_models.SyncInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerTemplateResponse:
+        """
+        Description: 同步已发布的模板
+        Summary: 同步已发布的模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_inner_template_ex_async(
+        self,
+        request: ato_models.SyncInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncInnerTemplateResponse:
+        """
+        Description: 同步已发布的模板
+        Summary: 同步已发布的模板
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def update_inner_template(
+        self,
+        request: ato_models.UpdateInnerTemplateRequest,
+    ) -> ato_models.UpdateInnerTemplateResponse:
+        """
+        Description: 更新魔法库模板基本信息
+        Summary: 更新魔法库模板基本信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_inner_template_ex(request, headers, runtime)
+
+    async def update_inner_template_async(
+        self,
+        request: ato_models.UpdateInnerTemplateRequest,
+    ) -> ato_models.UpdateInnerTemplateResponse:
+        """
+        Description: 更新魔法库模板基本信息
+        Summary: 更新魔法库模板基本信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_inner_template_ex_async(request, headers, runtime)
+
+    def update_inner_template_ex(
+        self,
+        request: ato_models.UpdateInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UpdateInnerTemplateResponse:
+        """
+        Description: 更新魔法库模板基本信息
+        Summary: 更新魔法库模板基本信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UpdateInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_inner_template_ex_async(
+        self,
+        request: ato_models.UpdateInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UpdateInnerTemplateResponse:
+        """
+        Description: 更新魔法库模板基本信息
+        Summary: 更新魔法库模板基本信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UpdateInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_inner_template(
+        self,
+        request: ato_models.QueryInnerTemplateRequest,
+    ) -> ato_models.QueryInnerTemplateResponse:
+        """
+        Description: 通过模板code更新模板的基本信息，比如模板名称等
+        Summary: 查询模板的基本信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_inner_template_ex(request, headers, runtime)
+
+    async def query_inner_template_async(
+        self,
+        request: ato_models.QueryInnerTemplateRequest,
+    ) -> ato_models.QueryInnerTemplateResponse:
+        """
+        Description: 通过模板code更新模板的基本信息，比如模板名称等
+        Summary: 查询模板的基本信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_inner_template_ex_async(request, headers, runtime)
+
+    def query_inner_template_ex(
+        self,
+        request: ato_models.QueryInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerTemplateResponse:
+        """
+        Description: 通过模板code更新模板的基本信息，比如模板名称等
+        Summary: 查询模板的基本信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.inner.template.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_inner_template_ex_async(
+        self,
+        request: ato_models.QueryInnerTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryInnerTemplateResponse:
+        """
+        Description: 通过模板code更新模板的基本信息，比如模板名称等
+        Summary: 查询模板的基本信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryInnerTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.inner.template.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_template_elementlink(
+        self,
+        request: ato_models.QueryTemplateElementlinkRequest,
+    ) -> ato_models.QueryTemplateElementlinkResponse:
+        """
+        Description: 获取模板关联的元素列表信息，包括组件信息
+        Summary: 获取模板关联的元素列表信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_template_elementlink_ex(request, headers, runtime)
+
+    async def query_template_elementlink_async(
+        self,
+        request: ato_models.QueryTemplateElementlinkRequest,
+    ) -> ato_models.QueryTemplateElementlinkResponse:
+        """
+        Description: 获取模板关联的元素列表信息，包括组件信息
+        Summary: 获取模板关联的元素列表信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_template_elementlink_ex_async(request, headers, runtime)
+
+    def query_template_elementlink_ex(
+        self,
+        request: ato_models.QueryTemplateElementlinkRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryTemplateElementlinkResponse:
+        """
+        Description: 获取模板关联的元素列表信息，包括组件信息
+        Summary: 获取模板关联的元素列表信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryTemplateElementlinkResponse(),
+            self.do_request('1.0', 'antchain.ato.template.elementlink.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_template_elementlink_ex_async(
+        self,
+        request: ato_models.QueryTemplateElementlinkRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryTemplateElementlinkResponse:
+        """
+        Description: 获取模板关联的元素列表信息，包括组件信息
+        Summary: 获取模板关联的元素列表信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryTemplateElementlinkResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.template.elementlink.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def register_merchantexpand_merchant(
+        self,
+        request: ato_models.RegisterMerchantexpandMerchantRequest,
+    ) -> ato_models.RegisterMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻
+        Summary: 商户入驻
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.register_merchantexpand_merchant_ex(request, headers, runtime)
+
+    async def register_merchantexpand_merchant_async(
+        self,
+        request: ato_models.RegisterMerchantexpandMerchantRequest,
+    ) -> ato_models.RegisterMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻
+        Summary: 商户入驻
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.register_merchantexpand_merchant_ex_async(request, headers, runtime)
+
+    def register_merchantexpand_merchant_ex(
+        self,
+        request: ato_models.RegisterMerchantexpandMerchantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.RegisterMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻
+        Summary: 商户入驻
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.RegisterMerchantexpandMerchantResponse(),
+            self.do_request('1.0', 'antchain.ato.merchantexpand.merchant.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def register_merchantexpand_merchant_ex_async(
+        self,
+        request: ato_models.RegisterMerchantexpandMerchantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.RegisterMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻
+        Summary: 商户入驻
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.RegisterMerchantexpandMerchantResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.merchantexpand.merchant.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_merchantexpand_file(
+        self,
+        request: ato_models.UploadMerchantexpandFileRequest,
+    ) -> ato_models.UploadMerchantexpandFileResponse:
+        """
+        Description: 获取临时上传文件链接
+        Summary: 获取临时上传文件链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_merchantexpand_file_ex(request, headers, runtime)
+
+    async def upload_merchantexpand_file_async(
+        self,
+        request: ato_models.UploadMerchantexpandFileRequest,
+    ) -> ato_models.UploadMerchantexpandFileResponse:
+        """
+        Description: 获取临时上传文件链接
+        Summary: 获取临时上传文件链接
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_merchantexpand_file_ex_async(request, headers, runtime)
+
+    def upload_merchantexpand_file_ex(
+        self,
+        request: ato_models.UploadMerchantexpandFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadMerchantexpandFileResponse:
+        """
+        Description: 获取临时上传文件链接
+        Summary: 获取临时上传文件链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadMerchantexpandFileResponse(),
+            self.do_request('1.0', 'antchain.ato.merchantexpand.file.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_merchantexpand_file_ex_async(
+        self,
+        request: ato_models.UploadMerchantexpandFileRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadMerchantexpandFileResponse:
+        """
+        Description: 获取临时上传文件链接
+        Summary: 获取临时上传文件链接
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadMerchantexpandFileResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.merchantexpand.file.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_merchantexpand_merchant(
+        self,
+        request: ato_models.QueryMerchantexpandMerchantRequest,
+    ) -> ato_models.QueryMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻查询
+        Summary: 商户入驻查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_merchantexpand_merchant_ex(request, headers, runtime)
+
+    async def query_merchantexpand_merchant_async(
+        self,
+        request: ato_models.QueryMerchantexpandMerchantRequest,
+    ) -> ato_models.QueryMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻查询
+        Summary: 商户入驻查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_merchantexpand_merchant_ex_async(request, headers, runtime)
+
+    def query_merchantexpand_merchant_ex(
+        self,
+        request: ato_models.QueryMerchantexpandMerchantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻查询
+        Summary: 商户入驻查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryMerchantexpandMerchantResponse(),
+            self.do_request('1.0', 'antchain.ato.merchantexpand.merchant.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_merchantexpand_merchant_ex_async(
+        self,
+        request: ato_models.QueryMerchantexpandMerchantRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryMerchantexpandMerchantResponse:
+        """
+        Description: 商户入驻查询
+        Summary: 商户入驻查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryMerchantexpandMerchantResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.merchantexpand.merchant.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_realperson_facevrf(
         self,
         request: ato_models.CreateRealpersonFacevrfRequest,
     ) -> ato_models.CreateRealpersonFacevrfResponse:
         """
         Description: 可信身份认证，创建认证
         Summary: 创建认证
@@ -1593,14 +3665,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.QueryRealpersonFacevrfResponse(),
             await self.do_request_async('1.0', 'antchain.ato.realperson.facevrf.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_risk(
+        self,
+        request: ato_models.QueryRiskRequest,
+    ) -> ato_models.QueryRiskResponse:
+        """
+        Description: 发起风控分析，获取风险分
+        Summary: 发起风控分析，获取风险分
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_risk_ex(request, headers, runtime)
+
+    async def query_risk_async(
+        self,
+        request: ato_models.QueryRiskRequest,
+    ) -> ato_models.QueryRiskResponse:
+        """
+        Description: 发起风控分析，获取风险分
+        Summary: 发起风控分析，获取风险分
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_risk_ex_async(request, headers, runtime)
+
+    def query_risk_ex(
+        self,
+        request: ato_models.QueryRiskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryRiskResponse:
+        """
+        Description: 发起风控分析，获取风险分
+        Summary: 发起风控分析，获取风险分
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryRiskResponse(),
+            self.do_request('1.0', 'antchain.ato.risk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_risk_ex_async(
+        self,
+        request: ato_models.QueryRiskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.QueryRiskResponse:
+        """
+        Description: 发起风控分析，获取风险分
+        Summary: 发起风控分析，获取风险分
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.QueryRiskResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.risk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def all_sign_template(
         self,
         request: ato_models.AllSignTemplateRequest,
     ) -> ato_models.AllSignTemplateResponse:
         """
         Description: 电子合同签署的合同模板查询服务
         Summary: 电子合同签署的合同模板查询服务
@@ -1963,14 +4091,70 @@
             request.file_id = upload_resp.file_id
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.UploadSignFlowResponse(),
             await self.do_request_async('1.0', 'antchain.ato.sign.flow.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def upload_sign_template(
+        self,
+        request: ato_models.UploadSignTemplateRequest,
+    ) -> ato_models.UploadSignTemplateResponse:
+        """
+        Description: 商户合同模板上传接口
+        Summary: 商户合同模板上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_sign_template_ex(request, headers, runtime)
+
+    async def upload_sign_template_async(
+        self,
+        request: ato_models.UploadSignTemplateRequest,
+    ) -> ato_models.UploadSignTemplateResponse:
+        """
+        Description: 商户合同模板上传接口
+        Summary: 商户合同模板上传
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_sign_template_ex_async(request, headers, runtime)
+
+    def upload_sign_template_ex(
+        self,
+        request: ato_models.UploadSignTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadSignTemplateResponse:
+        """
+        Description: 商户合同模板上传接口
+        Summary: 商户合同模板上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadSignTemplateResponse(),
+            self.do_request('1.0', 'antchain.ato.sign.template.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_sign_template_ex_async(
+        self,
+        request: ato_models.UploadSignTemplateRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UploadSignTemplateResponse:
+        """
+        Description: 商户合同模板上传接口
+        Summary: 商户合同模板上传
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UploadSignTemplateResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.sign.template.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def sync_trade(
         self,
         request: ato_models.SyncTradeRequest,
     ) -> ato_models.SyncTradeResponse:
         """
         Description: 对账saas交易信息同步接口
         Summary: 对账saas交易信息同步接口
@@ -2355,46 +4539,214 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.GetTradeMerchantperformanceResponse(),
             await self.do_request_async('1.0', 'antchain.ato.trade.merchantperformance.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def update_trade_userpromise(
+        self,
+        request: ato_models.UpdateTradeUserpromiseRequest,
+    ) -> ato_models.UpdateTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.update_trade_userpromise_ex(request, headers, runtime)
+
+    async def update_trade_userpromise_async(
+        self,
+        request: ato_models.UpdateTradeUserpromiseRequest,
+    ) -> ato_models.UpdateTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.update_trade_userpromise_ex_async(request, headers, runtime)
+
+    def update_trade_userpromise_ex(
+        self,
+        request: ato_models.UpdateTradeUserpromiseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UpdateTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UpdateTradeUserpromiseResponse(),
+            self.do_request('1.0', 'antchain.ato.trade.userpromise.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def update_trade_userpromise_ex_async(
+        self,
+        request: ato_models.UpdateTradeUserpromiseRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.UpdateTradeUserpromiseResponse:
+        """
+        Description: 商户调用，修改订单的用户还款承诺
+        Summary: 用户还款承诺信息修改
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.UpdateTradeUserpromiseResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.trade.userpromise.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_front_indirectorder(
+        self,
+        request: ato_models.SyncFrontIndirectorderRequest,
+    ) -> ato_models.SyncFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_front_indirectorder_ex(request, headers, runtime)
+
+    async def sync_front_indirectorder_async(
+        self,
+        request: ato_models.SyncFrontIndirectorderRequest,
+    ) -> ato_models.SyncFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_front_indirectorder_ex_async(request, headers, runtime)
+
+    def sync_front_indirectorder_ex(
+        self,
+        request: ato_models.SyncFrontIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncFrontIndirectorderResponse(),
+            self.do_request('1.0', 'antchain.ato.front.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_front_indirectorder_ex_async(
+        self,
+        request: ato_models.SyncFrontIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncFrontIndirectorderResponse:
+        """
+        Description: 前置签署间联模式订单进件
+        Summary: 前置签署间联模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncFrontIndirectorderResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.front.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def sync_trade_indirectorder(
+        self,
+        request: ato_models.SyncTradeIndirectorderRequest,
+    ) -> ato_models.SyncTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_trade_indirectorder_ex(request, headers, runtime)
+
+    async def sync_trade_indirectorder_async(
+        self,
+        request: ato_models.SyncTradeIndirectorderRequest,
+    ) -> ato_models.SyncTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_trade_indirectorder_ex_async(request, headers, runtime)
+
+    def sync_trade_indirectorder_ex(
+        self,
+        request: ato_models.SyncTradeIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncTradeIndirectorderResponse(),
+            self.do_request('1.0', 'antchain.ato.trade.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_trade_indirectorder_ex_async(
+        self,
+        request: ato_models.SyncTradeIndirectorderRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ato_models.SyncTradeIndirectorderResponse:
+        """
+        Description: 间联模式-后置模式订单进件
+        Summary: 间联模式-后置模式订单进件
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ato_models.SyncTradeIndirectorderResponse(),
+            await self.do_request_async('1.0', 'antchain.ato.trade.indirectorder.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_withhold_sign(
         self,
         request: ato_models.CreateWithholdSignRequest,
     ) -> ato_models.CreateWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.create_withhold_sign_ex(request, headers, runtime)
 
     async def create_withhold_sign_async(
         self,
         request: ato_models.CreateWithholdSignRequest,
     ) -> ato_models.CreateWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.create_withhold_sign_ex_async(request, headers, runtime)
 
     def create_withhold_sign_ex(
         self,
         request: ato_models.CreateWithholdSignRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ato_models.CreateWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.CreateWithholdSignResponse(),
             self.do_request('1.0', 'antchain.ato.withhold.sign.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -2402,15 +4754,15 @@
     async def create_withhold_sign_ex_async(
         self,
         request: ato_models.CreateWithholdSignRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ato_models.CreateWithholdSignResponse:
         """
-        Description: 代扣签约
+        Description: 代扣签约创建
         Summary: 代扣签约
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ato_models.CreateWithholdSignResponse(),
             await self.do_request_async('1.0', 'antchain.ato.withhold.sign.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
@@ -2584,58 +4936,66 @@
         )
 
     def repay_withhold_plan(
         self,
         request: ato_models.RepayWithholdPlanRequest,
     ) -> ato_models.RepayWithholdPlanResponse:
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
         return self.repay_withhold_plan_ex(request, headers, runtime)
 
     async def repay_withhold_plan_async(
         self,
         request: ato_models.RepayWithholdPlanRequest,
     ) -> ato_models.RepayWithholdPlanResponse:
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
         return await self.repay_withhold_plan_ex_async(request, headers, runtime)
 
     def repay_withhold_plan_ex(
         self,
         request: ato_models.RepayWithholdPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ato_models.RepayWithholdPlanResponse:
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
             ato_models.RepayWithholdPlanResponse(),
             self.do_request('1.0', 'antchain.ato.withhold.plan.repay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def repay_withhold_plan_ex_async(
         self,
         request: ato_models.RepayWithholdPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> ato_models.RepayWithholdPlanResponse:
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
             ato_models.RepayWithholdPlanResponse(),
             await self.do_request_async('1.0', 'antchain.ato.withhold.plan.repay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
```

### Comparing `antchain_ato-1.7.26/antchain_sdk_ato/models.py` & `antchain_ato-1.8.51/antchain_sdk_ato/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,14 +150,50 @@
         if m.get('maxRequests') is not None:
             self.max_requests = m.get('maxRequests')
         if m.get('maxRequestsPerHost') is not None:
             self.max_requests_per_host = m.get('maxRequestsPerHost')
         return self
 
 
+class FileInfo(TeaModel):
+    def __init__(
+        self,
+        file_name: str = None,
+        file_key: str = None,
+    ):
+        # 文件名称
+        self.file_name = file_name
+        # 文件key
+        self.file_key = file_key
+
+    def validate(self):
+        self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.file_key, 'file_key')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
 class PromiseInfo(TeaModel):
     def __init__(self):
         pass
 
     def validate(self):
         pass
 
@@ -190,14 +226,410 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         return self
 
 
+class CompanyInfo(TeaModel):
+    def __init__(
+        self,
+        business_license_file: FileInfo = None,
+        product_main_class: str = None,
+        company_name: str = None,
+        company_alias_name: str = None,
+        tenant_id: str = None,
+        merchant_id: str = None,
+        company_mobile: str = None,
+        company_address: str = None,
+        contact_name: str = None,
+        contact_mobile: str = None,
+        bind_alipay_no: str = None,
+        settle_alipay_no: str = None,
+        bind_alipay_uid: str = None,
+    ):
+        # 营业执照文件信息
+        self.business_license_file = business_license_file
+        # 业务类型 枚举
+        self.product_main_class = product_main_class
+        # 公司名称
+        self.company_name = company_name
+        # 公司别名
+        self.company_alias_name = company_alias_name
+        # 公司数科租户id
+        self.tenant_id = tenant_id
+        # 统一社会信用代码
+        self.merchant_id = merchant_id
+        # 公司联系电话
+        self.company_mobile = company_mobile
+        # 公司联系地址
+        self.company_address = company_address
+        # 联系人姓名
+        self.contact_name = contact_name
+        # 联系人手机号码
+        self.contact_mobile = contact_mobile
+        # 绑定企业支付宝账号
+        self.bind_alipay_no = bind_alipay_no
+        # 结算企业支付宝账号
+        self.settle_alipay_no = settle_alipay_no
+        # 绑定支付宝uid
+        self.bind_alipay_uid = bind_alipay_uid
+
+    def validate(self):
+        self.validate_required(self.business_license_file, 'business_license_file')
+        if self.business_license_file:
+            self.business_license_file.validate()
+        self.validate_required(self.product_main_class, 'product_main_class')
+        self.validate_required(self.company_name, 'company_name')
+        self.validate_required(self.company_alias_name, 'company_alias_name')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.merchant_id, 'merchant_id')
+        self.validate_required(self.company_mobile, 'company_mobile')
+        self.validate_required(self.company_address, 'company_address')
+        self.validate_required(self.contact_name, 'contact_name')
+        self.validate_required(self.contact_mobile, 'contact_mobile')
+        self.validate_required(self.bind_alipay_no, 'bind_alipay_no')
+        self.validate_required(self.settle_alipay_no, 'settle_alipay_no')
+        self.validate_required(self.bind_alipay_uid, 'bind_alipay_uid')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.business_license_file is not None:
+            result['business_license_file'] = self.business_license_file.to_map()
+        if self.product_main_class is not None:
+            result['product_main_class'] = self.product_main_class
+        if self.company_name is not None:
+            result['company_name'] = self.company_name
+        if self.company_alias_name is not None:
+            result['company_alias_name'] = self.company_alias_name
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.company_mobile is not None:
+            result['company_mobile'] = self.company_mobile
+        if self.company_address is not None:
+            result['company_address'] = self.company_address
+        if self.contact_name is not None:
+            result['contact_name'] = self.contact_name
+        if self.contact_mobile is not None:
+            result['contact_mobile'] = self.contact_mobile
+        if self.bind_alipay_no is not None:
+            result['bind_alipay_no'] = self.bind_alipay_no
+        if self.settle_alipay_no is not None:
+            result['settle_alipay_no'] = self.settle_alipay_no
+        if self.bind_alipay_uid is not None:
+            result['bind_alipay_uid'] = self.bind_alipay_uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('business_license_file') is not None:
+            temp_model = FileInfo()
+            self.business_license_file = temp_model.from_map(m['business_license_file'])
+        if m.get('product_main_class') is not None:
+            self.product_main_class = m.get('product_main_class')
+        if m.get('company_name') is not None:
+            self.company_name = m.get('company_name')
+        if m.get('company_alias_name') is not None:
+            self.company_alias_name = m.get('company_alias_name')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('company_mobile') is not None:
+            self.company_mobile = m.get('company_mobile')
+        if m.get('company_address') is not None:
+            self.company_address = m.get('company_address')
+        if m.get('contact_name') is not None:
+            self.contact_name = m.get('contact_name')
+        if m.get('contact_mobile') is not None:
+            self.contact_mobile = m.get('contact_mobile')
+        if m.get('bind_alipay_no') is not None:
+            self.bind_alipay_no = m.get('bind_alipay_no')
+        if m.get('settle_alipay_no') is not None:
+            self.settle_alipay_no = m.get('settle_alipay_no')
+        if m.get('bind_alipay_uid') is not None:
+            self.bind_alipay_uid = m.get('bind_alipay_uid')
+        return self
+
+
+class AgreementPage(TeaModel):
+    def __init__(
+        self,
+        agreement_id: str = None,
+        merchant_name: str = None,
+        tenant_id: str = None,
+        product_main_class: str = None,
+        agreement_type: str = None,
+        sign_status: str = None,
+    ):
+        # 协议id
+        self.agreement_id = agreement_id
+        # 代理企业名称
+        self.merchant_name = merchant_name
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 业务类型 枚举
+        self.product_main_class = product_main_class
+        # 协议类型 枚举
+        self.agreement_type = agreement_type
+        # 租户签约状态 枚举
+        self.sign_status = sign_status
+
+    def validate(self):
+        self.validate_required(self.agreement_id, 'agreement_id')
+        self.validate_required(self.merchant_name, 'merchant_name')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.product_main_class, 'product_main_class')
+        self.validate_required(self.agreement_type, 'agreement_type')
+        self.validate_required(self.sign_status, 'sign_status')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.agreement_id is not None:
+            result['agreement_id'] = self.agreement_id
+        if self.merchant_name is not None:
+            result['merchant_name'] = self.merchant_name
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.product_main_class is not None:
+            result['product_main_class'] = self.product_main_class
+        if self.agreement_type is not None:
+            result['agreement_type'] = self.agreement_type
+        if self.sign_status is not None:
+            result['sign_status'] = self.sign_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('agreement_id') is not None:
+            self.agreement_id = m.get('agreement_id')
+        if m.get('merchant_name') is not None:
+            self.merchant_name = m.get('merchant_name')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('product_main_class') is not None:
+            self.product_main_class = m.get('product_main_class')
+        if m.get('agreement_type') is not None:
+            self.agreement_type = m.get('agreement_type')
+        if m.get('sign_status') is not None:
+            self.sign_status = m.get('sign_status')
+        return self
+
+
+class RiskScene(TeaModel):
+    def __init__(
+        self,
+        scene_code: str = None,
+        decision: str = None,
+    ):
+        # 风险场景编码
+        self.scene_code = scene_code
+        # 该场景的风险决策结果
+        self.decision = decision
+
+    def validate(self):
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.decision, 'decision')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.decision is not None:
+            result['decision'] = self.decision
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('decision') is not None:
+            self.decision = m.get('decision')
+        return self
+
+
+class RiskStrategy(TeaModel):
+    def __init__(
+        self,
+        id: str = None,
+        name: str = None,
+        decision: str = None,
+        scene_code: str = None,
+    ):
+        # 策略ID
+        self.id = id
+        # 策略名称
+        self.name = name
+        # 策略决策结果
+        self.decision = decision
+        # 风险场景编码
+        self.scene_code = scene_code
+
+    def validate(self):
+        self.validate_required(self.id, 'id')
+        self.validate_required(self.name, 'name')
+        self.validate_required(self.decision, 'decision')
+        self.validate_required(self.scene_code, 'scene_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.id is not None:
+            result['id'] = self.id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.decision is not None:
+            result['decision'] = self.decision
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('decision') is not None:
+            self.decision = m.get('decision')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        return self
+
+
+class RelationPage(TeaModel):
+    def __init__(
+        self,
+        relation_id: str = None,
+        company_name: str = None,
+        merchant_id: str = None,
+        status: str = None,
+    ):
+        # 分账关系id
+        self.relation_id = relation_id
+        # 分账公司名称
+        self.company_name = company_name
+        # 分账公司名称统一社会信用代码
+        self.merchant_id = merchant_id
+        # 审核状态
+        self.status = status
+
+    def validate(self):
+        self.validate_required(self.relation_id, 'relation_id')
+        self.validate_required(self.company_name, 'company_name')
+        self.validate_required(self.merchant_id, 'merchant_id')
+        self.validate_required(self.status, 'status')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.relation_id is not None:
+            result['relation_id'] = self.relation_id
+        if self.company_name is not None:
+            result['company_name'] = self.company_name
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('relation_id') is not None:
+            self.relation_id = m.get('relation_id')
+        if m.get('company_name') is not None:
+            self.company_name = m.get('company_name')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class MerchantAgentPage(TeaModel):
+    def __init__(
+        self,
+        pay_expand_id: str = None,
+        agent_name: str = None,
+        tenant_id: str = None,
+        biz_type: str = None,
+        pay_expand_status: str = None,
+    ):
+        # 进件id
+        self.pay_expand_id = pay_expand_id
+        # 
+        # 代理企业名称
+        self.agent_name = agent_name
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 业务类型
+        self.biz_type = biz_type
+        # 进件审核状态 枚举
+        self.pay_expand_status = pay_expand_status
+
+    def validate(self):
+        self.validate_required(self.pay_expand_id, 'pay_expand_id')
+        self.validate_required(self.agent_name, 'agent_name')
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.biz_type, 'biz_type')
+        self.validate_required(self.pay_expand_status, 'pay_expand_status')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
+        if self.agent_name is not None:
+            result['agent_name'] = self.agent_name
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.pay_expand_status is not None:
+            result['pay_expand_status'] = self.pay_expand_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        if m.get('agent_name') is not None:
+            self.agent_name = m.get('agent_name')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('pay_expand_status') is not None:
+            self.pay_expand_status = m.get('pay_expand_status')
+        return self
+
+
 class OrderInfo(TeaModel):
     def __init__(self):
         pass
 
     def validate(self):
         pass
 
@@ -307,14 +739,93 @@
         if m.get('receipt_amount') is not None:
             self.receipt_amount = m.get('receipt_amount')
         if m.get('gmt_pay') is not None:
             self.gmt_pay = m.get('gmt_pay')
         return self
 
 
+class ApplicationInfo(TeaModel):
+    def __init__(
+        self,
+        application_scene: str = None,
+        tiny_app_id: str = None,
+        site_name: str = None,
+        sit_url: str = None,
+        merchant_name: str = None,
+        merchant_service_name: str = None,
+        merchant_service_desc: str = None,
+    ):
+        # 应用场景
+        # MINI_APP 小程序
+        # APP 自有app
+        # ALL 两种都有
+        self.application_scene = application_scene
+        # 小程序id
+        self.tiny_app_id = tiny_app_id
+        # 小程序名称
+        self.site_name = site_name
+        # 网站地址
+        self.sit_url = sit_url
+        # 商户名称
+        self.merchant_name = merchant_name
+        # 商户服务名称
+        self.merchant_service_name = merchant_service_name
+        # 商户服务描述
+        self.merchant_service_desc = merchant_service_desc
+
+    def validate(self):
+        self.validate_required(self.application_scene, 'application_scene')
+        self.validate_required(self.tiny_app_id, 'tiny_app_id')
+        self.validate_required(self.site_name, 'site_name')
+        self.validate_required(self.sit_url, 'sit_url')
+        self.validate_required(self.merchant_name, 'merchant_name')
+        self.validate_required(self.merchant_service_name, 'merchant_service_name')
+        self.validate_required(self.merchant_service_desc, 'merchant_service_desc')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.application_scene is not None:
+            result['application_scene'] = self.application_scene
+        if self.tiny_app_id is not None:
+            result['tiny_app_id'] = self.tiny_app_id
+        if self.site_name is not None:
+            result['site_name'] = self.site_name
+        if self.sit_url is not None:
+            result['sit_url'] = self.sit_url
+        if self.merchant_name is not None:
+            result['merchant_name'] = self.merchant_name
+        if self.merchant_service_name is not None:
+            result['merchant_service_name'] = self.merchant_service_name
+        if self.merchant_service_desc is not None:
+            result['merchant_service_desc'] = self.merchant_service_desc
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('application_scene') is not None:
+            self.application_scene = m.get('application_scene')
+        if m.get('tiny_app_id') is not None:
+            self.tiny_app_id = m.get('tiny_app_id')
+        if m.get('site_name') is not None:
+            self.site_name = m.get('site_name')
+        if m.get('sit_url') is not None:
+            self.sit_url = m.get('sit_url')
+        if m.get('merchant_name') is not None:
+            self.merchant_name = m.get('merchant_name')
+        if m.get('merchant_service_name') is not None:
+            self.merchant_service_name = m.get('merchant_service_name')
+        if m.get('merchant_service_desc') is not None:
+            self.merchant_service_desc = m.get('merchant_service_desc')
+        return self
+
+
 class GoodsInfo(TeaModel):
     def __init__(self):
         pass
 
     def validate(self):
         pass
 
@@ -327,14 +838,204 @@
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         return self
 
 
+class PageQuery(TeaModel):
+    def __init__(
+        self,
+        page_size: int = None,
+        page_index: int = None,
+    ):
+        # 页大小
+        self.page_size = page_size
+        # 当前页
+        self.page_index = page_index
+
+    def validate(self):
+        self.validate_required(self.page_size, 'page_size')
+        self.validate_required(self.page_index, 'page_index')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.page_index is not None:
+            result['page_index'] = self.page_index
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('page_index') is not None:
+            self.page_index = m.get('page_index')
+        return self
+
+
+class LegalInfo(TeaModel):
+    def __init__(
+        self,
+        legal_name: str = None,
+        legal_cert_no: str = None,
+        legal_cert_front_file: FileInfo = None,
+        legal_cert_back_file: FileInfo = None,
+    ):
+        # 法人名称
+        self.legal_name = legal_name
+        # 法人证件号
+        self.legal_cert_no = legal_cert_no
+        # 法人证件正面
+        self.legal_cert_front_file = legal_cert_front_file
+        # 法人证件反面
+        self.legal_cert_back_file = legal_cert_back_file
+
+    def validate(self):
+        self.validate_required(self.legal_name, 'legal_name')
+        self.validate_required(self.legal_cert_no, 'legal_cert_no')
+        self.validate_required(self.legal_cert_front_file, 'legal_cert_front_file')
+        if self.legal_cert_front_file:
+            self.legal_cert_front_file.validate()
+        self.validate_required(self.legal_cert_back_file, 'legal_cert_back_file')
+        if self.legal_cert_back_file:
+            self.legal_cert_back_file.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.legal_name is not None:
+            result['legal_name'] = self.legal_name
+        if self.legal_cert_no is not None:
+            result['legal_cert_no'] = self.legal_cert_no
+        if self.legal_cert_front_file is not None:
+            result['legal_cert_front_file'] = self.legal_cert_front_file.to_map()
+        if self.legal_cert_back_file is not None:
+            result['legal_cert_back_file'] = self.legal_cert_back_file.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('legal_name') is not None:
+            self.legal_name = m.get('legal_name')
+        if m.get('legal_cert_no') is not None:
+            self.legal_cert_no = m.get('legal_cert_no')
+        if m.get('legal_cert_front_file') is not None:
+            temp_model = FileInfo()
+            self.legal_cert_front_file = temp_model.from_map(m['legal_cert_front_file'])
+        if m.get('legal_cert_back_file') is not None:
+            temp_model = FileInfo()
+            self.legal_cert_back_file = temp_model.from_map(m['legal_cert_back_file'])
+        return self
+
+
+class AuditInfo(TeaModel):
+    def __init__(
+        self,
+        stage: str = None,
+        audit_subject: str = None,
+        status: str = None,
+        apply_date_str: str = None,
+        fail_reason: str = None,
+    ):
+        # 审核步骤
+        self.stage = stage
+        # 审核主体
+        self.audit_subject = audit_subject
+        # 审核状态
+        self.status = status
+        # 审核时间
+        self.apply_date_str = apply_date_str
+        # 审核失败描述
+        self.fail_reason = fail_reason
+
+    def validate(self):
+        self.validate_required(self.stage, 'stage')
+        self.validate_required(self.audit_subject, 'audit_subject')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.apply_date_str, 'apply_date_str')
+        self.validate_required(self.fail_reason, 'fail_reason')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.stage is not None:
+            result['stage'] = self.stage
+        if self.audit_subject is not None:
+            result['audit_subject'] = self.audit_subject
+        if self.status is not None:
+            result['status'] = self.status
+        if self.apply_date_str is not None:
+            result['apply_date_str'] = self.apply_date_str
+        if self.fail_reason is not None:
+            result['fail_reason'] = self.fail_reason
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('stage') is not None:
+            self.stage = m.get('stage')
+        if m.get('audit_subject') is not None:
+            self.audit_subject = m.get('audit_subject')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('apply_date_str') is not None:
+            self.apply_date_str = m.get('apply_date_str')
+        if m.get('fail_reason') is not None:
+            self.fail_reason = m.get('fail_reason')
+        return self
+
+
+class RiskModel(TeaModel):
+    def __init__(
+        self,
+        scene_code: str = None,
+        score: str = None,
+    ):
+        # 风险场景编码
+        self.scene_code = scene_code
+        # 该风险场景的风险分值
+        self.score = score
+
+    def validate(self):
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.score, 'score')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.score is not None:
+            result['score'] = self.score
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('score') is not None:
+            self.score = m.get('score')
+        return self
+
+
 class OrderGoodsModel(TeaModel):
     def __init__(self):
         pass
 
     def validate(self):
         pass
 
@@ -2452,14 +3153,121 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('response_data') is not None:
             self.response_data = m.get('response_data')
         return self
 
 
+class NotifyFundFlowRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_id: str = None,
+        order_id: str = None,
+        sign_no: str = None,
+        file_item_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单所属商户的统一社会信用代码
+        self.merchant_id = merchant_id
+        # 商户的订单号
+        self.order_id = order_id
+        # 签署合同单号
+        self.sign_no = sign_no
+        # 返回的文件fileItemNo编号
+        self.file_item_no = file_item_no
+
+    def validate(self):
+        self.validate_required(self.merchant_id, 'merchant_id')
+        self.validate_required(self.order_id, 'order_id')
+        self.validate_required(self.sign_no, 'sign_no')
+        self.validate_required(self.file_item_no, 'file_item_no')
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
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.order_id is not None:
+            result['order_id'] = self.order_id
+        if self.sign_no is not None:
+            result['sign_no'] = self.sign_no
+        if self.file_item_no is not None:
+            result['file_item_no'] = self.file_item_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('order_id') is not None:
+            self.order_id = m.get('order_id')
+        if m.get('sign_no') is not None:
+            self.sign_no = m.get('sign_no')
+        if m.get('file_item_no') is not None:
+            self.file_item_no = m.get('file_item_no')
+        return self
+
+
+class NotifyFundFlowResponse(TeaModel):
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
 class GetInnerProductRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         merchant_tenant_id: str = None,
         merchant_id: str = None,
@@ -2675,69 +3483,63 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         merchant_tenant_id: str = None,
         merchant_id: str = None,
         meter_product_code: str = None,
         order_id: str = None,
-        order_product_id: str = None,
-        order_product_version: str = None,
         order_rent_term: int = None,
         order_total_money: int = None,
         sys_name: str = None,
+        order_product_subclass: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 商户租户id
         self.merchant_tenant_id = merchant_tenant_id
         # 商户统一社会信用代码
         self.merchant_id = merchant_id
         # 商户购买的产品code
         self.meter_product_code = meter_product_code
         # 订单id
         self.order_id = order_id
-        # 订单关联的商品id
-        self.order_product_id = order_product_id
-        # 商品的版本
-        self.order_product_version = order_product_version
         # 订单总租期
         self.order_rent_term = order_rent_term
         # 订单总租金，单位为分
         self.order_total_money = order_total_money
         # 系统名称
         self.sys_name = sys_name
+        # 订单产品的二级类目
+        self.order_product_subclass = order_product_subclass
 
     def validate(self):
         self.validate_required(self.merchant_tenant_id, 'merchant_tenant_id')
         if self.merchant_tenant_id is not None:
             self.validate_max_length(self.merchant_tenant_id, 'merchant_tenant_id', 32)
         self.validate_required(self.merchant_id, 'merchant_id')
         if self.merchant_id is not None:
             self.validate_max_length(self.merchant_id, 'merchant_id', 199)
         self.validate_required(self.meter_product_code, 'meter_product_code')
         if self.meter_product_code is not None:
             self.validate_max_length(self.meter_product_code, 'meter_product_code', 64)
         self.validate_required(self.order_id, 'order_id')
         if self.order_id is not None:
             self.validate_max_length(self.order_id, 'order_id', 49)
-        self.validate_required(self.order_product_id, 'order_product_id')
-        if self.order_product_id is not None:
-            self.validate_max_length(self.order_product_id, 'order_product_id', 32)
-        self.validate_required(self.order_product_version, 'order_product_version')
-        if self.order_product_version is not None:
-            self.validate_max_length(self.order_product_version, 'order_product_version', 10)
         self.validate_required(self.order_rent_term, 'order_rent_term')
         if self.order_rent_term is not None:
             self.validate_maximum(self.order_rent_term, 'order_rent_term', 200)
             self.validate_minimum(self.order_rent_term, 'order_rent_term', 1)
         self.validate_required(self.order_total_money, 'order_total_money')
         self.validate_required(self.sys_name, 'sys_name')
         if self.sys_name is not None:
             self.validate_max_length(self.sys_name, 'sys_name', 32)
+        self.validate_required(self.order_product_subclass, 'order_product_subclass')
+        if self.order_product_subclass is not None:
+            self.validate_max_length(self.order_product_subclass, 'order_product_subclass', 64)
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -2749,24 +3551,22 @@
             result['merchant_tenant_id'] = self.merchant_tenant_id
         if self.merchant_id is not None:
             result['merchant_id'] = self.merchant_id
         if self.meter_product_code is not None:
             result['meter_product_code'] = self.meter_product_code
         if self.order_id is not None:
             result['order_id'] = self.order_id
-        if self.order_product_id is not None:
-            result['order_product_id'] = self.order_product_id
-        if self.order_product_version is not None:
-            result['order_product_version'] = self.order_product_version
         if self.order_rent_term is not None:
             result['order_rent_term'] = self.order_rent_term
         if self.order_total_money is not None:
             result['order_total_money'] = self.order_total_money
         if self.sys_name is not None:
             result['sys_name'] = self.sys_name
+        if self.order_product_subclass is not None:
+            result['order_product_subclass'] = self.order_product_subclass
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -2775,24 +3575,22 @@
             self.merchant_tenant_id = m.get('merchant_tenant_id')
         if m.get('merchant_id') is not None:
             self.merchant_id = m.get('merchant_id')
         if m.get('meter_product_code') is not None:
             self.meter_product_code = m.get('meter_product_code')
         if m.get('order_id') is not None:
             self.order_id = m.get('order_id')
-        if m.get('order_product_id') is not None:
-            self.order_product_id = m.get('order_product_id')
-        if m.get('order_product_version') is not None:
-            self.order_product_version = m.get('order_product_version')
         if m.get('order_rent_term') is not None:
             self.order_rent_term = m.get('order_rent_term')
         if m.get('order_total_money') is not None:
             self.order_total_money = m.get('order_total_money')
         if m.get('sys_name') is not None:
             self.sys_name = m.get('sys_name')
+        if m.get('order_product_subclass') is not None:
+            self.order_product_subclass = m.get('order_product_subclass')
         return self
 
 
 class SyncInnerMeterforwholeorderResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -2965,14 +3763,4185 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class AllInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        page_info: PageQuery = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 分页查询结构体
+        self.page_info = page_info
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板文件名称
+        self.template_name = template_name
+
+    def validate(self):
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
+        self.validate_required(self.tenant_id, 'tenant_id')
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
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_name is not None:
+            result['template_name'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_name') is not None:
+            self.template_name = m.get('template_name')
+        return self
+
+
+class AllInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        template_list: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板列表数据
+        self.template_list = template_list
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
+        if self.template_list is not None:
+            result['template_list'] = self.template_list
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
+        if m.get('template_list') is not None:
+            self.template_list = m.get('template_list')
+        return self
+
+
+class ListInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        page_info: PageQuery = None,
+        tenant_id: str = None,
+        template_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 分页查询
+        self.page_info = page_info
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+
+    def validate(self):
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
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
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        return self
+
+
+class ListInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        template_list: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板列表数据
+        self.template_list = template_list
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
+        if self.template_list is not None:
+            result['template_list'] = self.template_list
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
+        if m.get('template_list') is not None:
+            self.template_list = m.get('template_list')
+        return self
+
+
+class DetailInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        return self
+
+
+class DetailInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        template_info: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板详情信息
+        self.template_info = template_info
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
+        if self.template_info is not None:
+            result['template_info'] = self.template_info
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
+        if m.get('template_info') is not None:
+            self.template_info = m.get('template_info')
+        return self
+
+
+class CreateInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_name: str = None,
+        file_key: str = None,
+        file_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 创建的模板名称
+        self.template_name = template_name
+        # 文件oss存储的key
+        self.file_key = file_key
+        # 模板文件的名称
+        self.file_name = file_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_name, 'template_name')
+        if self.template_name is not None:
+            self.validate_max_length(self.template_name, 'template_name', 32)
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_name is not None:
+            result['template_name'] = self.template_name
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_name') is not None:
+            self.template_name = m.get('template_name')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        return self
+
+
+class CreateInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        template_code: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 魔法库模板code
+        self.template_code = template_code
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
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
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
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        return self
+
+
+class SaveInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+        preview_address: str = None,
+        template_element_list: str = None,
+        file_key: str = None,
+        confirm: bool = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+        # 文件预览地址
+        self.preview_address = preview_address
+        # 创建模板的元素列表
+        self.template_element_list = template_element_list
+        # 文件oss存储的key
+        self.file_key = file_key
+        # 是否确认保存。点击”保存“按钮传false、点击”下一步“按钮传true
+        self.confirm = confirm
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
+        self.validate_required(self.preview_address, 'preview_address')
+        self.validate_required(self.file_key, 'file_key')
+        self.validate_required(self.confirm, 'confirm')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        if self.preview_address is not None:
+            result['preview_address'] = self.preview_address
+        if self.template_element_list is not None:
+            result['template_element_list'] = self.template_element_list
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        if self.confirm is not None:
+            result['confirm'] = self.confirm
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        if m.get('preview_address') is not None:
+            self.preview_address = m.get('preview_address')
+        if m.get('template_element_list') is not None:
+            self.template_element_list = m.get('template_element_list')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        if m.get('confirm') is not None:
+            self.confirm = m.get('confirm')
+        return self
+
+
+class SaveInnerTemplateResponse(TeaModel):
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
+class SaveInnerSignfieldsRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+        sign_field_list: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+        # 模板签署区列表
+        self.sign_field_list = sign_field_list
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
+        self.validate_required(self.sign_field_list, 'sign_field_list')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        if self.sign_field_list is not None:
+            result['sign_field_list'] = self.sign_field_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        if m.get('sign_field_list') is not None:
+            self.sign_field_list = m.get('sign_field_list')
+        return self
+
+
+class SaveInnerSignfieldsResponse(TeaModel):
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
+class PublishInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库版本id
+        self.template_version_id = template_version_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version_id, 'template_version_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version_id is not None:
+            result['template_version_id'] = self.template_version_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version_id') is not None:
+            self.template_version_id = m.get('template_version_id')
+        return self
+
+
+class PublishInnerTemplateResponse(TeaModel):
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
+class PreviewInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        file_key: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 文件oss存储的key
+        self.file_key = file_key
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.file_key, 'file_key')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class PreviewInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 预览接口返回
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class DeleteInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+        template_version_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+        # 魔法库模板版本id
+        self.template_version_id = template_version_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
+        self.validate_required(self.template_version_id, 'template_version_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        if self.template_version_id is not None:
+            result['template_version_id'] = self.template_version_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        if m.get('template_version_id') is not None:
+            self.template_version_id = m.get('template_version_id')
+        return self
+
+
+class DeleteInnerTemplateResponse(TeaModel):
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
+class CloneInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        voucher_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库对应模板的模板复制id
+        self.voucher_id = voucher_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.voucher_id, 'voucher_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.voucher_id is not None:
+            result['voucher_id'] = self.voucher_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('voucher_id') is not None:
+            self.voucher_id = m.get('voucher_id')
+        return self
+
+
+class CloneInnerTemplateResponse(TeaModel):
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
+class UploadInnerFileRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        file_name: str = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 文件名称
+        self.file_name = file_name
+        # ● BUSINESS_LICENSE 营业执照
+        # ● CARD_FRONT 身份证正面
+        # ● CARD_BACK 身份证反面
+        # ● SPLITTING 分账
+        # ● CONTRACT_TEMPLATE 合同模板
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.biz_scene, 'biz_scene')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class UploadInnerFileResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        upload_url: str = None,
+        file_key: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 临时上传地址
+        self.upload_url = upload_url
+        # 文件key
+        self.file_key = file_key
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
+        if self.upload_url is not None:
+            result['upload_url'] = self.upload_url
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
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
+        if m.get('upload_url') is not None:
+            self.upload_url = m.get('upload_url')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class DownloadInnerFileRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        file_key: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 文件key
+        self.file_key = file_key
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.file_key, 'file_key')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class DownloadInnerFileResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        download_url: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 文件临时下载地址
+        self.download_url = download_url
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
+        if self.download_url is not None:
+            result['download_url'] = self.download_url
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
+        if m.get('download_url') is not None:
+            self.download_url = m.get('download_url')
+        return self
+
+
+class GetInnerTemplateofficeurlRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        return self
+
+
+class GetInnerTemplateofficeurlResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 返回值
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class RefreshInnerTemplatetokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        access_token: str = None,
+        refresh_token: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # accessToken
+        self.access_token = access_token
+        # refreshToekn
+        self.refresh_token = refresh_token
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.access_token, 'access_token')
+        self.validate_required(self.refresh_token, 'refresh_token')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        if self.refresh_token is not None:
+            result['refresh_token'] = self.refresh_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        if m.get('refresh_token') is not None:
+            self.refresh_token = m.get('refresh_token')
+        return self
+
+
+class RefreshInnerTemplatetokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 返回值
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class CreateInnerTemplatetextareaRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+        component_type: str = None,
+        component_name: str = None,
+        required: bool = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 模板编码
+        self.template_code = template_code
+        # 模板版本号
+        self.template_version = template_version
+        # 组件类型，INPUT:单行文本 TEXTAREA:多行文本
+        self.component_type = component_type
+        # 组件名称（占位符）
+        self.component_name = component_name
+        # 是否必填
+        self.required = required
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
+        self.validate_required(self.component_type, 'component_type')
+        self.validate_required(self.component_name, 'component_name')
+        self.validate_required(self.required, 'required')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        if self.component_type is not None:
+            result['component_type'] = self.component_type
+        if self.component_name is not None:
+            result['component_name'] = self.component_name
+        if self.required is not None:
+            result['required'] = self.required
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        if m.get('component_type') is not None:
+            self.component_type = m.get('component_type')
+        if m.get('component_name') is not None:
+            self.component_name = m.get('component_name')
+        if m.get('required') is not None:
+            self.required = m.get('required')
+        return self
+
+
+class CreateInnerTemplatetextareaResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 创建成功的文本域组件信息
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class QueryInnerTemplateimageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        page_info: PageQuery = None,
+        template_code: str = None,
+        template_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 分页查询结构体
+        self.page_info = page_info
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        return self
+
+
+class QueryInnerTemplateimageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板图片列表
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class CreateInnerFunddividerelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        relation_id: str = None,
+        company_name: str = None,
+        merchant_id: str = None,
+        contract_files: List[FileInfo] = None,
+        desc: str = None,
+        alipay_pid: str = None,
+        alipay_account: str = None,
+        submit: str = None,
+        user_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 第一次暂存或提交可以不传，由后端生成
+        self.relation_id = relation_id
+        # 分账公司名称
+        self.company_name = company_name
+        # 分账公司社会信用代码
+        self.merchant_id = merchant_id
+        # 分账合同或协议
+        self.contract_files = contract_files
+        # 分账关系说明
+        self.desc = desc
+        # 分账方企业pid
+        self.alipay_pid = alipay_pid
+        # 分账方企业支付宝账号
+        self.alipay_account = alipay_account
+        # 是否直接提交
+        # SUBMITTED 直接提交
+        # STAGE 暂存
+        self.submit = submit
+        # 操作人名称
+        self.user_name = user_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        if self.contract_files:
+            for k in self.contract_files:
+                if k:
+                    k.validate()
+        self.validate_required(self.submit, 'submit')
+        self.validate_required(self.user_name, 'user_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.relation_id is not None:
+            result['relation_id'] = self.relation_id
+        if self.company_name is not None:
+            result['company_name'] = self.company_name
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        result['contract_files'] = []
+        if self.contract_files is not None:
+            for k in self.contract_files:
+                result['contract_files'].append(k.to_map() if k else None)
+        if self.desc is not None:
+            result['desc'] = self.desc
+        if self.alipay_pid is not None:
+            result['alipay_pid'] = self.alipay_pid
+        if self.alipay_account is not None:
+            result['alipay_account'] = self.alipay_account
+        if self.submit is not None:
+            result['submit'] = self.submit
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('relation_id') is not None:
+            self.relation_id = m.get('relation_id')
+        if m.get('company_name') is not None:
+            self.company_name = m.get('company_name')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        self.contract_files = []
+        if m.get('contract_files') is not None:
+            for k in m.get('contract_files'):
+                temp_model = FileInfo()
+                self.contract_files.append(temp_model.from_map(k))
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
+        if m.get('alipay_pid') is not None:
+            self.alipay_pid = m.get('alipay_pid')
+        if m.get('alipay_account') is not None:
+            self.alipay_account = m.get('alipay_account')
+        if m.get('submit') is not None:
+            self.submit = m.get('submit')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        return self
+
+
+class CreateInnerFunddividerelationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        relation_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 分账关系id
+        self.relation_id = relation_id
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
+        if self.relation_id is not None:
+            result['relation_id'] = self.relation_id
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
+        if m.get('relation_id') is not None:
+            self.relation_id = m.get('relation_id')
+        return self
+
+
+class SubmitInnerFunddividerelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        relation_id: str = None,
+        user_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 分账关系id
+        self.relation_id = relation_id
+        # 操作人名称
+        self.user_name = user_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.relation_id, 'relation_id')
+        self.validate_required(self.user_name, 'user_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.relation_id is not None:
+            result['relation_id'] = self.relation_id
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('relation_id') is not None:
+            self.relation_id = m.get('relation_id')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        return self
+
+
+class SubmitInnerFunddividerelationResponse(TeaModel):
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
+class QueryInnerFunddividerelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        relation_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 分账关系id
+        self.relation_id = relation_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.relation_id, 'relation_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.relation_id is not None:
+            result['relation_id'] = self.relation_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('relation_id') is not None:
+            self.relation_id = m.get('relation_id')
+        return self
+
+
+class QueryInnerFunddividerelationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        company_name: str = None,
+        merchant_id: str = None,
+        contract_files: List[FileInfo] = None,
+        desc: str = None,
+        alipay_pid: str = None,
+        alipay_account: str = None,
+        audit_infos: List[AuditInfo] = None,
+        relation_status: str = None,
+        relation_fail_reason: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 分账公司名称
+        self.company_name = company_name
+        # 统一社会信用代码
+        self.merchant_id = merchant_id
+        # 分账合同或协议
+        self.contract_files = contract_files
+        # 分账关系说明
+        self.desc = desc
+        # 分账方企业pid
+        self.alipay_pid = alipay_pid
+        # 分账方企业支付宝账号
+        self.alipay_account = alipay_account
+        # 审核列表
+        self.audit_infos = audit_infos
+        # INIT:待提交 AUDIT:审批中 AUDIT_PASSED:审批通过 AUDIT_NOT_PASSED:审批不通过
+        self.relation_status = relation_status
+        # 分账关系绑定失败原因
+        self.relation_fail_reason = relation_fail_reason
+
+    def validate(self):
+        if self.contract_files:
+            for k in self.contract_files:
+                if k:
+                    k.validate()
+        if self.audit_infos:
+            for k in self.audit_infos:
+                if k:
+                    k.validate()
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
+        if self.company_name is not None:
+            result['company_name'] = self.company_name
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        result['contract_files'] = []
+        if self.contract_files is not None:
+            for k in self.contract_files:
+                result['contract_files'].append(k.to_map() if k else None)
+        if self.desc is not None:
+            result['desc'] = self.desc
+        if self.alipay_pid is not None:
+            result['alipay_pid'] = self.alipay_pid
+        if self.alipay_account is not None:
+            result['alipay_account'] = self.alipay_account
+        result['audit_infos'] = []
+        if self.audit_infos is not None:
+            for k in self.audit_infos:
+                result['audit_infos'].append(k.to_map() if k else None)
+        if self.relation_status is not None:
+            result['relation_status'] = self.relation_status
+        if self.relation_fail_reason is not None:
+            result['relation_fail_reason'] = self.relation_fail_reason
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
+        if m.get('company_name') is not None:
+            self.company_name = m.get('company_name')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        self.contract_files = []
+        if m.get('contract_files') is not None:
+            for k in m.get('contract_files'):
+                temp_model = FileInfo()
+                self.contract_files.append(temp_model.from_map(k))
+        if m.get('desc') is not None:
+            self.desc = m.get('desc')
+        if m.get('alipay_pid') is not None:
+            self.alipay_pid = m.get('alipay_pid')
+        if m.get('alipay_account') is not None:
+            self.alipay_account = m.get('alipay_account')
+        self.audit_infos = []
+        if m.get('audit_infos') is not None:
+            for k in m.get('audit_infos'):
+                temp_model = AuditInfo()
+                self.audit_infos.append(temp_model.from_map(k))
+        if m.get('relation_status') is not None:
+            self.relation_status = m.get('relation_status')
+        if m.get('relation_fail_reason') is not None:
+            self.relation_fail_reason = m.get('relation_fail_reason')
+        return self
+
+
+class PagequeryInnerFunddividerelationRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        page_info: PageQuery = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 分页查询对象
+        self.page_info = page_info
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        return self
+
+
+class PagequeryInnerFunddividerelationResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total_size: int = None,
+        relations: List[RelationPage] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 数据总量
+        self.total_size = total_size
+        # 分账关系页对象列表
+        self.relations = relations
+
+    def validate(self):
+        if self.relations:
+            for k in self.relations:
+                if k:
+                    k.validate()
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
+        if self.total_size is not None:
+            result['total_size'] = self.total_size
+        result['relations'] = []
+        if self.relations is not None:
+            for k in self.relations:
+                result['relations'].append(k.to_map() if k else None)
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
+        if m.get('total_size') is not None:
+            self.total_size = m.get('total_size')
+        self.relations = []
+        if m.get('relations') is not None:
+            for k in m.get('relations'):
+                temp_model = RelationPage()
+                self.relations.append(temp_model.from_map(k))
+        return self
+
+
+class CreateInnerMerchantagreementRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        agreement_id: str = None,
+        sign_action: str = None,
+        user_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 协议编号
+        self.agreement_id = agreement_id
+        # 签署动作
+        self.sign_action = sign_action
+        # 操作人名称
+        self.user_name = user_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.agreement_id, 'agreement_id')
+        self.validate_required(self.sign_action, 'sign_action')
+        self.validate_required(self.user_name, 'user_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.agreement_id is not None:
+            result['agreement_id'] = self.agreement_id
+        if self.sign_action is not None:
+            result['sign_action'] = self.sign_action
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('agreement_id') is not None:
+            self.agreement_id = m.get('agreement_id')
+        if m.get('sign_action') is not None:
+            self.sign_action = m.get('sign_action')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        return self
+
+
+class CreateInnerMerchantagreementResponse(TeaModel):
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
+class QueryInnerMerchantagreementRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        agreement_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 协议id
+        self.agreement_id = agreement_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.agreement_id, 'agreement_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.agreement_id is not None:
+            result['agreement_id'] = self.agreement_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('agreement_id') is not None:
+            self.agreement_id = m.get('agreement_id')
+        return self
+
+
+class QueryInnerMerchantagreementResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        sign_status: str = None,
+        sign_date_str: str = None,
+        agreement_content: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 签约状态 枚举
+        # TOBE 待签
+        # FAIL 签约失败
+        # SUCCESS 签约成功
+        self.sign_status = sign_status
+        # 签约时间
+        self.sign_date_str = sign_date_str
+        # 协议内容 富文本
+        self.agreement_content = agreement_content
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
+        if self.sign_status is not None:
+            result['sign_status'] = self.sign_status
+        if self.sign_date_str is not None:
+            result['sign_date_str'] = self.sign_date_str
+        if self.agreement_content is not None:
+            result['agreement_content'] = self.agreement_content
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
+        if m.get('sign_status') is not None:
+            self.sign_status = m.get('sign_status')
+        if m.get('sign_date_str') is not None:
+            self.sign_date_str = m.get('sign_date_str')
+        if m.get('agreement_content') is not None:
+            self.agreement_content = m.get('agreement_content')
+        return self
+
+
+class PagequeryInnerMerchantagreementRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        page_info: PageQuery = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 分页对象
+        self.page_info = page_info
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        return self
+
+
+class PagequeryInnerMerchantagreementResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total_size: int = None,
+        agreement_page: List[AgreementPage] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 数据总量
+        self.total_size = total_size
+        # 协议分页对象
+        self.agreement_page = agreement_page
+
+    def validate(self):
+        if self.agreement_page:
+            for k in self.agreement_page:
+                if k:
+                    k.validate()
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
+        if self.total_size is not None:
+            result['total_size'] = self.total_size
+        result['agreement_page'] = []
+        if self.agreement_page is not None:
+            for k in self.agreement_page:
+                result['agreement_page'].append(k.to_map() if k else None)
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
+        if m.get('total_size') is not None:
+            self.total_size = m.get('total_size')
+        self.agreement_page = []
+        if m.get('agreement_page') is not None:
+            for k in m.get('agreement_page'):
+                temp_model = AgreementPage()
+                self.agreement_page.append(temp_model.from_map(k))
+        return self
+
+
+class CreateInnerMerchantpayexpandRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        company_info: CompanyInfo = None,
+        legal_info: LegalInfo = None,
+        application_info: ApplicationInfo = None,
+        submit: str = None,
+        expand_mode: str = None,
+        sub_tenant_id: str = None,
+        user_name: str = None,
+        pay_expand_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 公司信息
+        self.company_info = company_info
+        # 法人信息
+        self.legal_info = legal_info
+        # 应用信息
+        self.application_info = application_info
+        # 是否直接提交
+        # SUBMITTED 直接提交
+        # STAGE 暂存
+        self.submit = submit
+        # 进件模式
+        # DIRECT(直连进件)
+        # AGENT(代理进件)
+        self.expand_mode = expand_mode
+        # expand_mode=_AGENT_ 必填
+        self.sub_tenant_id = sub_tenant_id
+        # 操作人名称
+        self.user_name = user_name
+        # 第一次暂存或保存可以不传，后端直接生成
+        self.pay_expand_id = pay_expand_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        if self.company_info:
+            self.company_info.validate()
+        if self.legal_info:
+            self.legal_info.validate()
+        if self.application_info:
+            self.application_info.validate()
+        self.validate_required(self.submit, 'submit')
+        self.validate_required(self.expand_mode, 'expand_mode')
+        self.validate_required(self.user_name, 'user_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.company_info is not None:
+            result['company_info'] = self.company_info.to_map()
+        if self.legal_info is not None:
+            result['legal_info'] = self.legal_info.to_map()
+        if self.application_info is not None:
+            result['application_info'] = self.application_info.to_map()
+        if self.submit is not None:
+            result['submit'] = self.submit
+        if self.expand_mode is not None:
+            result['expand_mode'] = self.expand_mode
+        if self.sub_tenant_id is not None:
+            result['sub_tenant_id'] = self.sub_tenant_id
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('company_info') is not None:
+            temp_model = CompanyInfo()
+            self.company_info = temp_model.from_map(m['company_info'])
+        if m.get('legal_info') is not None:
+            temp_model = LegalInfo()
+            self.legal_info = temp_model.from_map(m['legal_info'])
+        if m.get('application_info') is not None:
+            temp_model = ApplicationInfo()
+            self.application_info = temp_model.from_map(m['application_info'])
+        if m.get('submit') is not None:
+            self.submit = m.get('submit')
+        if m.get('expand_mode') is not None:
+            self.expand_mode = m.get('expand_mode')
+        if m.get('sub_tenant_id') is not None:
+            self.sub_tenant_id = m.get('sub_tenant_id')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        return self
+
+
+class CreateInnerMerchantpayexpandResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        pay_expand_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 进件流水号
+        self.pay_expand_id = pay_expand_id
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
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
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
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        return self
+
+
+class SubmitInnerMerchantpayexpandRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        pay_expand_id: str = None,
+        user_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 进件id
+        self.pay_expand_id = pay_expand_id
+        # 操作人名称
+        self.user_name = user_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.pay_expand_id, 'pay_expand_id')
+        self.validate_required(self.user_name, 'user_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        return self
+
+
+class SubmitInnerMerchantpayexpandResponse(TeaModel):
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
+class QueryInnerMerchantpayexpandRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        pay_expand_id: str = None,
+        expand_mode: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 进件id expand_mode=AGENT 必填 DIRECT可以根据tenant_id推断
+        self.pay_expand_id = pay_expand_id
+        # 进件模式 DIRECT(直连进件) AGENT(代理进件)
+        self.expand_mode = expand_mode
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.expand_mode, 'expand_mode')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
+        if self.expand_mode is not None:
+            result['expand_mode'] = self.expand_mode
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        if m.get('expand_mode') is not None:
+            self.expand_mode = m.get('expand_mode')
+        return self
+
+
+class QueryInnerMerchantpayexpandResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        company_info: CompanyInfo = None,
+        legal_info: LegalInfo = None,
+        application_info: ApplicationInfo = None,
+        audit_infos: List[AuditInfo] = None,
+        expand_mode: str = None,
+        expand_status: str = None,
+        expand_fail_reason: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 公司信息
+        self.company_info = company_info
+        # 法人信息
+        self.legal_info = legal_info
+        # 应用信息
+        self.application_info = application_info
+        # 审核列表
+        self.audit_infos = audit_infos
+        # 进件模式 DIRECT(直连进件) AGENT(代理进件)
+        self.expand_mode = expand_mode
+        # INIT:草稿态 SUB_MERCHANT_CREDIT:二级户商户签约中 AUDIT:审核中 AUDIT_PASSED:进件成功 AUDIT_NOT_PASSED:进件失败 MERCHANT_CONFIRM:待商户确认
+        self.expand_status = expand_status
+        # 进件失败描述
+        self.expand_fail_reason = expand_fail_reason
+
+    def validate(self):
+        if self.company_info:
+            self.company_info.validate()
+        if self.legal_info:
+            self.legal_info.validate()
+        if self.application_info:
+            self.application_info.validate()
+        if self.audit_infos:
+            for k in self.audit_infos:
+                if k:
+                    k.validate()
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
+        if self.company_info is not None:
+            result['company_info'] = self.company_info.to_map()
+        if self.legal_info is not None:
+            result['legal_info'] = self.legal_info.to_map()
+        if self.application_info is not None:
+            result['application_info'] = self.application_info.to_map()
+        result['audit_infos'] = []
+        if self.audit_infos is not None:
+            for k in self.audit_infos:
+                result['audit_infos'].append(k.to_map() if k else None)
+        if self.expand_mode is not None:
+            result['expand_mode'] = self.expand_mode
+        if self.expand_status is not None:
+            result['expand_status'] = self.expand_status
+        if self.expand_fail_reason is not None:
+            result['expand_fail_reason'] = self.expand_fail_reason
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
+        if m.get('company_info') is not None:
+            temp_model = CompanyInfo()
+            self.company_info = temp_model.from_map(m['company_info'])
+        if m.get('legal_info') is not None:
+            temp_model = LegalInfo()
+            self.legal_info = temp_model.from_map(m['legal_info'])
+        if m.get('application_info') is not None:
+            temp_model = ApplicationInfo()
+            self.application_info = temp_model.from_map(m['application_info'])
+        self.audit_infos = []
+        if m.get('audit_infos') is not None:
+            for k in m.get('audit_infos'):
+                temp_model = AuditInfo()
+                self.audit_infos.append(temp_model.from_map(k))
+        if m.get('expand_mode') is not None:
+            self.expand_mode = m.get('expand_mode')
+        if m.get('expand_status') is not None:
+            self.expand_status = m.get('expand_status')
+        if m.get('expand_fail_reason') is not None:
+            self.expand_fail_reason = m.get('expand_fail_reason')
+        return self
+
+
+class PagequeryInnerMerchantagentRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        agent_name: str = None,
+        page_info: PageQuery = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户8位id
+        self.tenant_id = tenant_id
+        # 代理商户名称
+        self.agent_name = agent_name
+        # 分页对象
+        self.page_info = page_info
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.agent_name, 'agent_name')
+        self.validate_required(self.page_info, 'page_info')
+        if self.page_info:
+            self.page_info.validate()
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.agent_name is not None:
+            result['agent_name'] = self.agent_name
+        if self.page_info is not None:
+            result['page_info'] = self.page_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('agent_name') is not None:
+            self.agent_name = m.get('agent_name')
+        if m.get('page_info') is not None:
+            temp_model = PageQuery()
+            self.page_info = temp_model.from_map(m['page_info'])
+        return self
+
+
+class PagequeryInnerMerchantagentResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        total_size: int = None,
+        merchant_agent_page: List[MerchantAgentPage] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 数据总量
+        self.total_size = total_size
+        # 代理租户分页对象
+        self.merchant_agent_page = merchant_agent_page
+
+    def validate(self):
+        if self.merchant_agent_page:
+            for k in self.merchant_agent_page:
+                if k:
+                    k.validate()
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
+        if self.total_size is not None:
+            result['total_size'] = self.total_size
+        result['merchant_agent_page'] = []
+        if self.merchant_agent_page is not None:
+            for k in self.merchant_agent_page:
+                result['merchant_agent_page'].append(k.to_map() if k else None)
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
+        if m.get('total_size') is not None:
+            self.total_size = m.get('total_size')
+        self.merchant_agent_page = []
+        if m.get('merchant_agent_page') is not None:
+            for k in m.get('merchant_agent_page'):
+                temp_model = MerchantAgentPage()
+                self.merchant_agent_page.append(temp_model.from_map(k))
+        return self
+
+
+class CloneInnerTemplatefileaddressRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        file_key: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 模板编码
+        self.template_code = template_code
+        # 文件key
+        self.file_key = file_key
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.file_key, 'file_key')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class CloneInnerTemplatefileaddressResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        file_key: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 拷贝后的文件key
+        self.file_key = file_key
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
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
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
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class QueryInnerSignfieldsRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库模板code
+        self.template_code = template_code
+        # 魔法库模板版本
+        self.template_version = template_version
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        return self
+
+
+class QueryInnerSignfieldsResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        sign_field_list: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 签署区列表
+        self.sign_field_list = sign_field_list
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
+        if self.sign_field_list is not None:
+            result['sign_field_list'] = self.sign_field_list
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
+        if m.get('sign_field_list') is not None:
+            self.sign_field_list = m.get('sign_field_list')
+        return self
+
+
+class SyncInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        source_template_code: str = None,
+        target_template_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 来源魔法库模板code
+        self.source_template_code = source_template_code
+        # 目标模板名称
+        self.target_template_name = target_template_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.source_template_code, 'source_template_code')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.source_template_code is not None:
+            result['source_template_code'] = self.source_template_code
+        if self.target_template_name is not None:
+            result['target_template_name'] = self.target_template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('source_template_code') is not None:
+            self.source_template_code = m.get('source_template_code')
+        if m.get('target_template_name') is not None:
+            self.target_template_name = m.get('target_template_name')
+        return self
+
+
+class SyncInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        target_template_code: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 同步后的新模板code
+        self.target_template_code = target_template_code
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
+        if self.target_template_code is not None:
+            result['target_template_code'] = self.target_template_code
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
+        if m.get('target_template_code') is not None:
+            self.target_template_code = m.get('target_template_code')
+        return self
+
+
+class UpdateInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_version_id: str = None,
+        template_name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 商户对应租户ID
+        self.tenant_id = tenant_id
+        # 魔法库版本id
+        self.template_version_id = template_version_id
+        # 模板名称
+        self.template_name = template_name
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_version_id, 'template_version_id')
+        self.validate_required(self.template_name, 'template_name')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_version_id is not None:
+            result['template_version_id'] = self.template_version_id
+        if self.template_name is not None:
+            result['template_name'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_version_id') is not None:
+            self.template_version_id = m.get('template_version_id')
+        if m.get('template_name') is not None:
+            self.template_name = m.get('template_name')
+        return self
+
+
+class UpdateInnerTemplateResponse(TeaModel):
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
+class QueryInnerTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        template_code: str = None,
+        tenant_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 模板code
+        self.template_code = template_code
+        # 租户8位id
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.tenant_id, 'tenant_id')
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
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        return self
+
+
+class QueryInnerTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板的基本信息，json格式
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class QueryTemplateElementlinkRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        template_code: str = None,
+        template_version: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户id
+        self.tenant_id = tenant_id
+        # 模板code
+        self.template_code = template_code
+        # 模板版本
+        self.template_version = template_version
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.template_code, 'template_code')
+        self.validate_required(self.template_version, 'template_version')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.template_code is not None:
+            result['template_code'] = self.template_code
+        if self.template_version is not None:
+            result['template_version'] = self.template_version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('template_code') is not None:
+            self.template_code = m.get('template_code')
+        if m.get('template_version') is not None:
+            self.template_version = m.get('template_version')
+        return self
+
+
+class QueryTemplateElementlinkResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 模板元素列表，json格式
+        self.data = data
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
+        if self.data is not None:
+            result['data'] = self.data
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
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class RegisterMerchantexpandMerchantRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        company_info: CompanyInfo = None,
+        legal_info: LegalInfo = None,
+        application_info: ApplicationInfo = None,
+        expand_mode: str = None,
+        sub_tenant_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 公司信息
+        self.company_info = company_info
+        # 法人信息
+        self.legal_info = legal_info
+        # 应用信息
+        self.application_info = application_info
+        # 进件模式 DIRECT(直连进件) AGENT(代理进件)
+        self.expand_mode = expand_mode
+        # expand_mode=_AGENT_ 必填
+        self.sub_tenant_id = sub_tenant_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.company_info, 'company_info')
+        if self.company_info:
+            self.company_info.validate()
+        self.validate_required(self.legal_info, 'legal_info')
+        if self.legal_info:
+            self.legal_info.validate()
+        self.validate_required(self.application_info, 'application_info')
+        if self.application_info:
+            self.application_info.validate()
+        self.validate_required(self.expand_mode, 'expand_mode')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.company_info is not None:
+            result['company_info'] = self.company_info.to_map()
+        if self.legal_info is not None:
+            result['legal_info'] = self.legal_info.to_map()
+        if self.application_info is not None:
+            result['application_info'] = self.application_info.to_map()
+        if self.expand_mode is not None:
+            result['expand_mode'] = self.expand_mode
+        if self.sub_tenant_id is not None:
+            result['sub_tenant_id'] = self.sub_tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('company_info') is not None:
+            temp_model = CompanyInfo()
+            self.company_info = temp_model.from_map(m['company_info'])
+        if m.get('legal_info') is not None:
+            temp_model = LegalInfo()
+            self.legal_info = temp_model.from_map(m['legal_info'])
+        if m.get('application_info') is not None:
+            temp_model = ApplicationInfo()
+            self.application_info = temp_model.from_map(m['application_info'])
+        if m.get('expand_mode') is not None:
+            self.expand_mode = m.get('expand_mode')
+        if m.get('sub_tenant_id') is not None:
+            self.sub_tenant_id = m.get('sub_tenant_id')
+        return self
+
+
+class RegisterMerchantexpandMerchantResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        pay_expand_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 进件流水号
+        self.pay_expand_id = pay_expand_id
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
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
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
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        return self
+
+
+class UploadMerchantexpandFileRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        file_name: str = None,
+        biz_scene: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 文件名称 包含后缀
+        self.file_name = file_name
+        # ● BUSINESS_LICENSE 营业执照 ● CARD_FRONT 身份证正面 ● CARD_BACK 身份证反面 ● SPLITTING 分账
+        self.biz_scene = biz_scene
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.biz_scene, 'biz_scene')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.biz_scene is not None:
+            result['biz_scene'] = self.biz_scene
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('biz_scene') is not None:
+            self.biz_scene = m.get('biz_scene')
+        return self
+
+
+class UploadMerchantexpandFileResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        upload_url: str = None,
+        file_key: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 临时上传文件地址
+        self.upload_url = upload_url
+        # 文件key
+        self.file_key = file_key
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
+        if self.upload_url is not None:
+            result['upload_url'] = self.upload_url
+        if self.file_key is not None:
+            result['file_key'] = self.file_key
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
+        if m.get('upload_url') is not None:
+            self.upload_url = m.get('upload_url')
+        if m.get('file_key') is not None:
+            self.file_key = m.get('file_key')
+        return self
+
+
+class QueryMerchantexpandMerchantRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        tenant_id: str = None,
+        pay_expand_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户ID
+        self.tenant_id = tenant_id
+        # 商户入驻返回的进件编号 expand_mode=AGENT必填
+        self.pay_expand_id = pay_expand_id
+
+    def validate(self):
+        self.validate_required(self.tenant_id, 'tenant_id')
+        self.validate_required(self.pay_expand_id, 'pay_expand_id')
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
+        if self.tenant_id is not None:
+            result['tenant_id'] = self.tenant_id
+        if self.pay_expand_id is not None:
+            result['pay_expand_id'] = self.pay_expand_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('tenant_id') is not None:
+            self.tenant_id = m.get('tenant_id')
+        if m.get('pay_expand_id') is not None:
+            self.pay_expand_id = m.get('pay_expand_id')
+        return self
+
+
+class QueryMerchantexpandMerchantResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        enrollment_status: str = None,
+        fail_reason: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 商户入驻状态
+        # INIT 入驻中
+        # SUCCESS 入驻成功
+        # FAIL 入驻失败
+        self.enrollment_status = enrollment_status
+        # 入驻失败原因
+        self.fail_reason = fail_reason
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
+        if self.enrollment_status is not None:
+            result['enrollment_status'] = self.enrollment_status
+        if self.fail_reason is not None:
+            result['fail_reason'] = self.fail_reason
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
+        if m.get('enrollment_status') is not None:
+            self.enrollment_status = m.get('enrollment_status')
+        if m.get('fail_reason') is not None:
+            self.fail_reason = m.get('fail_reason')
+        return self
+
+
 class CreateRealpersonFacevrfRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         cert_name: str = None,
         cert_no: str = None,
@@ -3213,14 +8182,190 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('data') is not None:
             self.data = m.get('data')
         return self
 
 
+class QueryRiskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        user_name: str = None,
+        cert_no: str = None,
+        mobile: str = None,
+        ip: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 账户ID
+        self.user_id = user_id
+        # 用户姓名
+        self.user_name = user_name
+        # 用户证件号码
+        self.cert_no = cert_no
+        # 用户手机号码
+        self.mobile = mobile
+        # 用户ip地址
+        self.ip = ip
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.user_name, 'user_name')
+        self.validate_required(self.cert_no, 'cert_no')
+        self.validate_required(self.mobile, 'mobile')
+        self.validate_required(self.ip, 'ip')
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
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.user_name is not None:
+            result['user_name'] = self.user_name
+        if self.cert_no is not None:
+            result['cert_no'] = self.cert_no
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
+        if self.ip is not None:
+            result['ip'] = self.ip
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('user_name') is not None:
+            self.user_name = m.get('user_name')
+        if m.get('cert_no') is not None:
+            self.cert_no = m.get('cert_no')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
+        if m.get('ip') is not None:
+            self.ip = m.get('ip')
+        return self
+
+
+class QueryRiskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        security_id: str = None,
+        decision: str = None,
+        scenes: List[RiskScene] = None,
+        strategies: List[RiskStrategy] = None,
+        models: List[RiskModel] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 请求唯一ID标识，为空则是异常
+        self.security_id = security_id
+        # 总风险决策结果，枚举值为：reject[拒绝],validate[待定],accept[通过]。
+        self.decision = decision
+        # 风险场景的决策结果
+        self.scenes = scenes
+        # 策略结果详情
+        self.strategies = strategies
+        # 模型结果详情
+        self.models = models
+
+    def validate(self):
+        if self.scenes:
+            for k in self.scenes:
+                if k:
+                    k.validate()
+        if self.strategies:
+            for k in self.strategies:
+                if k:
+                    k.validate()
+        if self.models:
+            for k in self.models:
+                if k:
+                    k.validate()
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
+        if self.security_id is not None:
+            result['security_id'] = self.security_id
+        if self.decision is not None:
+            result['decision'] = self.decision
+        result['scenes'] = []
+        if self.scenes is not None:
+            for k in self.scenes:
+                result['scenes'].append(k.to_map() if k else None)
+        result['strategies'] = []
+        if self.strategies is not None:
+            for k in self.strategies:
+                result['strategies'].append(k.to_map() if k else None)
+        result['models'] = []
+        if self.models is not None:
+            for k in self.models:
+                result['models'].append(k.to_map() if k else None)
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
+        if m.get('security_id') is not None:
+            self.security_id = m.get('security_id')
+        if m.get('decision') is not None:
+            self.decision = m.get('decision')
+        self.scenes = []
+        if m.get('scenes') is not None:
+            for k in m.get('scenes'):
+                temp_model = RiskScene()
+                self.scenes.append(temp_model.from_map(k))
+        self.strategies = []
+        if m.get('strategies') is not None:
+            for k in m.get('strategies'):
+                temp_model = RiskStrategy()
+                self.strategies.append(temp_model.from_map(k))
+        self.models = []
+        if m.get('models') is not None:
+            for k in m.get('models'):
+                temp_model = RiskModel()
+                self.models.append(temp_model.from_map(k))
+        return self
+
+
 class AllSignTemplateRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         contract_type: str = None,
         merchant_id: str = None,
@@ -3428,15 +8573,14 @@
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
@@ -3989,15 +9133,14 @@
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
@@ -4324,14 +9467,149 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('file_item_no') is not None:
             self.file_item_no = m.get('file_item_no')
         return self
 
 
+class UploadSignTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        merchant_id: str = None,
+        template_args: str = None,
+        pos_conf: str = None,
+        agreement_type: str = None,
+        file_object: BinaryIO = None,
+        file_object_name: str = None,
+        file_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 订单所属商户的统一社会信用代码
+        self.merchant_id = merchant_id
+        # 模板参数
+        self.template_args = template_args
+        # 签署区坐标配置
+        self.pos_conf = pos_conf
+        # 模板类型
+        self.agreement_type = agreement_type
+        # 上传的pdf文件，需要以.pdf后缀结尾
+        # 待上传文件
+        self.file_object = file_object
+        # 待上传文件名
+        self.file_object_name = file_object_name
+        self.file_id = file_id
+
+    def validate(self):
+        self.validate_required(self.merchant_id, 'merchant_id')
+        self.validate_required(self.pos_conf, 'pos_conf')
+        self.validate_required(self.agreement_type, 'agreement_type')
+        self.validate_required(self.file_id, 'file_id')
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
+        if self.merchant_id is not None:
+            result['merchant_id'] = self.merchant_id
+        if self.template_args is not None:
+            result['template_args'] = self.template_args
+        if self.pos_conf is not None:
+            result['pos_conf'] = self.pos_conf
+        if self.agreement_type is not None:
+            result['agreement_type'] = self.agreement_type
+        if self.file_object is not None:
+            result['fileObject'] = self.file_object
+        if self.file_object_name is not None:
+            result['fileObjectName'] = self.file_object_name
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('merchant_id') is not None:
+            self.merchant_id = m.get('merchant_id')
+        if m.get('template_args') is not None:
+            self.template_args = m.get('template_args')
+        if m.get('pos_conf') is not None:
+            self.pos_conf = m.get('pos_conf')
+        if m.get('agreement_type') is not None:
+            self.agreement_type = m.get('agreement_type')
+        if m.get('fileObject') is not None:
+            self.file_object = m.get('fileObject')
+        if m.get('fileObjectName') is not None:
+            self.file_object_name = m.get('fileObjectName')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        return self
+
+
+class UploadSignTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        template_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 上传模板后返回的模板id
+        self.template_id = template_id
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
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
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
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        return self
+
+
 class SyncTradeRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_content: str = None,
         type: str = None,
@@ -5052,51 +10330,363 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('response_data') is not None:
             self.response_data = m.get('response_data')
         return self
 
 
+class UpdateTradeUserpromiseRequest(TeaModel):
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
+class UpdateTradeUserpromiseResponse(TeaModel):
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
+class SyncFrontIndirectorderRequest(TeaModel):
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
+class SyncFrontIndirectorderResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        response_data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 返回值，json字符串
+        self.response_data = response_data
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
+        if self.response_data is not None:
+            result['response_data'] = self.response_data
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
+        if m.get('response_data') is not None:
+            self.response_data = m.get('response_data')
+        return self
+
+
+class SyncTradeIndirectorderRequest(TeaModel):
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
+class SyncTradeIndirectorderResponse(TeaModel):
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
 class CreateWithholdSignRequest(TeaModel):
     def __init__(
         self,
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
@@ -5110,14 +10700,16 @@
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
@@ -5128,14 +10720,16 @@
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
 
 
 class CreateWithholdSignResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -5505,26 +11099,26 @@
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
@@ -5532,18 +11126,16 @@
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
```

### Comparing `antchain_ato-1.7.26/setup.py` & `antchain_ato-1.8.51/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ato.
 
-Created on 09/05/2024
+Created on 23/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ato"
 NAME = "antchain_ato" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain ATO SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

