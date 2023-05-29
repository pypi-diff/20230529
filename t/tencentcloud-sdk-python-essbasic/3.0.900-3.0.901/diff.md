# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.900.tar", last modified: Fri May 26 02:18:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.901.tar", last modified: Mon May 29 02:27:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.900.tar` & `tencentcloud-sdk-python-essbasic-3.0.901.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16065 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   231689 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:18:43.000000 tencentcloud-sdk-python-essbasic-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51460 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   232146 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:27:46.000000 tencentcloud-sdk-python-essbasic-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.900'
+__version__ = '3.0.901'
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,17 @@
 
 # 参数错误。
 INVALIDPARAMETER_PARAMERROR = 'InvalidParameter.ParamError'
 
 # 资源类型错误。
 INVALIDPARAMETER_RESOURCETYPE = 'InvalidParameter.ResourceType'
 
+# 角色ID不正确
+INVALIDPARAMETER_ROLEID = 'InvalidParameter.RoleId'
+
 # 文件内容敏感信息。
 INVALIDPARAMETER_SENSITIVEFILECONTENT = 'InvalidParameter.SensitiveFileContent'
 
 # 参数错误，不合法的签署控件类型，请修改后重试。
 INVALIDPARAMETER_SIGNCOMPONENTTYPE = 'InvalidParameter.SignComponentType'
 
 # 类型不支持。
@@ -379,14 +382,17 @@
 
 # 无权操作合同。
 OPERATIONDENIED_NOFLOWPERMISSION = 'OperationDenied.NoFlowPermission'
 
 # 未通过个人实名。
 OPERATIONDENIED_NOIDENTITYVERIFY = 'OperationDenied.NoIdentityVerify'
 
+# 无权限进行操作
+OPERATIONDENIED_NOPERMISSIONUSERESOURCE = 'OperationDenied.NoPermissionUseResource'
+
 # 流程配额不足。
 OPERATIONDENIED_NOQUOTA = 'OperationDenied.NoQuota'
 
 # 不属于企业超管或者法人。
 OPERATIONDENIED_NOTBELONGSUPERADMINORLEGALPERSON = 'OperationDenied.NotBelongSuperAdminOrLegalPerson'
 
 # 操作类型不支持。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,18 +273,19 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateFlowSignReview(self, request):
-        """提交企业签署流程审批结果
+        """提交企业流程审批结果
+        目前存在两种审核操作，签署审核，发起审核
+        签署审核：通过接口（CreateFlowsByTemplates或ChannelCreateFlowByFiles或ChannelCreatePrepareFlow）发起签署流程后，若指定了参数 NeedSignReview 为true,则可以调用此接口，指定operate=SignReview，提交企业内部签署审批结果；若签署流程状态正常，且本企业存在签署方未签署，同一签署流程可以多次提交签署审批结果，签署时的最后一个“审批结果”有效
 
-        在通过接口(CreateFlowsByTemplates 或者ChannelCreateFlowByFiles)创建签署流程时，若指定了参数 NeedSignReview 为true,则可以调用此接口提交企业内部签署审批结果。
-        若签署流程状态正常，且本企业存在签署方未签署，同一签署流程可以多次提交签署审批结果，签署时的最后一个“审批结果”有效。
+        发起审核：通过接口ChannelCreatePrepareFlow指定发起后需要审核，则可以通过调用此接口，指定operate=CreateReview，提交企业内部审批结果，可多次提交，当通过后，后续提交结果无效
 
         :param request: Request instance for ChannelCreateFlowSignReview.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowSignReviewRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowSignReviewResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1019,30 +1019,37 @@
 SIGN_REJECT:拒签(流程结束)
         :type ReviewType: str
         :param ReviewMessage: 审核原因 
 当ReviewType 是REJECT 时此字段必填,字符串长度不超过200
         :type ReviewMessage: str
         :param RecipientId: 签署节点审核时需要指定
         :type RecipientId: str
+        :param OperateType: 操作类型，默认：SignReview；SignReview:签署审核，CreateReview：发起审核
+注：接口通过该字段区分操作类型
+该字段不传或者为空，则默认为SignReview签署审核，走签署审核流程
+若想使用发起审核，请指定该字段为：CreateReview
+        :type OperateType: str
         """
         self.Agent = None
         self.FlowId = None
         self.ReviewType = None
         self.ReviewMessage = None
         self.RecipientId = None
+        self.OperateType = None
 
 
     def _deserialize(self, params):
         if params.get("Agent") is not None:
             self.Agent = Agent()
             self.Agent._deserialize(params.get("Agent"))
         self.FlowId = params.get("FlowId")
         self.ReviewType = params.get("ReviewType")
         self.ReviewMessage = params.get("ReviewMessage")
         self.RecipientId = params.get("RecipientId")
+        self.OperateType = params.get("OperateType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1260,15 +1267,15 @@
         :type FlowInfo: :class:`tencentcloud.essbasic.v20210526.models.BaseFlowInfo`
         :param FlowApproverList: 合同签署人信息
         :type FlowApproverList: list of CommonFlowApprover
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param FlowOption: 合同流程配置信息
         :type FlowOption: :class:`tencentcloud.essbasic.v20210526.models.CreateFlowOption`
-        :param FlowId: 该参数不可用，请通过获取 web 可嵌入接口获取合同流程预览 URL
+        :param FlowId: 通过flowid快速获得之前成功通过页面发起的合同生成链接
         :type FlowId: str
         :param NeedPreview: 该参数不可用，请通过获取 web 可嵌入接口获取合同流程预览 URL
         :type NeedPreview: bool
         :param Organization: 企业机构信息，不用传
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
         :param Operator: 操作人（用户）信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
@@ -1565,15 +1572,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Agent: 代理信息
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
-        :param RoleId: 角色Id
+        :param RoleId: 角色Id（非超管或法人角色Id）
         :type RoleId: str
         :param UserIds: 用户列表
         :type UserIds: list of str
         :param Operator: 操作人信息
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self.Agent = None
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.901/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.900/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.901/setup.py`

 * *Files identical despite different names*

