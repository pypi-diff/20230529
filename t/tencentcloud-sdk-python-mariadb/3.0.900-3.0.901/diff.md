# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.900.tar", last modified: Fri May 26 02:22:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.901.tar", last modified: Mon May 29 02:31:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.900.tar` & `tencentcloud-sdk-python-mariadb-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)    70751 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)    14808 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   216004 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:22:41.000000 tencentcloud-sdk-python-mariadb-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    70802 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14808 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   217944 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:31:38.000000 tencentcloud-sdk-python-mariadb-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class MariadbClient(AbstractClient):
     _apiVersion = '2017-03-12'
     _endpoint = 'mariadb.tencentcloudapi.com'
     _service = 'mariadb'
 
 
     def ActivateHourDBInstance(self, request):
-        """解隔离后付费实例
+        """解隔离MariaDB按量计费实例
 
         :param request: Request instance for ActivateHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.ActivateHourDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.ActivateHourDBInstanceResponse`
 
         """
         try:
@@ -185,15 +185,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDBInstance(self, request):
-        """本接口（CreateDBInstance）用于创建包年包月的云数据库实例，可通过传入实例规格、数据库版本号、购买时长和数量等信息创建云数据库实例。
+        """本接口（CreateDBInstance）用于创建包年包月的MariaDB云数据库实例，可通过传入实例规格、数据库版本号、购买时长和数量等信息创建云数据库实例。
 
         :param request: Request instance for CreateDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.CreateDBInstanceResponse`
 
         """
         try:
@@ -208,15 +208,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDedicatedClusterDBInstance(self, request):
-        """创建独享集群Mariadb实例
+        """创建Mariadb独享集群实例
 
         :param request: Request instance for CreateDedicatedClusterDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateDedicatedClusterDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.CreateDedicatedClusterDBInstanceResponse`
 
         """
         try:
@@ -231,15 +231,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateHourDBInstance(self, request):
-        """创建后付费实例
+        """创建MariaDB按量计费实例
 
         :param request: Request instance for CreateHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.CreateHourDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.CreateHourDBInstanceResponse`
 
         """
         try:
@@ -923,15 +923,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DestroyHourDBInstance(self, request):
-        """本接口（DestroyHourDBInstance）用于销毁按量计费实例。
+        """本接口（DestroyHourDBInstance）用于销毁MariaDB按量计费实例。
 
         :param request: Request instance for DestroyHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DestroyHourDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.DestroyHourDBInstanceResponse`
 
         """
         try:
@@ -1039,15 +1039,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def IsolateDBInstance(self, request):
-        """本接口(IsolateDBInstance)用于隔离云数据库实例（包年包月），隔离后不能通过IP和端口访问数据库。隔离的实例可在回收站中进行开机。若为欠费隔离，请尽快进行充值。
+        """本接口(IsolateDBInstance)用于隔离云数据库MariaDB实例（包年包月），隔离后不能通过IP和端口访问数据库。隔离的实例可在回收站中进行开机。若为欠费隔离，请尽快进行充值。
 
         :param request: Request instance for IsolateDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.IsolateDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.IsolateDBInstanceResponse`
 
         """
         try:
@@ -1085,15 +1085,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def IsolateHourDBInstance(self, request):
-        """隔离后付费实例
+        """隔离MariaDB按量计费实例
 
         :param request: Request instance for IsolateHourDBInstance.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.IsolateHourDBInstanceRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.IsolateHourDBInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.901/tencentcloud/mariadb/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
         :type DbVersionId: str
         :param InstanceName: 实例名称， 可以通过该字段自主的设置实例的名字
         :type InstanceName: str
         :param SecurityGroupIds: 安全组ID列表
         :type SecurityGroupIds: list of str
         :param AutoRenewFlag: 自动续费标志，1:自动续费，2:不自动续费
         :type AutoRenewFlag: int
-        :param Ipv6Flag: 是否支持IPv6
+        :param Ipv6Flag: 是否支持IPv6，0:不支持，1:支持
         :type Ipv6Flag: int
         :param ResourceTags: 标签键值对数组
         :type ResourceTags: list of ResourceTag
         :param InitParams: 参数列表。本接口的可选值为：character_set_server（字符集，必传），lower_case_table_names（表名大小写敏感，必传，0 - 敏感；1-不敏感），innodb_page_size（innodb数据页，默认16K），sync_mode（同步模式：0 - 异步； 1 - 强同步；2 - 强同步可退化。默认为强同步可退化）。
         :type InitParams: list of DBParamValue
         :param DcnRegion: DCN源地域
         :type DcnRegion: str
@@ -841,27 +841,27 @@
         :type SubnetId: str
         :param DbVersionId: 数据库引擎版本，当前可选：8.0，5.7，10.1，10.0。
         :type DbVersionId: str
         :param InstanceName: 自定义实例名称
         :type InstanceName: str
         :param SecurityGroupIds: 安全组ID，不传表示不绑定安全组
         :type SecurityGroupIds: list of str
-        :param Ipv6Flag: 是否支持IPv6
+        :param Ipv6Flag: 是否支持IPv6，0:不支持，1:支持
         :type Ipv6Flag: int
         :param ResourceTags: 标签键值对数组
         :type ResourceTags: list of ResourceTag
         :param DcnRegion: DCN源地域
         :type DcnRegion: str
         :param DcnInstanceId: DCN源实例ID
         :type DcnInstanceId: str
         :param InitParams: 参数列表。本接口的可选值为：
 character_set_server（字符集，必传），lower_case_table_names（表名大小写敏感，必传，0 - 敏感；1-不敏感），
 innodb_page_size（innodb数据页，默认16K），sync_mode（同步模式：0 - 异步； 1 - 强同步；2 - 强同步可退化，默认为强同步可退化）。
         :type InitParams: list of DBParamValue
-        :param RollbackInstanceId: 回档源实例ID
+        :param RollbackInstanceId: 回档源实例ID，例如“2021-11-22 00:00:00”
         :type RollbackInstanceId: str
         :param RollbackTime: 回档时间
         :type RollbackTime: str
         """
         self.Zones = None
         self.NodeCount = None
         self.Memory = None
@@ -1021,34 +1021,38 @@
         :param ReadOnly: 只读标记，0：否， 1：该账号的sql请求优先选择备机执行，备机不可用时选择主机执行，2：优先选择备机执行，备机不可用时操作失败。
         :type ReadOnly: int
         :param DelayThresh: 该字段对只读帐号有意义，表示选择主备延迟小于该值的备机
 注意：此字段可能返回 null，表示取不到有效值。
         :type DelayThresh: int
         :param SlaveConst: 针对只读账号，设置策略是否固定备机，0：不固定备机，即备机不满足条件与客户端不断开连接，Proxy选择其他可用备机，1：备机不满足条件断开连接，确保一个连接固定备机。
         :type SlaveConst: int
+        :param MaxUserConnections: 用户最大连接数，0代表无限制
+        :type MaxUserConnections: int
         """
         self.UserName = None
         self.Host = None
         self.Description = None
         self.CreateTime = None
         self.UpdateTime = None
         self.ReadOnly = None
         self.DelayThresh = None
         self.SlaveConst = None
+        self.MaxUserConnections = None
 
 
     def _deserialize(self, params):
         self.UserName = params.get("UserName")
         self.Host = params.get("Host")
         self.Description = params.get("Description")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         self.ReadOnly = params.get("ReadOnly")
         self.DelayThresh = params.get("DelayThresh")
         self.SlaveConst = params.get("SlaveConst")
+        self.MaxUserConnections = params.get("MaxUserConnections")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2265,14 +2269,16 @@
         :type ReplicaStatus: :class:`tencentcloud.mariadb.v20170312.models.DCNReplicaStatus`
         :param ExclusterType: 独享集群类型，0:公有云, 1:金融围笼, 2:CDC集群
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExclusterType: int
         :param RsAccessStrategy: VPC就近访问
 注意：此字段可能返回 null，表示取不到有效值。
         :type RsAccessStrategy: int
+        :param ReservedNetResources: 尚未回收的网络资源
+        :type ReservedNetResources: list of ReservedNetResource
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceId = None
         self.InstanceName = None
         self.Status = None
         self.StatusDesc = None
@@ -2323,14 +2329,15 @@
         self.IsMaxUserConnectionsSupported = None
         self.DbVersionId = None
         self.EncryptStatus = None
         self.ReplicaConfig = None
         self.ReplicaStatus = None
         self.ExclusterType = None
         self.RsAccessStrategy = None
+        self.ReservedNetResources = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Status = params.get("Status")
@@ -2396,14 +2403,20 @@
             self.ReplicaConfig = DCNReplicaConfig()
             self.ReplicaConfig._deserialize(params.get("ReplicaConfig"))
         if params.get("ReplicaStatus") is not None:
             self.ReplicaStatus = DCNReplicaStatus()
             self.ReplicaStatus._deserialize(params.get("ReplicaStatus"))
         self.ExclusterType = params.get("ExclusterType")
         self.RsAccessStrategy = params.get("RsAccessStrategy")
+        if params.get("ReservedNetResources") is not None:
+            self.ReservedNetResources = []
+            for item in params.get("ReservedNetResources"):
+                obj = ReservedNetResource()
+                obj._deserialize(item)
+                self.ReservedNetResources.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribeDBInstanceSpecsRequest(AbstractModel):
     """DescribeDBInstanceSpecs请求参数结构体
 
     """
@@ -5525,14 +5538,54 @@
 
 
     def _deserialize(self, params):
         self.DealName = params.get("DealName")
         self.RequestId = params.get("RequestId")
 
 
+class ReservedNetResource(AbstractModel):
+    """保留的网络资源信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VpcId: 私有网络
+        :type VpcId: str
+        :param SubnetId: 子网
+        :type SubnetId: str
+        :param Vip: VpcId,SubnetId下保留的内网ip
+        :type Vip: str
+        :param Vports: Vip下的端口
+        :type Vports: list of int
+        :param RecycleTime: vip的回收时间
+        :type RecycleTime: str
+        """
+        self.VpcId = None
+        self.SubnetId = None
+        self.Vip = None
+        self.Vports = None
+        self.RecycleTime = None
+
+
+    def _deserialize(self, params):
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.Vip = params.get("Vip")
+        self.Vports = params.get("Vports")
+        self.RecycleTime = params.get("RecycleTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ResetAccountPasswordRequest(AbstractModel):
     """ResetAccountPassword请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.901/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.900/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.901/setup.py`

 * *Files identical despite different names*

