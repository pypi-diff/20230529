# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.900.tar", last modified: Fri May 26 02:24:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.901.tar", last modified: Mon May 29 02:33:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.900.tar` & `tencentcloud-sdk-python-ocr-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113845 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   508075 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:24:22.000000 tencentcloud-sdk-python-ocr-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   113899 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   508075 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:33:17.000000 tencentcloud-sdk-python-ocr-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.901/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/README.rst` & `tencentcloud-sdk-python-ocr-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1775,14 +1775,16 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeTableAccurateOCR(self, request):
         """本接口支持中英文图片/PDF内常规表格、无线表格、多表格的检测和识别，返回每个单元格的文字内容，支持旋转的表格图片识别，且支持将识别结果保存为 Excel 格式。识别效果比表格识别V2更好，覆盖场景更加广泛，对表格难例场景，如无线表格、嵌套表格（有线表格中包含无线表格）的识别效果均优于表格识别V2。点击[立即体验](https://cloud.tencent.com/product/smart-ocr)。
 
+        默认接口请求频率限制：2次/秒。
+
         :param request: Request instance for RecognizeTableAccurateOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeTableAccurateOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeTableAccurateOCRResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.901/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.900/setup.py` & `tencentcloud-sdk-python-ocr-3.0.901/setup.py`

 * *Files identical despite different names*

