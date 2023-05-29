# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.900.tar", last modified: Fri May 26 02:24:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.901.tar", last modified: Mon May 29 02:33:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.900.tar` & `tencentcloud-sdk-python-oceanus-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)     9176 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112543 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)    23497 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:24:16.000000 tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   113771 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)    23497 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:33:11.000000 tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,36 +740,45 @@
         :type Remark: str
         :param FolderId: 作业名所属文件夹ID，根目录为"root"
         :type FolderId: str
         :param FlinkVersion: 作业运行的Flink版本
         :type FlinkVersion: str
         :param WorkSpaceId: 工作空间 SerialId
         :type WorkSpaceId: str
+        :param Tags: 作业标签
+        :type Tags: list of Tag
         """
         self.Name = None
         self.JobType = None
         self.ClusterType = None
         self.ClusterId = None
         self.CuMem = None
         self.Remark = None
         self.FolderId = None
         self.FlinkVersion = None
         self.WorkSpaceId = None
+        self.Tags = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.JobType = params.get("JobType")
         self.ClusterType = params.get("ClusterType")
         self.ClusterId = params.get("ClusterId")
         self.CuMem = params.get("CuMem")
         self.Remark = params.get("Remark")
         self.FolderId = params.get("FolderId")
         self.FlinkVersion = params.get("FlinkVersion")
         self.WorkSpaceId = params.get("WorkSpaceId")
+        if params.get("Tags") is not None:
+            self.Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2188,14 +2197,17 @@
         :type FlinkVersion: str
         :param WorkSpaceId: 工作空间 SerialId
 注意：此字段可能返回 null，表示取不到有效值。
         :type WorkSpaceId: str
         :param WorkSpaceName: 工作空间名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type WorkSpaceName: str
+        :param Tags: 作业标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tags: list of Tag
         """
         self.JobId = None
         self.Region = None
         self.Zone = None
         self.AppId = None
         self.OwnerUin = None
         self.CreatorUin = None
@@ -2220,14 +2232,15 @@
         self.WebUIUrl = None
         self.SchedulerType = None
         self.ClusterStatus = None
         self.RunningCu = None
         self.FlinkVersion = None
         self.WorkSpaceId = None
         self.WorkSpaceName = None
+        self.Tags = None
 
 
     def _deserialize(self, params):
         self.JobId = params.get("JobId")
         self.Region = params.get("Region")
         self.Zone = params.get("Zone")
         self.AppId = params.get("AppId")
@@ -2254,14 +2267,20 @@
         self.WebUIUrl = params.get("WebUIUrl")
         self.SchedulerType = params.get("SchedulerType")
         self.ClusterStatus = params.get("ClusterStatus")
         self.RunningCu = params.get("RunningCu")
         self.FlinkVersion = params.get("FlinkVersion")
         self.WorkSpaceId = params.get("WorkSpaceId")
         self.WorkSpaceName = params.get("WorkSpaceName")
+        if params.get("Tags") is not None:
+            self.Tags = []
+            for item in params.get("Tags"):
+                obj = Tag()
+                obj._deserialize(item)
+                self.Tags.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3096,30 +3115,40 @@
         :type Remark: str
         :param FileName: 文件名
 注意：此字段可能返回 null，表示取不到有效值。
         :type FileName: str
         :param FolderId: 目录ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type FolderId: str
+        :param RefJobStatusCountSet: 分状态统计关联作业数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RefJobStatusCountSet: list of RefJobStatusCountItem
         """
         self.ResourceId = None
         self.Name = None
         self.ResourceType = None
         self.Remark = None
         self.FileName = None
         self.FolderId = None
+        self.RefJobStatusCountSet = None
 
 
     def _deserialize(self, params):
         self.ResourceId = params.get("ResourceId")
         self.Name = params.get("Name")
         self.ResourceType = params.get("ResourceType")
         self.Remark = params.get("Remark")
         self.FileName = params.get("FileName")
         self.FolderId = params.get("FolderId")
+        if params.get("RefJobStatusCountSet") is not None:
+            self.RefJobStatusCountSet = []
+            for item in params.get("RefJobStatusCountSet"):
+                obj = RefJobStatusCountItem()
+                obj._deserialize(item)
+                self.RefJobStatusCountSet.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.901/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.901/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.900/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.901/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

