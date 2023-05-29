# Comparing `tmp/clickzetta-connector-0.7.6.tar.gz` & `tmp/clickzetta-connector-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.7.6.tar", last modified: Mon May 29 03:47:40 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.7.7.tar", last modified: Mon May 29 06:31:09 2023, max compression
```

## Comparing `clickzetta-connector-0.7.6.tar` & `clickzetta-connector-0.7.7.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.081292 clickzetta-connector-0.7.6/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 03:47:40.081159 clickzetta-connector-0.7.6/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.068578 clickzetta-connector-0.7.6/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.069153 clickzetta-connector-0.7.6/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    38181 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.6/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.070149 clickzetta-connector-0.7.6/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4100 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.066310 clickzetta-connector-0.7.6/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.077091 clickzetta-connector-0.7.6/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 03:47:39.000000 clickzetta-connector-0.7.6/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.080428 clickzetta-connector-0.7.6/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8775 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.6/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 03:47:33.000000 clickzetta-connector-0.7.6/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 03:47:40.080991 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      630 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 03:47:40.000000 clickzetta-connector-0.7.6/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 03:47:40.081331 clickzetta-connector-0.7.6/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2880 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.6/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699878 clickzetta-connector-0.7.7/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 06:31:09.699737 clickzetta-connector-0.7.7/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.686217 clickzetta-connector-0.7.7/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.686923 clickzetta-connector-0.7.7/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    38181 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.7/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.687813 clickzetta-connector-0.7.7/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4544 2023-05-29 06:30:58.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.683874 clickzetta-connector-0.7.7/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.695682 clickzetta-connector-0.7.7/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699037 clickzetta-connector-0.7.7/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8775 2023-05-29 03:46:45.000000 clickzetta-connector-0.7.7/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.7.7/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-29 06:30:58.000000 clickzetta-connector-0.7.7/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-29 06:31:09.699581 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      646 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-29 06:31:09.000000 clickzetta-connector-0.7.7/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-29 06:31:09.699925 clickzetta-connector-0.7.7/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2906 2023-05-29 06:12:31.000000 clickzetta-connector-0.7.7/setup.py
```

### Comparing `clickzetta-connector-0.7.6/clickzetta/_helpers.py` & `clickzetta-connector-0.7.7/clickzetta/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_stream.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.7.7/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/client.py` & `clickzetta-connector-0.7.7/clickzetta/client.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/cursor.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/cursor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Cursor for ClickZetta DB-API."""
 
 import collections
 from collections import abc as collections_abc
 import copy
 import logging
+import sqlparse
 import re
 from datetime import datetime
 
 from clickzetta.enums import *
 from clickzetta.table import EmptyRowIterator
 from clickzetta.query_result import QueryResult
 
@@ -57,45 +58,57 @@
                 precision=field.precision,
                 scale=field.scale,
                 null_ok=field.nullable,
             )
             for field in query_result.schema
         )
 
+    def _parse_dml_or_ddl_from_sql(self, sql: str):
+        format_sql = sqlparse.parse(sql)
+        dml_or_ddl = ""
+        # TODO(hanmiao.li): multi sql is not supported yet.
+        for token in format_sql[0].tokens:
+            if token.ttype == sqlparse.tokens.DDL or token.ttype == sqlparse.tokens.DML:
+                dml_or_ddl = token.value.upper()
+                break
+        return dml_or_ddl
+
     def execute(self, operation: str, parameters=None):
 
         self._execute(operation, parameters)
 
     def _execute(
             self, operation: str, parameters
     ):
+        if operation is None or operation == "":
+            raise ValueError("sql is empty")
         self._query_data = None
         self._query_job = None
         client = self.connection._client
         if not operation.endswith(';'):
             operation = operation + ';'
-        operation_upper = operation.upper().strip()
+        operation_upper = self._parse_dml_or_ddl_from_sql(operation)
 
-        if operation_upper.startswith('SELECT') or operation_upper.startswith("SET"):
+        if operation_upper == 'SELECT' or operation_upper == "SET":
             self._query_result = client.select_table(client.token, operation, parameters)
-        elif operation_upper.startswith("DROP"):
+        elif operation_upper == "DROP":
             self._query_result = client.drop_table(client.token, operation)
-        elif operation_upper.startswith("CREATE"):
+        elif operation_upper == "CREATE":
             self._query_result = client.create_table(client.token, operation)
-        elif operation_upper.startswith('ALTER'):
+        elif operation_upper == 'ALTER':
             self._query_result = client.alter_table(client.token, operation)
-        elif operation_upper.startswith("TRUNCATE"):
+        elif operation_upper == "TRUNCATE":
             self._query_result = client.truncate_table(client.token, operation)
-        elif operation_upper.startswith('SHOW'):
+        elif operation_upper == 'SHOW':
             self._query_result = client.show_table(client.token, operation)
-        elif operation_upper.startswith('INSERT'):
+        elif operation_upper == 'INSERT':
             self._query_result = client.insert_table(client.token, operation)
-        elif operation_upper.startswith('UPDATE'):
+        elif operation_upper == 'UPDATE':
             self._query_result = client.update_table(client.token, operation)
-        elif operation_upper.startswith('DESC'):
+        elif operation_upper == 'DESC':
             self._query_result = client.desc_table(client.token, operation)
         else:
             self._query_result = client.execute_other_sql(client.token, operation)
         self._set_rowcount(self._query_result)
         self._query_data = self._query_result.data
         self._set_description(self._query_result)
```

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/dbapi/types.py` & `clickzetta-connector-0.7.7/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/enums.py` & `clickzetta-connector-0.7.7/clickzetta/enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.7.7/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/ingestion.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.7.7/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/query_result.py` & `clickzetta-connector-0.7.7/clickzetta/query_result.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/schema.py` & `clickzetta-connector-0.7.7/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/session.py` & `clickzetta-connector-0.7.7/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/standard_sql.py` & `clickzetta-connector-0.7.7/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta/table.py` & `clickzetta-connector-0.7.7/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.7.7/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.7.6/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.7.7/clickzetta_connector.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 packaging<24.0.0dev,>=14.3
 protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 python-dateutil<3.0dev,>=2.7.2
 requests<3.0.0dev,>=2.21.0
 pyarrow>=11.0.0
 sqlalchemy==2.0.6
 ossfs>=2023.1.0
+sqlparse>=0.4.1
 
 [all]
 pandas>=1.0.0
 db-dtypes<2.0.0dev,>=0.3.0
 ipywidgets==7.7.1
 geopandas<1.0dev,>=0.9.0
 Shapely<2.0dev,>=1.6.0
```

### Comparing `clickzetta-connector-0.7.6/setup.py` & `clickzetta-connector-0.7.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     "proto-plus >= 1.22.0, <2.0.0dev",
     "packaging >= 14.3, <24.0.0dev",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
     "python-dateutil >= 2.7.2, <3.0dev",
     "requests >= 2.21.0, < 3.0.0dev",
     "pyarrow >= 11.0.0",
     "sqlalchemy==2.0.6",
-    "ossfs >= 2023.1.0"
+    "ossfs >= 2023.1.0",
+    "sqlparse >= 0.4.1",
 ]
 extras = {
     "pandas": ["pandas>=1.0.0", "db-dtypes>=0.3.0,<2.0.0dev"],
     "ipywidgets": ["ipywidgets==7.7.1"],
     "geopandas": ["geopandas>=0.9.0, <1.0dev", "Shapely>=1.6.0, <2.0dev"],
     "ipython": ["ipython>=7.0.1,!=8.1.0"],
     "tqdm": ["tqdm >= 4.7.4, <5.0.0dev"],
```

