# Comparing `tmp/my-provider-0.1.7.tar.gz` & `tmp/my-provider-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/my-provider-0.1.7.tar", last modified: Mon May 29 09:20:13 2023, max compression
+gzip compressed data, was "dist/my-provider-0.1.8.tar", last modified: Mon May 29 09:54:13 2023, max compression
```

## Comparing `my-provider-0.1.7.tar` & `my-provider-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:20:13.000000 my-provider-0.1.7/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:20:13.000000 my-provider-0.1.7/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider/
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my-provider-0.1.7/my_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my-provider-0.1.7/my_provider/operators/dlc_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 09:19:25.000000 my-provider-0.1.7/my_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my-provider-0.1.7/my_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7738 2023-05-26 07:27:32.000000 my-provider-0.1.7/my_provider/hooks/dlc_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 09:20:11.000000 my-provider-0.1.7/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       82 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 09:20:13.000000 my-provider-0.1.7/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 09:20:13.000000 my-provider-0.1.7/setup.cfg
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:54:13.000000 my-provider-0.1.8/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my-provider-0.1.8/my_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my-provider-0.1.8/my_provider/operators/dlc_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 09:19:25.000000 my-provider-0.1.8/my_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my-provider-0.1.8/my_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7858 2023-05-29 09:54:07.000000 my-provider-0.1.8/my_provider/hooks/dlc_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 09:54:07.000000 my-provider-0.1.8/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       82 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 09:54:13.000000 my-provider-0.1.8/setup.cfg
```

### Comparing `my-provider-0.1.7/my_provider/operators/dlc_operator.py` & `my-provider-0.1.8/my_provider/operators/dlc_operator.py`

 * *Files identical despite different names*

### Comparing `my-provider-0.1.7/my_provider/hooks/dlc_hook.py` & `my-provider-0.1.8/my_provider/hooks/dlc_hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         try:
             response = client.CreateTasks(request)
             return set(response.TaskIdSet)
         except TencentCloudSDKException:
             LOG.exception(
                 "Exception while create task"
             )
+            raise
 
     # 检查任务状态
     def check_task_state(self, task_set: set) -> bool:
         client = self.get_conn()
         request = models.DescribeTasksRequest()
         request_filter = models.Filter()
         request_filter.Name = "task-id"
@@ -103,14 +104,15 @@
                         task_set.remove(task.Id)
                         state = False
                         break
             except TencentCloudSDKException:
                 LOG.exception(
                     "Exception while getting task state. Task id: %s", task_set
                 )
+                raise
             time.sleep(2)
         return state
 
     # 取消sql任务
     def cancel_task(self, task_set: set):
         client = self.get_conn()
         request = models.CancelTaskRequest()
@@ -119,14 +121,15 @@
             request.TaskId = task
             try:
                 client.CancelTask(request)
             except TencentCloudSDKException:
                 LOG.exception(
                     "Exception while cancelling query. Task id: %s .", task
                 )
+                raise
 
     # 创建spark 作业任务
     def create_spark_app_task(self, job_name: str, cmd_args: str):
         client = self.get_conn()
         request = models.CreateSparkAppTaskRequest()
         request.JobName = job_name
         request.CmdArgs = cmd_args
@@ -152,14 +155,15 @@
         try:
             response = client.CreateSparkSessionBatchSQL(create_spark_batch_sql_request)
             return response.BatchId
         except TencentCloudSDKException:
             LOG.exception(
                 "Exception while create task"
             )
+            raise
 
     # 检查spark batch sql 任务状态
     def check_spark_batch_sql_task_state(self, batch_id: str) -> bool:
         client = self.get_conn()
         request = models.DescribeSparkSessionBatchSqlLogRequest()
         request.BatchId = batch_id
         state = False
@@ -180,21 +184,23 @@
                     break
                 elif response.State in [BatchSQLTaskSates.EXPIRATION, response.State == BatchSQLTaskSates.INIT]:
                     LOG.info(f"batch id [{batch_id}], logs[{response.LogSet}]")
             except TencentCloudSDKException:
                 LOG.exception(
                     "Exception while getting task state. Batch id: %s", batch_id
                 )
+                raise
             time.sleep(2)
         return state
 
     # 取消spark batch sql任务
     def cancel_spark_batch_sql_task(self, batch_id: str):
         client = self.get_conn()
         request = models.CancelSparkSessionBatchSQLRequest()
         request.BatchId = batch_id
         try:
             client.CreateSparkSessionBatchSQL(request)
         except TencentCloudSDKException:
             LOG.exception(
                 "Exception while cancelling query. Batch id: %s .", batch_id
             )
+            raise
```

