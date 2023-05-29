# Comparing `tmp/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0.tar.gz` & `tmp/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0.tar", last modified: Thu May 25 07:01:55 2023, max compression
+gzip compressed data, was "dist/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1.tar", last modified: Mon May 29 08:22:39 2023, max compression
```

## Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0.tar` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:01:55.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-25 07:01:55.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:01:55.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:01:55.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17850 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/client.py
--rw-r--r--   0 root         (0) root         (0)    10929 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-25 07:01:55.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-25 07:01:54.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20446 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/client.py
+-rw-r--r--   0 root         (0) root         (0)    13683 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-29 08:22:39.000000 antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/setup.py
```

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/LICENSE` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/PKG-INFO` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_039036ceaf344eae826f7a5f2e0c0a1a SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/README-CN.md` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/README.md` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/PKG-INFO` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-039036ceaf344eae826f7a5f2e0c0a1a
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_039036ceaf344eae826f7a5f2e0c0a1a SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/SOURCES.txt` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/client.py` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_039036ceaf344eae826f7a5f2e0c0a1a',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_039036ceaf344eae826f7a5f2e0c0a1a',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -380,7 +380,63 @@
         Summary: 自动化测试创建（勿动）
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoAaaBbbCccResponse(),
             await self.do_request_async('1.0', 'demo.aaa.bbb.ccc.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_demo_approval_test(
+        self,
+        request: ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestRequest,
+    ) -> ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse:
+        """
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_demo_approval_test_ex(request, headers, runtime)
+
+    async def query_demo_approval_test_async(
+        self,
+        request: ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestRequest,
+    ) -> ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse:
+        """
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_demo_approval_test_ex_async(request, headers, runtime)
+
+    def query_demo_approval_test_ex(
+        self,
+        request: ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse:
+        """
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse(),
+            self.do_request('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_demo_approval_test_ex_async(
+        self,
+        request: ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse:
+        """
+        Description: 用于测试api评审接入SDL的测试使用
+        Summary: api评审测试
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak__039036ceaf_344eae_826f_7a_5f_2e_0c_0a_1a_models.QueryDemoApprovalTestResponse(),
+            await self.do_request_async('1.0', 'demo.approval.test.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/models.py` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -308,7 +308,97 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class QueryDemoApprovalTestRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        input: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 字符串
+        self.input = input
+
+    def validate(self):
+        self.validate_required(self.input, 'input')
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
+        if self.input is not None:
+            result['input'] = self.input
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('input') is not None:
+            self.input = m.get('input')
+        return self
+
+
+class QueryDemoApprovalTestResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 回参
+        self.msg = msg
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
+        if self.msg is not None:
+            result['msg'] = self.msg
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
+        if m.get('msg') is not None:
+            self.msg = m.get('msg')
+        return self
+
+
```

### Comparing `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.0/setup.py` & `antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a.
 
-Created on 25/05/2023
+Created on 29/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_039036ceaf344eae826f7a5f2e0c0a1a"
 NAME = "antchain_ak_039036ceaf344eae826f7a5f2e0c0a1a" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_039036ceaf344eae826f7a5f2e0c0a1a SDK Library for Python"
```

