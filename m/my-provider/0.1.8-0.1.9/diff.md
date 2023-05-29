# Comparing `tmp/my-provider-0.1.8.tar.gz` & `tmp/my-provider-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/my-provider-0.1.8.tar", last modified: Mon May 29 09:54:13 2023, max compression
+gzip compressed data, was "dist/my-provider-0.1.9.tar", last modified: Mon May 29 11:34:26 2023, max compression
```

## Comparing `my-provider-0.1.8.tar` & `my-provider-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:54:13.000000 my-provider-0.1.8/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my-provider-0.1.8/my_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my-provider-0.1.8/my_provider/operators/dlc_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 09:19:25.000000 my-provider-0.1.8/my_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my-provider-0.1.8/my_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7858 2023-05-29 09:54:07.000000 my-provider-0.1.8/my_provider/hooks/dlc_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 09:54:07.000000 my-provider-0.1.8/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       82 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 09:54:13.000000 my-provider-0.1.8/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 09:54:13.000000 my-provider-0.1.8/setup.cfg
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 11:34:26.000000 my-provider-0.1.9/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 11:34:26.000000 my-provider-0.1.9/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider/
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my-provider-0.1.9/my_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my-provider-0.1.9/my_provider/operators/dlc_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 09:19:25.000000 my-provider-0.1.9/my_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my-provider-0.1.9/my_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7858 2023-05-29 11:34:23.000000 my-provider-0.1.9/my_provider/hooks/dlc_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 11:34:23.000000 my-provider-0.1.9/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       82 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 11:34:26.000000 my-provider-0.1.9/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 11:34:26.000000 my-provider-0.1.9/setup.cfg
```

### Comparing `my-provider-0.1.8/my_provider/operators/dlc_operator.py` & `my-provider-0.1.9/my_provider/operators/dlc_operator.py`

 * *Files identical despite different names*

### Comparing `my-provider-0.1.8/my_provider/hooks/dlc_hook.py` & `my-provider-0.1.9/my_provider/hooks/dlc_hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,13 +194,13 @@
 
     # 取消spark batch sql任务
     def cancel_spark_batch_sql_task(self, batch_id: str):
         client = self.get_conn()
         request = models.CancelSparkSessionBatchSQLRequest()
         request.BatchId = batch_id
         try:
-            client.CreateSparkSessionBatchSQL(request)
+            client.CancelSparkSessionBatchSQL(request)
         except TencentCloudSDKException:
             LOG.exception(
                 "Exception while cancelling query. Batch id: %s .", batch_id
             )
             raise
```

