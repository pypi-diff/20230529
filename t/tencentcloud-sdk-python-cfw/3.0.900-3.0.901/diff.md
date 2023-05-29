# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.900.tar", last modified: Fri May 26 02:13:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.901.tar", last modified: Mon May 29 02:22:20 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.900.tar` & `tencentcloud-sdk-python-cfw-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    66476 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223027 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:13:34.000000 tencentcloud-sdk-python-cfw-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    66476 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223068 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:22:20.000000 tencentcloud-sdk-python-cfw-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/README.rst` & `tencentcloud-sdk-python-cfw-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/cfw/v20190904/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4157,15 +4157,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param RuleType: 1封禁列表 2 放通列表
         :type RuleType: int
-        :param IOC: IP、Domain二选一，不能同时为空
+        :param IOC: IP、Domain二选一（注：封禁列表，只能填写IP），不能同时为空
         :type IOC: list of IocListData
         :param IocAction: 可选值：delete（删除）、edit（编辑）、add（添加）  其他值无效
         :type IocAction: str
         :param StartTime: 时间格式：yyyy-MM-dd HH:mm:ss，IocAction 为edit或add时必填
         :type StartTime: str
         :param EndTime: 时间格式：yyyy-MM-dd HH:mm:ss，IocAction 为edit或add时必填，必须大于当前时间且大于StartTime
         :type EndTime: str
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.901/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.900/setup.py` & `tencentcloud-sdk-python-cfw-3.0.901/setup.py`

 * *Files identical despite different names*

