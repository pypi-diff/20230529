# Comparing `tmp/backend.ai-storage-proxy-23.3.3.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.3.tar", last modified: Thu May 25 17:30:44 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.4.tar", last modified: Mon May 29 10:42:35 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.3.tar` & `backend.ai-storage-proxy-23.3.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.581146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_quota_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/quotamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.585146 backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:44.589146 backend.ai-storage-proxy-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-25 17:30:44.000000 backend.ai-storage-proxy-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_quota_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/quotamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.3/PKG-INFO` & `backend.ai-storage-proxy-23.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_client.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/dellemc_quota_manager.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_quota_manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/netapp/quotamanager.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/quotamanager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.3/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/backend_shim.py` & `backend.ai-storage-proxy-23.3.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.3/setup.py` & `backend.ai-storage-proxy-23.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,24 @@
         'PyJWT~=2.0',
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'attrs>=20.3',
-        """backend.ai-common==23.03.3
+        """backend.ai-common==23.03.4
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
-        'setproctitle~=1.2.2',
+        'setproctitle~=1.3.2',
         'tenacity>=8.0',
         'trafaret~=2.1',
+        'types-aiofiles',
+        'types-click',
         'uvloop>=0.17; sys_platform != "Windows"',
         'yarl~=1.8.2',
         'zipstream-new~=1.1.8',
     ),
     'license': 'LGPLv3',
     'long_description': """# Backend.AI Storage Proxy
 
@@ -245,11 +247,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.3
+    'version': """23.03.4
 """,
     'zip_safe': False,
 })
```

