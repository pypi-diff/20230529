# Comparing `tmp/tencentcloud-sdk-python-cynosdb-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-cynosdb-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.900.tar", last modified: Fri May 26 02:15:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cynosdb-3.0.901.tar", last modified: Mon May 29 02:25:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cynosdb-3.0.900.tar` & `tencentcloud-sdk-python-cynosdb-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)    99466 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)    10242 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   341152 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:15:58.000000 tencentcloud-sdk-python-cynosdb-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)    99466 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    10242 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   341152 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:25:07.000000 tencentcloud-sdk-python-cynosdb-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/README.rst` & `tencentcloud-sdk-python-cynosdb-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateParamTemplate(self, request):
-        """本接口（CreateParamTemplate）用于创建参数模版
+        """本接口（CreateParamTemplate）用于创建参数模板
 
         :param request: Request instance for CreateParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.CreateParamTemplateRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.CreateParamTemplateResponse`
 
         """
         try:
@@ -483,15 +483,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteParamTemplate(self, request):
-        """本接口（DeleteParamTemplate）用于删除用户创建的参数模版。
+        """本接口（DeleteParamTemplate）用于删除用户创建的参数模板。
 
         :param request: Request instance for DeleteParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DeleteParamTemplateRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DeleteParamTemplateResponse`
 
         """
         try:
@@ -1173,15 +1173,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeParamTemplateDetail(self, request):
-        """本接口（DescribeParamTemplateDetail）用于查询用户参数模版详情
+        """本接口（DescribeParamTemplateDetail）用于查询用户参数模板详情
 
         :param request: Request instance for DescribeParamTemplateDetail.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.DescribeParamTemplateDetailRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.DescribeParamTemplateDetailResponse`
 
         """
         try:
@@ -1955,15 +1955,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyParamTemplate(self, request):
-        """本接口（ModifyParamTemplate）用于修改用户参数模版。
+        """本接口（ModifyParamTemplate）用于修改用户参数模板。
 
         :param request: Request instance for ModifyParamTemplate.
         :type request: :class:`tencentcloud.cynosdb.v20190107.models.ModifyParamTemplateRequest`
         :rtype: :class:`tencentcloud.cynosdb.v20190107.models.ModifyParamTemplateResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/cynosdb/v20190107/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.901/tencentcloud_sdk_python_cynosdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-cynosdb-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cynosdb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cynosdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cynosdb-3.0.900/setup.py` & `tencentcloud-sdk-python-cynosdb-3.0.901/setup.py`

 * *Files identical despite different names*

