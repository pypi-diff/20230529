# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.900.tar", last modified: Fri May 26 02:18:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.901.tar", last modified: Mon May 29 02:27:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.900.tar` & `tencentcloud-sdk-python-ess-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51121 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23810 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223871 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:18:37.000000 tencentcloud-sdk-python-ess-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51121 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23810 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223871 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:27:39.000000 tencentcloud-sdk-python-ess-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.900/README.rst` & `tencentcloud-sdk-python-ess-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateBatchCancelFlowUrl(self, request):
-        """注：此接口建会废弃，请使用撤销单个签署流程（CancelFlow）接口。
+        """注：此接口将会废弃，请使用撤销单个签署流程（CancelFlow）接口。
         指定需要批量撤回的签署流程Id，获取批量撤销链接。
         客户指定需要撤回的签署流程Id，最多100个，超过100不处理；接口调用成功返回批量撤回合同的链接，通过链接跳转到电子签小程序完成批量撤回。
 
         :param request: Request instance for CreateBatchCancelFlowUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateBatchCancelFlowUrlResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.900/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.901/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.900/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.901/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.900/setup.py` & `tencentcloud-sdk-python-ess-3.0.901/setup.py`

 * *Files identical despite different names*

