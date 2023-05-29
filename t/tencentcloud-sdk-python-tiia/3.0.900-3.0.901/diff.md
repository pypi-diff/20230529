# Comparing `tmp/tencentcloud-sdk-python-tiia-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-tiia-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.900.tar", last modified: Fri May 26 02:29:56 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiia-3.0.901.tar", last modified: Mon May 29 02:39:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiia-3.0.900.tar` & `tencentcloud-sdk-python-tiia-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/
--rw-r--r--   0 root         (0) root         (0)    32444 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/tiia_client.py
--rw-r--r--   0 root         (0) root         (0)     7113 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102357 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:29:56.000000 tencentcloud-sdk-python-tiia-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/
+-rw-r--r--   0 root         (0) root         (0)    32443 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/tiia_client.py
+-rw-r--r--   0 root         (0) root         (0)     7218 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102395 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:39:01.000000 tencentcloud-sdk-python-tiia-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/README.rst` & `tencentcloud-sdk-python-tiia-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.901/tencentcloud_sdk_python_tiia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/tiia_client.py` & `tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/tiia_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
             在自建图库中搜索相似的图案、logo、纹理等图像元素或主体，并给出相似度打分。</td>
             </tr>
         </table>
 
         >
         - 可前往 [图像搜索](https://cloud.tencent.com/document/product/1589) 产品文档中查看更多产品信息。
 
-
         :param request: Request instance for CreateGroup.
         :type request: :class:`tencentcloud.tiia.v20190529.models.CreateGroupRequest`
         :rtype: :class:`tencentcloud.tiia.v20190529.models.CreateGroupResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/errorcodes.py` & `tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 # 文件下载失败。
 FAILEDOPERATION_DOWNLOADERROR = 'FailedOperation.DownLoadError'
 
 # 图片内容为空。
 FAILEDOPERATION_EMPTYIMAGEERROR = 'FailedOperation.EmptyImageError'
 
+# 图库数量超出限制。
+FAILEDOPERATION_GROUPCOUNTEXCEEDED = 'FailedOperation.GroupCountExceeded'
+
 # 图片解码失败。
 FAILEDOPERATION_IMAGEDECODEFAILED = 'FailedOperation.ImageDecodeFailed'
 
 # 图片删除失败。
 FAILEDOPERATION_IMAGEDELETEFAILED = 'FailedOperation.ImageDeleteFailed'
 
 # 图片下载错误。
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/tencentcloud/tiia/v20190529/models.py` & `tencentcloud-sdk-python-tiia-3.0.901/tencentcloud/tiia/v20190529/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
 class CreateGroupRequest(AbstractModel):
     """CreateGroup请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param GroupId: 图库ID，不可重复，仅支持字母、数字和下划线。
+        :param GroupId: 图库ID，不可重复，仅支持字母、数字和下划线。图库数量单个用户上限为30。
         :type GroupId: str
         :param GroupName: 图库名称描述。
         :type GroupName: str
         :param MaxCapacity: 图片库可容纳的最大图片特征条数，一张图片对应一条图片特征数据，不支持修改。
 单个图片库容量最大可达亿级，达到容量限制后继续创建图片将会报错。
 注意，包月计费下支持绑定的最小库容量为500万。
         :type MaxCapacity: int
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-tiia-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiia
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Tiia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiia-3.0.900/setup.py` & `tencentcloud-sdk-python-tiia-3.0.901/setup.py`

 * *Files identical despite different names*

