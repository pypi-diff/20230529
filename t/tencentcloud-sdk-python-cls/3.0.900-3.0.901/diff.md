# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.900.tar", last modified: Fri May 26 02:14:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.901.tar", last modified: Mon May 29 02:23:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.900.tar` & `tencentcloud-sdk-python-cls-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)     8559 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   254271 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    67925 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:14:39.000000 tencentcloud-sdk-python-cls-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)     8559 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   254636 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    67925 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:23:38.000000 tencentcloud-sdk-python-cls-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:23:39.000000 tencentcloud-sdk-python-cls-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.900/README.rst` & `tencentcloud-sdk-python-cls-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3643,28 +3643,34 @@
         :type To: int
         :param Query: 查询语句
         :type Query: str
         :param TopicId: 要查询的日志主题ID
         :type TopicId: str
         :param Interval: 时间间隔: 单位ms  限制性条件：(To-From) / interval <= 200
         :type Interval: int
+        :param SyntaxRule: 检索语法规则，默认值为0。
+0：Lucene语法，1：CQL语法。
+详细说明参见<a href="https://cloud.tencent.com/document/product/614/47044#RetrievesConditionalRules" target="_blank">检索条件语法规则</a>
+        :type SyntaxRule: int
         """
         self.From = None
         self.To = None
         self.Query = None
         self.TopicId = None
         self.Interval = None
+        self.SyntaxRule = None
 
 
     def _deserialize(self, params):
         self.From = params.get("From")
         self.To = params.get("To")
         self.Query = params.get("Query")
         self.TopicId = params.get("TopicId")
         self.Interval = params.get("Interval")
+        self.SyntaxRule = params.get("SyntaxRule")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cls-3.0.900/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.901/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.900/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.901/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.900/setup.py` & `tencentcloud-sdk-python-cls-3.0.901/setup.py`

 * *Files identical despite different names*

