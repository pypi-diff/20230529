# Comparing `tmp/ml-management-0.0.32.tar.gz` & `tmp/ml-management-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.32.tar", last modified: Thu May 18 13:07:10 2023, max compression
+gzip compressed data, was "ml-management-0.0.33.tar", last modified: Mon May 29 06:00:27 2023, max compression
```

## Comparing `ml-management-0.0.32.tar` & `ml-management-0.0.33.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.197035 ml-management-0.0.32/
--rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.32/MANIFEST.in
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/
--rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-05-18 07:29:32.000000 ml-management-0.0.32/ML_management/collectors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-05-17 12:25:48.000000 ml-management-0.0.32/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-05-18 06:45:39.000000 ml-management-0.0.32/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      509 2023-05-18 07:27:29.000000 ml-management-0.0.32/ML_management/collectors/collectors.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/dummy/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-05-17 13:22:23.000000 ml-management-0.0.32/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/s3/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10557 2023-05-17 13:22:23.000000 ml-management-0.0.32/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/collectors/topic_markers/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-05-18 08:42:14.000000 ml-management-0.0.32/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/dataset_loader_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-05-17 10:16:44.000000 ml-management-0.0.32/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-18 07:11:26.000000 ml-management-0.0.32/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/executor_template/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/executor_template/default_executors/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-05-17 10:16:44.000000 ml-management-0.0.32/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-05-18 07:11:58.000000 ml-management-0.0.32/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/mlmanagement/
--rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.32/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-11 13:44:22.000000 ml-management-0.0.32/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-11 13:44:22.000000 ml-management-0.0.32/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    11676 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    10262 2023-05-17 08:18:52.000000 ml-management-0.0.32/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/models/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/models/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/models/patterns/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/registry/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.32/ML_management/registry/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-15 06:26:38.000000 ml-management-0.0.32/ML_management/registry/exceptions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-15 06:26:40.000000 ml-management-0.0.32/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/tests/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.32/ML_management/tests/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.32/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     9298 2023-05-16 14:18:14.000000 ml-management-0.0.32/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.193035 ml-management-0.0.32/ML_management/uploader_data/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-16 08:53:37.000000 ml-management-0.0.32/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1582 2023-05-16 08:55:47.000000 ml-management-0.0.32/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-18 13:07:10.197035 ml-management-0.0.32/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.32/README.md
--rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-18 13:07:02.000000 ml-management-0.0.32/VERSION
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-18 13:07:10.197035 ml-management-0.0.32/ml_management.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/requires.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-18 13:07:10.000000 ml-management-0.0.32/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-18 13:07:10.197035 ml-management-0.0.32/setup.cfg
--rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-05-15 06:26:38.000000 ml-management-0.0.32/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-04-17 13:42:26.000000 ml-management-0.0.33/MANIFEST.in
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      509 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/collectors.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/dummy/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/s3/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10557 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/dataset_loader_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/executor_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.795593 ml-management-0.0.33/ML_management/mlmanagement/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      581 2023-04-26 06:58:05.000000 ml-management-0.0.33/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-11 13:44:22.000000 ml-management-0.0.33/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-11 13:44:22.000000 ml-management-0.0.33/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    12327 2023-05-26 08:34:53.000000 ml-management-0.0.33/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10262 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/models/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/models/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/models/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/registry/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2022-10-04 18:14:32.000000 ml-management-0.0.33/ML_management/registry/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-15 06:26:38.000000 ml-management-0.0.33/ML_management/registry/exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-15 06:26:40.000000 ml-management-0.0.33/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/tests/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-04-17 13:42:26.000000 ml-management-0.0.33/ML_management/tests/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-04-17 13:42:26.000000 ml-management-0.0.33/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9298 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ML_management/uploader_data/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1582 2023-05-19 13:53:18.000000 ml-management-0.0.33/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-29 06:00:27.799593 ml-management-0.0.33/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)       56 2022-11-02 13:55:55.000000 ml-management-0.0.33/README.md
+-rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-05-29 06:00:26.000000 ml-management-0.0.33/VERSION
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-29 06:00:27.799593 ml-management-0.0.33/ml_management.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      312 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)      142 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-05-29 06:00:27.000000 ml-management-0.0.33/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-29 06:00:27.799593 ml-management-0.0.33/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1030 2023-05-15 06:26:38.000000 ml-management-0.0.33/setup.py
```

### Comparing `ml-management-0.0.32/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.33/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.33/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.33/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.33/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.33/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.33/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.33/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.33/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.33/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.33/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.33/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.33/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.33/ML_management/mlmanagement/mlmanagement.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,14 +136,34 @@
 
 def log_metric(key: str, value: float, step: Optional[int] = None) -> None:
     """Log a metric under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
+def log_artifact(local_path: str, artifact_path: Optional[str] = None) -> None:
+    """
+    Log a local file or directory as an artifact of the currently active run.
+
+    If no run is active, this method will create a new active run.
+    """
+    start_run_if_not_exist()
+    return request_for_function(inspect.currentframe())
+
+
+def log_artifacts(local_dir: str, artifact_path: Optional[str] = None) -> None:
+    """
+    Log all the contents of a local directory as artifacts of the run.
+
+    If no run is active, this method will create a new active run.
+    """
+    start_run_if_not_exist()
+    return request_for_function(inspect.currentframe())
+
+
 def set_tag(key: str, value: Any) -> None:
     """Set a tag under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
 def autolog(
```

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.33/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.33/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.33/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.33/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.33/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/registry/exceptions.py` & `ml-management-0.0.33/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/registry/registry_manager.py` & `ml-management-0.0.33/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.33/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.33/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.33/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.33/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.32/setup.py` & `ml-management-0.0.33/setup.py`

 * *Files identical despite different names*

