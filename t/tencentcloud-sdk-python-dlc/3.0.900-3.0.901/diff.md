# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.900.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.900.tar", last modified: Fri May 26 02:16:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.901.tar", last modified: Mon May 29 02:26:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.900.tar` & `tencentcloud-sdk-python-dlc-3.0.901.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)    78374 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   324571 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 02:16:55.000000 tencentcloud-sdk-python-dlc-3.0.900/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)    81336 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   333828 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-29 02:26:02.000000 tencentcloud-sdk-python-dlc-3.0.901/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/README.rst` & `tencentcloud-sdk-python-dlc-3.0.901/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CancelSparkSessionBatchSQL(self, request):
+        """本接口（CancelSparkSessionBatchSQL）用于取消Spark SQL批任务。
+
+        :param request: Request instance for CancelSparkSessionBatchSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CancelSparkSessionBatchSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelSparkSessionBatchSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CancelSparkSessionBatchSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CancelSparkSessionBatchSQLResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CancelTask(self, request):
         """本接口（CancelTask），用于取消任务执行
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelTaskResponse`
 
@@ -620,14 +643,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateSparkSessionBatchSQL(self, request):
+        """本接口（CreateSparkSessionBatchSQL）用于提交Spark SQL批任务。
+
+        :param request: Request instance for CreateSparkSessionBatchSQL.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkSessionBatchSQLRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkSessionBatchSQLResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateSparkSessionBatchSQL", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateSparkSessionBatchSQLResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateStoreLocation(self, request):
         """该接口（CreateStoreLocation）新增或覆盖计算结果存储位置。
 
         :param request: Request instance for CreateStoreLocation.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateStoreLocationRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateStoreLocationResponse`
 
@@ -1400,14 +1446,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeSparkSessionBatchSqlLog(self, request):
+        """本接口（DescribeSparkSessionBatchSqlLog）用于获取SparkSQL批任务日志
+
+        :param request: Request instance for DescribeSparkSessionBatchSqlLog.
+        :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlLogRequest`
+        :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkSessionBatchSqlLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSparkSessionBatchSqlLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSparkSessionBatchSqlLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeStoreLocation(self, request):
         """查询计算结果存储位置。
 
         :param request: Request instance for DescribeStoreLocation.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeStoreLocationRequest`
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/dlc/v20210125/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,14 +752,55 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CancelSparkSessionBatchSQLRequest(AbstractModel):
+    """CancelSparkSessionBatchSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        """
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CancelSparkSessionBatchSQLResponse(AbstractModel):
+    """CancelSparkSessionBatchSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CancelTaskRequest(AbstractModel):
     """CancelTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2062,14 +2103,100 @@
 
     def _deserialize(self, params):
         self.BatchId = params.get("BatchId")
         self.TaskId = params.get("TaskId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateSparkSessionBatchSQLRequest(AbstractModel):
+    """CreateSparkSessionBatchSQL请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DataEngineName: DLC Spark作业引擎名称
+        :type DataEngineName: str
+        :param ExecuteSQL: 运行sql
+        :type ExecuteSQL: str
+        :param DriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
+        :type DriverSize: str
+        :param ExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
+        :type ExecutorSize: str
+        :param ExecutorNumbers: 指定的Executor数量，默认为1
+        :type ExecutorNumbers: int
+        :param ExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于ExecutorNumbers
+        :type ExecutorMaxNumbers: int
+        :param TimeoutInSecond: 指定的Session超时时间，单位秒，默认3600秒
+        :type TimeoutInSecond: int
+        :param SessionId: Session唯一标识，当指定sessionid，则使用该session运行任务。
+        :type SessionId: str
+        :param SessionName: 指定要创建的session名称
+        :type SessionName: str
+        :param Arguments: Session相关配置，当前支持：dlc.eni、dlc.role.arn、dlc.sql.set.config以及用户指定的配置，注：roleArn必填；
+        :type Arguments: list of KVPair
+        """
+        self.DataEngineName = None
+        self.ExecuteSQL = None
+        self.DriverSize = None
+        self.ExecutorSize = None
+        self.ExecutorNumbers = None
+        self.ExecutorMaxNumbers = None
+        self.TimeoutInSecond = None
+        self.SessionId = None
+        self.SessionName = None
+        self.Arguments = None
+
+
+    def _deserialize(self, params):
+        self.DataEngineName = params.get("DataEngineName")
+        self.ExecuteSQL = params.get("ExecuteSQL")
+        self.DriverSize = params.get("DriverSize")
+        self.ExecutorSize = params.get("ExecutorSize")
+        self.ExecutorNumbers = params.get("ExecutorNumbers")
+        self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        self.TimeoutInSecond = params.get("TimeoutInSecond")
+        self.SessionId = params.get("SessionId")
+        self.SessionName = params.get("SessionName")
+        if params.get("Arguments") is not None:
+            self.Arguments = []
+            for item in params.get("Arguments"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Arguments.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateSparkSessionBatchSQLResponse(AbstractModel):
+    """CreateSparkSessionBatchSQL返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: 批任务唯一标识
+        :type BatchId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.BatchId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateStoreLocationRequest(AbstractModel):
     """CreateStoreLocation请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5127,14 +5254,69 @@
             for item in params.get("SparkAppTasks"):
                 obj = TaskResponseInfo()
                 obj._deserialize(item)
                 self.SparkAppTasks.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeSparkSessionBatchSqlLogRequest(AbstractModel):
+    """DescribeSparkSessionBatchSqlLog请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BatchId: SparkSQL唯一标识
+        :type BatchId: str
+        """
+        self.BatchId = None
+
+
+    def _deserialize(self, params):
+        self.BatchId = params.get("BatchId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSparkSessionBatchSqlLogResponse(AbstractModel):
+    """DescribeSparkSessionBatchSqlLog返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param State: 状态：0：初始化、1：成功、2：失败、3：取消、4：异常；
+        :type State: int
+        :param LogSet: 日志信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogSet: list of SparkSessionBatchLog
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.State = None
+        self.LogSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.State = params.get("State")
+        if params.get("LogSet") is not None:
+            self.LogSet = []
+            for item in params.get("LogSet"):
+                obj = SparkSessionBatchLog()
+                obj._deserialize(item)
+                self.LogSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeStoreLocationRequest(AbstractModel):
     """DescribeStoreLocation请求参数结构体
 
     """
 
 
 class DescribeStoreLocationResponse(AbstractModel):
@@ -7610,14 +7792,99 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SparkSessionBatchLog(AbstractModel):
+    """SparkSQL批任务运行日志
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Step: 日志步骤：BEG/CS/DS/DSS/DSF/FINF/RTO/CANCEL/CT/DT/DTS/DTF/FINT/EXCE
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Step: str
+        :param Time: 时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Time: str
+        :param Message: 日志提示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param Operate: 日志操作
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operate: list of SparkSessionBatchLogOperate
+        """
+        self.Step = None
+        self.Time = None
+        self.Message = None
+        self.Operate = None
+
+
+    def _deserialize(self, params):
+        self.Step = params.get("Step")
+        self.Time = params.get("Time")
+        self.Message = params.get("Message")
+        if params.get("Operate") is not None:
+            self.Operate = []
+            for item in params.get("Operate"):
+                obj = SparkSessionBatchLogOperate()
+                obj._deserialize(item)
+                self.Operate.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SparkSessionBatchLogOperate(AbstractModel):
+    """SparkSQL批任务日志操作信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Text: 操作提示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Text: str
+        :param Operate: 操作类型：COPY、LOG、UI、RESULT、List、TAB
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Operate: str
+        :param Supplement: 补充信息：如：taskid、sessionid、sparkui等
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Supplement: list of KVPair
+        """
+        self.Text = None
+        self.Operate = None
+        self.Supplement = None
+
+
+    def _deserialize(self, params):
+        self.Text = params.get("Text")
+        self.Operate = params.get("Operate")
+        if params.get("Supplement") is not None:
+            self.Supplement = []
+            for item in params.get("Supplement"):
+                obj = KVPair()
+                obj._deserialize(item)
+                self.Supplement.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class StatementOutput(AbstractModel):
     """notebook session statement输出信息。
 
     """
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.901/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.901/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/setup.py` & `tencentcloud-sdk-python-dlc-3.0.901/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.900/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.901/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.900
+Version: 3.0.901
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

