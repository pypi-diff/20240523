# Comparing `tmp/alibabacloud_es-serverless20230627-1.0.2.tar.gz` & `tmp/alibabacloud_es-serverless20230627-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_es-serverless20230627-1.0.2.tar", last modified: Wed Jan 24 17:18:39 2024, max compression
+gzip compressed data, was "dist/alibabacloud_es-serverless20230627-2.0.0.tar", last modified: Thu May 23 05:11:13 2024, max compression
```

## Comparing `alibabacloud_es-serverless20230627-1.0.2.tar` & `alibabacloud_es-serverless20230627-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      152 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24737 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627/client.py
--rw-r--r--   0 root         (0) root         (0)    59449 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2663 2024-01-24 17:18:39.000000 alibabacloud_es-serverless20230627-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1220 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34651 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627/client.py
+-rw-r--r--   0 root         (0) root         (0)    71439 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2471 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-05-23 05:11:13.000000 alibabacloud_es-serverless20230627-2.0.0/setup.py
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/LICENSE` & `alibabacloud_es-serverless20230627-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_es-serverless20230627-1.0.2/PKG-INFO` & `alibabacloud_es-serverless20230627-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_es-serverless20230627
-Version: 1.0.2
+Version: 2.0.0
 Summary: Alibaba Cloud es-serverless (20230627) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/es-serverless-20230627/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/README-CN.md` & `alibabacloud_es-serverless20230627-2.0.0/README-CN.md`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/es-serverless-20230627/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/README.md` & `alibabacloud_es-serverless20230627-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/es-serverless-20230627/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627/models.py` & `alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -302,27 +302,33 @@
         authentication: CreateAppRequestAuthentication = None,
         charge_type: str = None,
         description: str = None,
         network: List[CreateAppRequestNetwork] = None,
         private_network: List[CreateAppRequestPrivateNetwork] = None,
         quota_info: CreateAppRequestQuotaInfo = None,
         region_id: str = None,
+        scenario: str = None,
         version: str = None,
         dry_run: bool = None,
     ):
         # 应用名
+        # 
+        # This parameter is required.
         self.app_name = app_name
+        # This parameter is required.
         self.authentication = authentication
+        # This parameter is required.
         self.charge_type = charge_type
         # 应用备注
         self.description = description
         self.network = network
         self.private_network = private_network
         self.quota_info = quota_info
         self.region_id = region_id
+        self.scenario = scenario
         self.version = version
         self.dry_run = dry_run
 
     def validate(self):
         if self.authentication:
             self.authentication.validate()
         if self.network:
@@ -358,14 +364,16 @@
         if self.private_network is not None:
             for k in self.private_network:
                 result['privateNetwork'].append(k.to_map() if k else None)
         if self.quota_info is not None:
             result['quotaInfo'] = self.quota_info.to_map()
         if self.region_id is not None:
             result['regionId'] = self.region_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
         if self.version is not None:
             result['version'] = self.version
         if self.dry_run is not None:
             result['dryRun'] = self.dry_run
         return result
 
     def from_map(self, m: dict = None):
@@ -390,14 +398,16 @@
                 temp_model = CreateAppRequestPrivateNetwork()
                 self.private_network.append(temp_model.from_map(k))
         if m.get('quotaInfo') is not None:
             temp_model = CreateAppRequestQuotaInfo()
             self.quota_info = temp_model.from_map(m['quotaInfo'])
         if m.get('regionId') is not None:
             self.region_id = m.get('regionId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
         if m.get('version') is not None:
             self.version = m.get('version')
         if m.get('dryRun') is not None:
             self.dry_run = m.get('dryRun')
         return self
 
 
@@ -471,17 +481,14 @@
         body: CreateAppResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -503,14 +510,206 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateEndpointRequestEndpointZones(TeaModel):
+    def __init__(
+        self,
+        vswitch_id: str = None,
+        zone_id: str = None,
+    ):
+        self.vswitch_id = vswitch_id
+        self.zone_id = zone_id
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
+        if self.vswitch_id is not None:
+            result['vswitchId'] = self.vswitch_id
+        if self.zone_id is not None:
+            result['zoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('vswitchId') is not None:
+            self.vswitch_id = m.get('vswitchId')
+        if m.get('zoneId') is not None:
+            self.zone_id = m.get('zoneId')
+        return self
+
+
+class CreateEndpointRequest(TeaModel):
+    def __init__(
+        self,
+        endpoint_zones: List[CreateEndpointRequestEndpointZones] = None,
+        name: str = None,
+        vpc_id: str = None,
+        type: str = None,
+    ):
+        # This parameter is required.
+        self.endpoint_zones = endpoint_zones
+        self.name = name
+        # This parameter is required.
+        self.vpc_id = vpc_id
+        self.type = type
+
+    def validate(self):
+        if self.endpoint_zones:
+            for k in self.endpoint_zones:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['endpointZones'] = []
+        if self.endpoint_zones is not None:
+            for k in self.endpoint_zones:
+                result['endpointZones'].append(k.to_map() if k else None)
+        if self.name is not None:
+            result['name'] = self.name
+        if self.vpc_id is not None:
+            result['vpcId'] = self.vpc_id
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.endpoint_zones = []
+        if m.get('endpointZones') is not None:
+            for k in m.get('endpointZones'):
+                temp_model = CreateEndpointRequestEndpointZones()
+                self.endpoint_zones.append(temp_model.from_map(k))
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('vpcId') is not None:
+            self.vpc_id = m.get('vpcId')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class CreateEndpointResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        endpoint_id: str = None,
+    ):
+        self.endpoint_id = endpoint_id
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
+        if self.endpoint_id is not None:
+            result['endpointId'] = self.endpoint_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('endpointId') is not None:
+            self.endpoint_id = m.get('endpointId')
+        return self
+
+
+class CreateEndpointResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        result: CreateEndpointResponseBodyResult = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        if m.get('result') is not None:
+            temp_model = CreateEndpointResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class CreateEndpointResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateEndpointResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateEndpointResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteAppResponseBodyResult(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         self.instance_id = instance_id
 
@@ -577,17 +776,14 @@
         body: DeleteAppResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -636,41 +832,248 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('detailed') is not None:
             self.detailed = m.get('detailed')
         return self
 
 
+class GetAppResponseBodyResultNetworkWhiteIpGroup(TeaModel):
+    def __init__(
+        self,
+        group_name: str = None,
+        ips: List[str] = None,
+    ):
+        self.group_name = group_name
+        self.ips = ips
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
+        if self.group_name is not None:
+            result['groupName'] = self.group_name
+        if self.ips is not None:
+            result['ips'] = self.ips
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('groupName') is not None:
+            self.group_name = m.get('groupName')
+        if m.get('ips') is not None:
+            self.ips = m.get('ips')
+        return self
+
+
+class GetAppResponseBodyResultNetwork(TeaModel):
+    def __init__(
+        self,
+        domain: str = None,
+        enabled: bool = None,
+        port: int = None,
+        type: str = None,
+        white_ip_group: List[GetAppResponseBodyResultNetworkWhiteIpGroup] = None,
+    ):
+        self.domain = domain
+        self.enabled = enabled
+        self.port = port
+        self.type = type
+        self.white_ip_group = white_ip_group
+
+    def validate(self):
+        if self.white_ip_group:
+            for k in self.white_ip_group:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.domain is not None:
+            result['domain'] = self.domain
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.port is not None:
+            result['port'] = self.port
+        if self.type is not None:
+            result['type'] = self.type
+        result['whiteIpGroup'] = []
+        if self.white_ip_group is not None:
+            for k in self.white_ip_group:
+                result['whiteIpGroup'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('domain') is not None:
+            self.domain = m.get('domain')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        self.white_ip_group = []
+        if m.get('whiteIpGroup') is not None:
+            for k in m.get('whiteIpGroup'):
+                temp_model = GetAppResponseBodyResultNetworkWhiteIpGroup()
+                self.white_ip_group.append(temp_model.from_map(k))
+        return self
+
+
+class GetAppResponseBodyResultPrivateNetworkWhiteIpGroup(TeaModel):
+    def __init__(
+        self,
+        group_name: str = None,
+        ips: List[str] = None,
+    ):
+        self.group_name = group_name
+        self.ips = ips
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
+        if self.group_name is not None:
+            result['groupName'] = self.group_name
+        if self.ips is not None:
+            result['ips'] = self.ips
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('groupName') is not None:
+            self.group_name = m.get('groupName')
+        if m.get('ips') is not None:
+            self.ips = m.get('ips')
+        return self
+
+
+class GetAppResponseBodyResultPrivateNetwork(TeaModel):
+    def __init__(
+        self,
+        domain: str = None,
+        enabled: bool = None,
+        port: int = None,
+        pvl_endpoint_id: str = None,
+        type: str = None,
+        vpc_id: str = None,
+        white_ip_group: List[GetAppResponseBodyResultPrivateNetworkWhiteIpGroup] = None,
+    ):
+        self.domain = domain
+        self.enabled = enabled
+        self.port = port
+        self.pvl_endpoint_id = pvl_endpoint_id
+        self.type = type
+        self.vpc_id = vpc_id
+        self.white_ip_group = white_ip_group
+
+    def validate(self):
+        if self.white_ip_group:
+            for k in self.white_ip_group:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.domain is not None:
+            result['domain'] = self.domain
+        if self.enabled is not None:
+            result['enabled'] = self.enabled
+        if self.port is not None:
+            result['port'] = self.port
+        if self.pvl_endpoint_id is not None:
+            result['pvlEndpointId'] = self.pvl_endpoint_id
+        if self.type is not None:
+            result['type'] = self.type
+        if self.vpc_id is not None:
+            result['vpcId'] = self.vpc_id
+        result['whiteIpGroup'] = []
+        if self.white_ip_group is not None:
+            for k in self.white_ip_group:
+                result['whiteIpGroup'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('domain') is not None:
+            self.domain = m.get('domain')
+        if m.get('enabled') is not None:
+            self.enabled = m.get('enabled')
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        if m.get('pvlEndpointId') is not None:
+            self.pvl_endpoint_id = m.get('pvlEndpointId')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('vpcId') is not None:
+            self.vpc_id = m.get('vpcId')
+        self.white_ip_group = []
+        if m.get('whiteIpGroup') is not None:
+            for k in m.get('whiteIpGroup'):
+                temp_model = GetAppResponseBodyResultPrivateNetworkWhiteIpGroup()
+                self.white_ip_group.append(temp_model.from_map(k))
+        return self
+
+
 class GetAppResponseBodyResult(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         app_name: str = None,
         create_time: str = None,
         description: str = None,
         instance_id: str = None,
         modified_time: str = None,
+        network: List[GetAppResponseBodyResultNetwork] = None,
         owner_id: str = None,
+        private_network: List[GetAppResponseBodyResultPrivateNetwork] = None,
         region_id: str = None,
         status: str = None,
         version: str = None,
     ):
         self.app_id = app_id
         self.app_name = app_name
         self.create_time = create_time
         self.description = description
         self.instance_id = instance_id
         self.modified_time = modified_time
+        self.network = network
         self.owner_id = owner_id
+        self.private_network = private_network
         self.region_id = region_id
         self.status = status
         self.version = version
 
     def validate(self):
-        pass
+        if self.network:
+            for k in self.network:
+                if k:
+                    k.validate()
+        if self.private_network:
+            for k in self.private_network:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -682,16 +1085,24 @@
             result['createTime'] = self.create_time
         if self.description is not None:
             result['description'] = self.description
         if self.instance_id is not None:
             result['instanceId'] = self.instance_id
         if self.modified_time is not None:
             result['modifiedTime'] = self.modified_time
+        result['network'] = []
+        if self.network is not None:
+            for k in self.network:
+                result['network'].append(k.to_map() if k else None)
         if self.owner_id is not None:
             result['ownerId'] = self.owner_id
+        result['privateNetwork'] = []
+        if self.private_network is not None:
+            for k in self.private_network:
+                result['privateNetwork'].append(k.to_map() if k else None)
         if self.region_id is not None:
             result['regionId'] = self.region_id
         if self.status is not None:
             result['status'] = self.status
         if self.version is not None:
             result['version'] = self.version
         return result
@@ -706,16 +1117,26 @@
             self.create_time = m.get('createTime')
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('instanceId') is not None:
             self.instance_id = m.get('instanceId')
         if m.get('modifiedTime') is not None:
             self.modified_time = m.get('modifiedTime')
+        self.network = []
+        if m.get('network') is not None:
+            for k in m.get('network'):
+                temp_model = GetAppResponseBodyResultNetwork()
+                self.network.append(temp_model.from_map(k))
         if m.get('ownerId') is not None:
             self.owner_id = m.get('ownerId')
+        self.private_network = []
+        if m.get('privateNetwork') is not None:
+            for k in m.get('privateNetwork'):
+                temp_model = GetAppResponseBodyResultPrivateNetwork()
+                self.private_network.append(temp_model.from_map(k))
         if m.get('regionId') is not None:
             self.region_id = m.get('regionId')
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
@@ -764,17 +1185,14 @@
         body: GetAppResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -958,17 +1376,14 @@
         body: GetAppQuotaResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1145,17 +1560,14 @@
         body: GetMonitorDataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1336,14 +1748,15 @@
         self,
         request_id: str = None,
         result: List[ListAppsResponseBodyResult] = None,
         total_count: int = None,
     ):
         self.request_id = request_id
         self.result = result
+        # This parameter is required.
         self.total_count = total_count
 
     def validate(self):
         if self.result:
             for k in self.result:
                 if k:
                     k.validate()
@@ -1386,17 +1799,14 @@
         body: ListAppsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1911,17 +2321,14 @@
         body: UpdateAppResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/alibabacloud_es_serverless20230627.egg-info/PKG-INFO` & `alibabacloud_es-serverless20230627-2.0.0/alibabacloud_es_serverless20230627.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-es-serverless20230627
-Version: 1.0.2
+Version: 2.0.0
 Summary: Alibaba Cloud es-serverless (20230627) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/es-serverless-20230627/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_es-serverless20230627-1.0.2/setup.py` & `alibabacloud_es-serverless20230627-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_es-serverless20230627.
 
-Created on 24/01/2024
+Created on 23/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_es_serverless20230627"
 NAME = "alibabacloud_es-serverless20230627" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud es-serverless (20230627) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

