# Comparing `tmp/alibabacloud_drds20171016-1.0.0.tar.gz` & `tmp/alibabacloud_drds20171016-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_drds20171016-1.0.0.tar", last modified: Fri Oct 29 07:20:15 2021, max compression
+gzip compressed data, was "dist/alibabacloud_drds20171016-1.0.1.tar", last modified: Thu May 23 17:13:15 2024, max compression
```

## Comparing `alibabacloud_drds20171016-1.0.0.tar` & `alibabacloud_drds20171016-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2369 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016/
--rw-r--r--   0 root         (0) root         (0)       21 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88978 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016/client.py
--rw-r--r--   0 root         (0) root         (0)   165484 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2369 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2021-10-29 07:20:15.000000 alibabacloud_drds20171016-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   118312 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016/client.py
+-rw-r--r--   0 root         (0) root         (0)   172992 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 17:13:15.000000 alibabacloud_drds20171016-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-23 17:13:14.000000 alibabacloud_drds20171016-1.0.1/setup.py
```

### Comparing `alibabacloud_drds20171016-1.0.0/LICENSE` & `alibabacloud_drds20171016-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_drds20171016-1.0.0/PKG-INFO` & `alibabacloud_drds20171016-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_drds20171016
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Distributed Relational Database Service (20171016) SDK Library for Python
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
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/drds-20171016/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_drds20171016-1.0.0/README-CN.md` & `alibabacloud_drds20171016-1.0.1/README-CN.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/drds-20171016/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_drds20171016-1.0.0/README.md` & `alibabacloud_drds20171016-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/drds-20171016/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016/models.py` & `alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,18 @@
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         password: str = None,
         user_name: str = None,
     ):
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
         self.password = password
+        # This parameter is required.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -82,41 +84,45 @@
         return self
 
 
 class CreateDrdsAccountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateDrdsAccountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDrdsAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDrdsDBRequest(TeaModel):
@@ -124,18 +130,23 @@
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         encode: str = None,
         password: str = None,
         rds_instances: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.encode = encode
+        # This parameter is required.
         self.password = password
+        # This parameter is required.
         self.rds_instances = rds_instances
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -203,41 +214,45 @@
         return self
 
 
 class CreateDrdsDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateDrdsDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDrdsDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateDrdsInstanceRequest(TeaModel):
@@ -261,22 +276,28 @@
     ):
         self.client_token = client_token
         self.description = description
         self.duration = duration
         self.instance_series = instance_series
         self.is_auto_renew = is_auto_renew
         self.is_ha = is_ha
+        # This parameter is required.
         self.pay_type = pay_type
         self.pricing_cycle = pricing_cycle
+        # This parameter is required.
         self.quantity = quantity
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.specification = specification
+        # This parameter is required.
         self.type = type
         self.vpc_id = vpc_id
         self.vswitch_id = vswitch_id
+        # This parameter is required.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -454,56 +475,63 @@
         return self
 
 
 class CreateDrdsInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateDrdsInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateDrdsInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateReadOnlyAccountRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         password: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.password = password
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -610,54 +638,60 @@
         return self
 
 
 class CreateReadOnlyAccountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: CreateReadOnlyAccountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateReadOnlyAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteDrdsDBRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -713,54 +747,60 @@
         return self
 
 
 class DeleteDrdsDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteDrdsDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteDrdsDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFailedDrdsDBRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -816,52 +856,57 @@
         return self
 
 
 class DeleteFailedDrdsDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DeleteFailedDrdsDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteFailedDrdsDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCreateDrdsInstanceStatusRequest(TeaModel):
     def __init__(
         self,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -948,54 +993,60 @@
         return self
 
 
 class DescribeCreateDrdsInstanceStatusResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeCreateDrdsInstanceStatusResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCreateDrdsInstanceStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsDBRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1110,55 +1161,61 @@
         return self
 
 
 class DescribeDrdsDBResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsDBResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsDBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsDBIpWhiteListRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         group_name: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
         self.group_name = group_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1283,52 +1340,57 @@
         return self
 
 
 class DescribeDrdsDBIpWhiteListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsDBIpWhiteListResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsDBIpWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsDBsRequest(TeaModel):
     def __init__(
         self,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1474,52 +1536,57 @@
         return self
 
 
 class DescribeDrdsDBsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsDBsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsDBsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsInstanceRequest(TeaModel):
     def __init__(
         self,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1760,41 +1827,45 @@
         return self
 
 
 class DescribeDrdsInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsInstanceDbMonitorRequest(TeaModel):
@@ -1802,18 +1873,23 @@
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         end_time: int = None,
         key: str = None,
         start_time: int = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.end_time = end_time
+        # This parameter is required.
         self.key = key
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2033,41 +2109,45 @@
         return self
 
 
 class DescribeDrdsInstanceDbMonitorResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsInstanceDbMonitorResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsInstanceDbMonitorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsInstanceMonitorRequest(TeaModel):
@@ -2075,18 +2155,22 @@
         self,
         drds_instance_id: str = None,
         end_time: int = None,
         key: str = None,
         period_multiple: int = None,
         start_time: int = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.end_time = end_time
+        # This parameter is required.
         self.key = key
         self.period_multiple = period_multiple
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2306,52 +2390,57 @@
         return self
 
 
 class DescribeDrdsInstanceMonitorResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsInstanceMonitorResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsInstanceMonitorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsInstanceNetInfoForInnerRequest(TeaModel):
     def __init__(
         self,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2503,54 +2592,59 @@
         return self
 
 
 class DescribeDrdsInstanceNetInfoForInnerResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsInstanceNetInfoForInnerResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsInstanceNetInfoForInnerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDrdsInstancesRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         tags: str = None,
         type: str = None,
     ):
+        # This parameter is required.
         self.region_id = region_id
         self.tags = tags
         self.type = type
 
     def validate(self):
         pass
 
@@ -2878,55 +2972,61 @@
         return self
 
 
 class DescribeDrdsInstancesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeDrdsInstancesResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeDrdsInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRdsListRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         region_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3199,54 +3299,60 @@
         return self
 
 
 class DescribeRdsListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRdsListResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRdsListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeReadOnlyAccountRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3349,41 +3455,45 @@
         return self
 
 
 class DescribeReadOnlyAccountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeReadOnlyAccountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeReadOnlyAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRegionsResponseBodyDrdsRegionsDrdsRegionInstanceSeriesListInstanceSeriesSpecListSpec(TeaModel):
@@ -3659,54 +3769,60 @@
         return self
 
 
 class DescribeRegionsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeRegionsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeShardDBsRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3844,56 +3960,63 @@
         return self
 
 
 class DescribeShardDBsResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeShardDBsResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeShardDBsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeShardDbConnectionInfoRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         sub_db_name: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.sub_db_name = sub_db_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4054,41 +4177,45 @@
         return self
 
 
 class DescribeShardDbConnectionInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: DescribeShardDbConnectionInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeShardDbConnectionInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableInstanceRequest(TeaModel):
@@ -4107,14 +4234,15 @@
     ):
         self.backup_id = backup_id
         self.client_token = client_token
         self.db_instance_class = db_instance_class
         self.drds_instance_id = drds_instance_id
         self.engine_version = engine_version
         self.restore_time = restore_time
+        # This parameter is required.
         self.source_db_inst_id = source_db_inst_id
         self.switch_id = switch_id
         self.vpc_id = vpc_id
         self.zone_id = zone_id
 
     def validate(self):
         pass
@@ -4211,56 +4339,63 @@
         return self
 
 
 class EnableInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: EnableInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDrdsDBPasswdRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         new_passwd: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.new_passwd = new_passwd
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4320,54 +4455,60 @@
         return self
 
 
 class ModifyDrdsDBPasswdResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyDrdsDBPasswdResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDrdsDBPasswdResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDrdsInstanceDescriptionRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.description = description
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4423,41 +4564,45 @@
         return self
 
 
 class ModifyDrdsInstanceDescriptionResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyDrdsInstanceDescriptionResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDrdsInstanceDescriptionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyDrdsIpWhiteListRequest(TeaModel):
@@ -4466,18 +4611,21 @@
         db_name: str = None,
         drds_instance_id: str = None,
         group_attribute: str = None,
         group_name: str = None,
         ip_white_list: str = None,
         mode: bool = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
         self.group_attribute = group_attribute
         self.group_name = group_name
+        # This parameter is required.
         self.ip_white_list = ip_white_list
         self.mode = mode
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4550,58 +4698,66 @@
         return self
 
 
 class ModifyDrdsIpWhiteListResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyDrdsIpWhiteListResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyDrdsIpWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyFullTableScanRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         full_table_scan: bool = None,
         table_names: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.full_table_scan = full_table_scan
+        # This parameter is required.
         self.table_names = table_names
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4665,58 +4821,66 @@
         return self
 
 
 class ModifyFullTableScanResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyFullTableScanResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyFullTableScanResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyRdsReadWeightRequest(TeaModel):
     def __init__(
         self,
         db_name: str = None,
         drds_instance_id: str = None,
         instance_names: str = None,
         weights: str = None,
     ):
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.instance_names = instance_names
+        # This parameter is required.
         self.weights = weights
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4780,41 +4944,45 @@
         return self
 
 
 class ModifyRdsReadWeightResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyRdsReadWeightResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyRdsReadWeightResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyReadOnlyAccountPasswordRequest(TeaModel):
@@ -4822,18 +4990,23 @@
         self,
         account_name: str = None,
         db_name: str = None,
         drds_instance_id: str = None,
         new_passwd: str = None,
         origin_password: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
+        # This parameter is required.
         self.new_passwd = new_passwd
+        # This parameter is required.
         self.origin_password = origin_password
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4901,56 +5074,63 @@
         return self
 
 
 class ModifyReadOnlyAccountPasswordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: ModifyReadOnlyAccountPasswordResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyReadOnlyAccountPasswordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class QueryInstanceInfoByConnRequest(TeaModel):
     def __init__(
         self,
         host: str = None,
         port: int = None,
         user_name: str = None,
     ):
+        # This parameter is required.
         self.host = host
+        # This parameter is required.
         self.port = port
+        # This parameter is required.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5211,52 +5391,57 @@
         return self
 
 
 class QueryInstanceInfoByConnResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: QueryInstanceInfoByConnResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryInstanceInfoByConnResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveDrdsInstanceRequest(TeaModel):
     def __init__(
         self,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5308,56 +5493,63 @@
         return self
 
 
 class RemoveDrdsInstanceResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RemoveDrdsInstanceResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveDrdsInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RemoveReadOnlyAccountRequest(TeaModel):
     def __init__(
         self,
         account_name: str = None,
         db_name: str = None,
         drds_instance_id: str = None,
     ):
+        # This parameter is required.
         self.account_name = account_name
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.drds_instance_id = drds_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5417,40 +5609,44 @@
         return self
 
 
 class RemoveReadOnlyAccountResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: RemoveReadOnlyAccountResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveReadOnlyAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_drds20171016-1.0.0/alibabacloud_drds20171016.egg-info/PKG-INFO` & `alibabacloud_drds20171016-1.0.1/alibabacloud_drds20171016.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-drds20171016
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Distributed Relational Database Service (20171016) SDK Library for Python
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
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/drds-20171016/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_drds20171016-1.0.0/setup.py` & `alibabacloud_drds20171016-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_drds20171016.
 
-Created on 29/10/2021
+Created on 23/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_drds20171016"
 NAME = "alibabacloud_drds20171016" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Distributed Relational Database Service (20171016) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.7, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

