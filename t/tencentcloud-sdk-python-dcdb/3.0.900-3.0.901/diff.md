# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.900.tar", last modified: Fri May 26 02:16:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.901.tar", last modified: Mon May 29 02:25:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.900.tar` & `tencentcloud-sdk-python-dcdb-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13507 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   235272 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    68182 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-26 02:16:47.000000 tencentcloud-sdk-python-dcdb-3.0.900/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:16:48.000000 tencentcloud-sdk-python-dcdb-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13609 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   238676 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    69104 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:25:55.000000 tencentcloud-sdk-python-dcdb-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,17 @@
 
 # 当前部署方式不允许设置此同步模式。
 INVALIDPARAMETERVALUE_SYNCMODENOTALLOWED = 'InvalidParameterValue.SyncModeNotAllowed'
 
 # 请求过于频繁。
 LIMITEXCEEDED_TOOFREQUENTLYCALLED = 'LimitExceeded.TooFrequentlyCalled'
 
+# 临时实例已经存在了。
+RESOURCEINUSE_TEMPINSTANCEEXIST = 'ResourceInUse.TempInstanceExist'
+
 # 资源不足。
 RESOURCEINSUFFICIENT = 'ResourceInsufficient'
 
 # 指定的账号不存在。
 RESOURCENOTFOUND_ACCOUNTDOESNOTEXIST = 'ResourceNotFound.AccountDoesNotExist'
 
 # 实例不存在。
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,25 +623,25 @@
         :type AutoVoucher: bool
         :param VoucherIds: 代金券ID列表，目前仅支持指定一张代金券。
         :type VoucherIds: list of str
         :param SecurityGroupId: 安全组id
         :type SecurityGroupId: str
         :param InstanceName: 实例名称， 可以通过该字段自主的设置实例的名字
         :type InstanceName: str
-        :param Ipv6Flag: 是否支持IPv6
+        :param Ipv6Flag: 是否支持IPv6，0:不支持，1:支持
         :type Ipv6Flag: int
         :param ResourceTags: 标签键值对数组
         :type ResourceTags: list of ResourceTag
         :param InitParams: 参数列表。本接口的可选值为：character_set_server（字符集，必传），lower_case_table_names（表名大小写敏感，必传，0 - 敏感；1-不敏感），innodb_page_size（innodb数据页，默认16K），sync_mode（同步模式：0 - 异步； 1 - 强同步；2 - 强同步可退化。默认为强同步可退化）。
         :type InitParams: list of DBParamValue
         :param DcnRegion: DCN源地域
         :type DcnRegion: str
         :param DcnInstanceId: DCN源实例ID
         :type DcnInstanceId: str
-        :param AutoRenewFlag: 自动续费标记，0表示默认状态(用户未设置，即初始状态即手动续费，用户开通了预付费不停服特权也会进行自动续费)， 1表示自动续费，2表示明确不自动续费(用户设置)，若业务无续费概念或无需自动续费，需要设置为0
+        :param AutoRenewFlag: 自动续费标记，0:默认状态(用户未设置，即初始状态即手动续费，用户开通了预付费不停服特权也会进行自动续费)， 1:自动续费，2:明确不自动续费(用户设置)。若业务无续费概念或无需自动续费，需要设置为0
         :type AutoRenewFlag: int
         :param SecurityGroupIds: 安全组ids，安全组可以传数组形式，兼容之前SecurityGroupId参数
         :type SecurityGroupIds: list of str
         """
         self.Zones = None
         self.Period = None
         self.ShardMemory = None
@@ -927,27 +927,27 @@
         :type DbVersionId: str
         :param Zones: 分片节点可用区分布，最多可填两个可用区。当分片规格为一主两从时，其中两个节点在第一个可用区。
         :type Zones: list of str
         :param SecurityGroupId: 安全组id
         :type SecurityGroupId: str
         :param InstanceName: 实例名称， 可以通过该字段自主的设置实例的名字
         :type InstanceName: str
-        :param Ipv6Flag: 是否支持IPv6
+        :param Ipv6Flag: 是否支持IPv6，0:不支持，1:支持
         :type Ipv6Flag: int
         :param ResourceTags: 标签键值对数组
         :type ResourceTags: list of ResourceTag
         :param DcnRegion: DCN源地域
         :type DcnRegion: str
         :param DcnInstanceId: DCN源实例ID
         :type DcnInstanceId: str
         :param InitParams: 参数列表。本接口的可选值为：character_set_server（字符集，必传），lower_case_table_names（表名大小写敏感，必传，0 - 敏感；1-不敏感），innodb_page_size（innodb数据页，默认16K），sync_mode（同步模式：0 - 异步； 1 - 强同步；2 - 强同步可退化。默认为强同步可退化）。
         :type InitParams: list of DBParamValue
         :param RollbackInstanceId: 需要回档的源实例ID
         :type RollbackInstanceId: str
-        :param RollbackTime: 回档时间
+        :param RollbackTime: 回档时间，例如“2021-11-22 00:00:00”
         :type RollbackTime: str
         :param SecurityGroupIds: 安全组ids，安全组可以传数组形式，兼容之前SecurityGroupId参数
         :type SecurityGroupIds: list of str
         """
         self.ShardMemory = None
         self.ShardStorage = None
         self.ShardNodeCount = None
@@ -1038,14 +1038,63 @@
     def _deserialize(self, params):
         self.InstanceIds = params.get("InstanceIds")
         self.FlowId = params.get("FlowId")
         self.DealName = params.get("DealName")
         self.RequestId = params.get("RequestId")
 
 
+class CreateTmpDCDBInstanceRequest(AbstractModel):
+    """CreateTmpDCDBInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 回档实例的ID
+        :type InstanceId: str
+        :param RollbackTime: 回档时间点
+        :type RollbackTime: str
+        """
+        self.InstanceId = None
+        self.RollbackTime = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.RollbackTime = params.get("RollbackTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateTmpDCDBInstanceResponse(AbstractModel):
+    """CreateTmpDCDBInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 任务流ID
+        :type FlowId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.RequestId = params.get("RequestId")
+
+
 class DBAccount(AbstractModel):
     """云数据库账号信息
 
     """
 
     def __init__(self):
         r"""
@@ -1062,34 +1111,38 @@
         :param ReadOnly: 只读标记，0：否， 1：该账号的sql请求优先选择备机执行，备机不可用时选择主机执行，2：优先选择备机执行，备机不可用时操作失败。
         :type ReadOnly: int
         :param DelayThresh: 如果备机延迟超过本参数设置值，系统将认为备机发生故障
 建议该参数值大于10。当ReadOnly选择1、2时该参数生效。
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
         
@@ -2600,14 +2653,16 @@
         :type EncryptStatus: int
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
@@ -2653,14 +2708,15 @@
         self.DcnDstNum = None
         self.InstanceType = None
         self.IsMaxUserConnectionsSupported = None
         self.DbVersionId = None
         self.EncryptStatus = None
         self.ExclusterType = None
         self.RsAccessStrategy = None
+        self.ReservedNetResources = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.Status = params.get("Status")
@@ -2717,14 +2773,20 @@
         self.DcnDstNum = params.get("DcnDstNum")
         self.InstanceType = params.get("InstanceType")
         self.IsMaxUserConnectionsSupported = params.get("IsMaxUserConnectionsSupported")
         self.DbVersionId = params.get("DbVersionId")
         self.EncryptStatus = params.get("EncryptStatus")
         self.ExclusterType = params.get("ExclusterType")
         self.RsAccessStrategy = params.get("RsAccessStrategy")
+        if params.get("ReservedNetResources") is not None:
+            self.ReservedNetResources = []
+            for item in params.get("ReservedNetResources"):
+                obj = ReservedNetResource()
+                obj._deserialize(item)
+                self.ReservedNetResources.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DescribeDCDBInstanceNodeInfoRequest(AbstractModel):
     """DescribeDCDBInstanceNodeInfo请求参数结构体
 
     """
@@ -4419,15 +4481,15 @@
 class IsolateHourDCDBInstanceRequest(AbstractModel):
     """IsolateHourDCDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceIds: 实例uuid列表
+        :param InstanceIds: 待升级的实例ID列表。形如：["dcdbt-ow728lmc"]，可以通过 DescribeDCDBInstances 查询实例详情获得。
         :type InstanceIds: list of str
         """
         self.InstanceIds = None
 
 
     def _deserialize(self, params):
         self.InstanceIds = params.get("InstanceIds")
@@ -5586,14 +5648,54 @@
 
 
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
+        :param RecycleTime: Vip的回收时间	
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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class DcdbClient(AbstractClient):
     _apiVersion = '2018-04-11'
     _endpoint = 'dcdb.tencentcloudapi.com'
     _service = 'dcdb'
 
 
     def ActiveHourDCDBInstance(self, request):
-        """解隔离DCDB后付费实例
+        """解隔离TDSQL按量计费实例
 
         :param request: Request instance for ActiveHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ActiveHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.ActiveHourDCDBInstanceResponse`
 
         """
         try:
@@ -185,15 +185,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDCDBInstance(self, request):
-        """本接口（CreateDCDBInstance）用于创建包年包月的云数据库实例，可通过传入实例规格、数据库版本号、购买时长等信息创建云数据库实例。
+        """本接口（CreateDCDBInstance）用于创建包年包月的TDSQL实例，可通过传入实例规格、数据库版本号、购买时长等信息创建云数据库实例。
 
         :param request: Request instance for CreateDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateDCDBInstanceResponse`
 
         """
         try:
@@ -208,15 +208,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDedicatedClusterDCDBInstance(self, request):
-        """创建独享集群DCDB实例
+        """创建TDSQL独享集群实例
 
         :param request: Request instance for CreateDedicatedClusterDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateDedicatedClusterDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateDedicatedClusterDCDBInstanceResponse`
 
         """
         try:
@@ -231,15 +231,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateHourDCDBInstance(self, request):
-        """创建DCDB后付费实例
+        """创建TDSQL按量计费实例
 
         :param request: Request instance for CreateHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateHourDCDBInstanceResponse`
 
         """
         try:
@@ -253,14 +253,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateTmpDCDBInstance(self, request):
+        """回档TDSQL实例
+
+        :param request: Request instance for CreateTmpDCDBInstance.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateTmpDCDBInstanceRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateTmpDCDBInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateTmpDCDBInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateTmpDCDBInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteAccount(self, request):
         """本接口（DeleteAccount）用于删除云数据库账号。用户名+host唯一确定一个账号。
 
         :param request: Request instance for DeleteAccount.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DeleteAccountRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DeleteAccountResponse`
 
@@ -485,15 +508,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDCDBInstanceDetail(self, request):
-        """本接口（DescribeDCDBInstanceDetail）用于获取DCDB实例详情
+        """本接口（DescribeDCDBInstanceDetail）用于获取TDSQL实例详情
 
         :param request: Request instance for DescribeDCDBInstanceDetail.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBInstanceDetailRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DescribeDCDBInstanceDetailResponse`
 
         """
         try:
@@ -948,15 +971,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DestroyDCDBInstance(self, request):
-        """本接口(DestroyDCDBInstance)用于销毁已隔离的包年包月实例。
+        """本接口(DestroyDCDBInstance)用于销毁已隔离的TDSQL包年包月实例。
 
         :param request: Request instance for DestroyDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DestroyDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DestroyDCDBInstanceResponse`
 
         """
         try:
@@ -971,15 +994,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DestroyHourDCDBInstance(self, request):
-        """本接口（DestroyHourDCDBInstance）用于销毁按量计费实例。
+        """本接口（DestroyHourDCDBInstance）用于TDSQL销毁按量计费实例。
 
         :param request: Request instance for DestroyHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DestroyHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DestroyHourDCDBInstanceResponse`
 
         """
         try:
@@ -1110,15 +1133,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def IsolateHourDCDBInstance(self, request):
-        """隔离DCDB后付费实例
+        """隔离TDSQL按量计费实例
 
         :param request: Request instance for IsolateHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.IsolateHourDCDBInstanceResponse`
 
         """
         try:
@@ -1582,15 +1605,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpgradeDedicatedDCDBInstance(self, request):
-        """本接口（UpgradeDedicatedDCDBInstance）用于升级独享DCDB实例
+        """本接口（UpgradeDedicatedDCDBInstance）用于升级TDSQL独享集群实例
 
         :param request: Request instance for UpgradeDedicatedDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDedicatedDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDedicatedDCDBInstanceResponse`
 
         """
         try:
@@ -1605,15 +1628,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpgradeHourDCDBInstance(self, request):
-        """本接口（UpgradeHourDCDBInstance）用于升级后付费分布式数据库实例。
+        """本接口（UpgradeHourDCDBInstance）用于升级分布式数据库TDSQL按量计费实例。
 
         :param request: Request instance for UpgradeHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.UpgradeHourDCDBInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.900/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.901/setup.py`

 * *Files identical despite different names*

