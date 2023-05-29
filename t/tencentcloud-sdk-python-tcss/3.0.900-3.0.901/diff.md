# Comparing `tmp/tencentcloud-sdk-python-tcss-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-tcss-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.900.tar", last modified: Fri May 26 02:28:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcss-3.0.901.tar", last modified: Mon May 29 02:37:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcss-3.0.900.tar` & `tencentcloud-sdk-python-tcss-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   316128 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1040213 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:28:38.000000 tencentcloud-sdk-python-tcss-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   316128 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1040497 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:37:43.000000 tencentcloud-sdk-python-tcss-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/README.rst` & `tencentcloud-sdk-python-tcss-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-tcss-3.0.901/tencentcloud/tcss/v20201101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25482,27 +25482,31 @@
         :param EnableRuleCount: 已开启策略数量
         :type EnableRuleCount: int
         :param NetworkPolicyPluginStatus: 集群网络插件状态，正常：Running 不正常：Error
         :type NetworkPolicyPluginStatus: str
         :param NetworkPolicyPluginError: 集群网络插件错误信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type NetworkPolicyPluginError: str
+        :param ClusterNetworkSettings: 容器网络插件
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterNetworkSettings: str
         """
         self.ClusterId = None
         self.ClusterName = None
         self.ClusterVersion = None
         self.ClusterOs = None
         self.ClusterType = None
         self.Region = None
         self.NetworkPolicyPlugin = None
         self.ClusterStatus = None
         self.TotalRuleCount = None
         self.EnableRuleCount = None
         self.NetworkPolicyPluginStatus = None
         self.NetworkPolicyPluginError = None
+        self.ClusterNetworkSettings = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.ClusterVersion = params.get("ClusterVersion")
         self.ClusterOs = params.get("ClusterOs")
@@ -25510,14 +25514,15 @@
         self.Region = params.get("Region")
         self.NetworkPolicyPlugin = params.get("NetworkPolicyPlugin")
         self.ClusterStatus = params.get("ClusterStatus")
         self.TotalRuleCount = params.get("TotalRuleCount")
         self.EnableRuleCount = params.get("EnableRuleCount")
         self.NetworkPolicyPluginStatus = params.get("NetworkPolicyPluginStatus")
         self.NetworkPolicyPluginError = params.get("NetworkPolicyPluginError")
+        self.ClusterNetworkSettings = params.get("ClusterNetworkSettings")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.901/tencentcloud_sdk_python_tcss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-tcss-3.0.901/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcss
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Tcss SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcss-3.0.900/setup.py` & `tencentcloud-sdk-python-tcss-3.0.901/setup.py`

 * *Files identical despite different names*

